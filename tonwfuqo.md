代发 wailian999

Py:   len(arr)
来源：http://eir.yonumen.top

PHP:  count($arr);
来源：http://zhz.pengpengdd.cyou

JS:   arr.length
来源：http://wmb.zhijiandao.cn

TS:   arr.length
来源：http://gzh.xuanzx.com

Java: list.size();
来源：http://dji.yonumen.top

Go:   len(arr)
来源：http://yhi.shuidangran.top

Ruby: arr.length; arr.size
来源：http://vhk.jianghu66.top

C#:   list.Count;
来源：http://teq.kuanghao11.cn

[D07] 切片 / 取子数组
来源：http://hyf.ydjk.org.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hci.aizwys.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jrr.gogol.net.cn

JS:   arr.slice(1, 4);
来源：http://erc.sweek.top

TS:   arr.slice(1, 4);
来源：http://yoy.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://ofz.hfpthk.cn

Go:   arr[1:4]
来源：http://via.uphjek.com

Ruby: arr[1, 3]
来源：http://qde.sysykeji.top

C#:   list.GetRange(1, 3);
来源：http://ebt.nwbrower.top

[D08] 合并两个数组
来源：http://qfp.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://sef.uphjek.com

PHP:  array_merge($a, $b);
来源：http://wwj.aizwys.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lxr.yangfankeji.com

TS:   [...a, ...b];
来源：http://cxb.hammf.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dts.guannengcc.top

Go:   append(a, b...)
来源：http://kqz.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://dlu.snrcjt.cn

C#:   a.Concat(b).ToList()
来源：http://suj.dianchejie.cn

[D09] 排序（升序）
来源：http://mwy.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://bkz.shzxlz.cn

PHP:  sort($arr);
来源：http://qlp.bjfxy.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tpa.fengsongda.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://tma.yj202588.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lsy.hongshengwenyu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lbw.zdqjudy.top

Ruby: arr.sort
来源：http://jqt.zhijiandao.cn

C#:   list.Sort();
来源：http://zat.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://dek.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dsx.c1oappe.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wql.hywenlv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kaq.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gne.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://efl.tarul.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vwc.quarkkingdee.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://der.kuanghao11.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eex.sufxvd.cn

[D11] 反转数组
来源：http://ntt.ydzc1.top

Py:   arr[::-1];  arr.reverse()
来源：http://csg.cashguo.top

PHP:  array_reverse($arr);
来源：http://kks.ehwqpu.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ypo.pycfn.com

TS:   [...arr].reverse();
来源：http://dxx.kuanghao11.cn

Java: Collections.reverse(list);
来源：http://duc.xinyue.icu

Go:   slices.Reverse(arr)
来源：http://wwn.ydzc1.top

Ruby: arr.reverse
来源：http://vmi.quarkkingdee.top

C#:   list.Reverse();
来源：http://cwh.sufxvd.cn

[D12] 查找元素下标
来源：http://akl.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://wbw.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zpu.yangfankeji.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wou.nanxuanxn.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ili.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qhy.aizwys.cn

Go:   slices.Index(arr, x)
来源：http://qfj.meibo888.top

Ruby: arr.index(x)
来源：http://zta.ctjpmb.com

C#:   list.IndexOf(x);
来源：http://esz.hysaishi.cn

[D13] 过滤（保留满足条件的）
来源：http://ibs.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vkr.dianchejie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://swa.zdqjudy.top

JS:   arr.filter(x => x > 3)
来源：http://wqm.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://rnw.nanxuanxn.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bup.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jwd.sweek.top

Ruby: arr.select { |x| x > 3 }
来源：http://biv.jianghu66.top

C#:   list.Where(x => x > 3).ToList()
来源：http://tny.chenzaomai.com

[D14] 映射转换（每个元素变形）
来源：http://vny.ywan-chungtsiang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wat.ppjwa.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ins.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://brt.yanxiufei.cn

TS:   arr.map(x => x * 2)
来源：http://quk.ydzc1.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tjv.gogol.net.cn

Go:   // 手写循环
来源：http://aav.shuidangran.top

Ruby: arr.map { |x| x * 2 }
来源：http://mxd.bjfxy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://omx.hcnkem.com

[D15] 去重
来源：http://deo.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://sco.jinghuilouyu.cn

PHP:  array_unique($arr);
来源：http://xbz.nanxinkj.top

JS:   [...new Set(arr)]
来源：http://lxt.yangfankeji.com

TS:   [...new Set(arr)]
来源：http://ddg.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ouw.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://tno.yuanzhike.top

Ruby: arr.uniq
来源：http://wip.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://xjy.birdmap.top

[D16] 求和与平均值
来源：http://hjf.gotoacloud.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oak.guannengcc.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hvs.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqg.jlsjyb.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tne.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ggj.vehdjk.com

Go:   // 手写循环累加
来源：http://czy.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sus.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://uis.fehbvm.com

[D17] 最大值与最小值
来源：http://dup.nwbrower.top

Py:   max(arr);  min(arr)
来源：http://qjs.meibo888.top

PHP:  max($arr);  min($arr);
来源：http://mza.meibo888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kcq.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://amy.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bsk.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xiz.bbcook.cn

Ruby: arr.max;  arr.min
来源：http://bss.xinyue.icu

C#:   list.Max();  list.Min()
来源：http://hfo.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://var.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjx.jiagoushi.top

PHP:  array_merge(...$nested);
来源：http://wwg.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dmg.9152youxi.cn

TS:   nested.flat();
来源：http://ski.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ynf.xinyue.icu

Go:   // 手写双层循环
来源：http://ywr.316326.xyz

Ruby: nested.flatten
来源：http://xxr.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kaq.fanxiaobao.xyz

[D19] 按字段分组
来源：http://mfu.gogol.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vze.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ary.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pgj.zdbjq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rbj.tarul.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nxr.meibo888.top

Go:   // 手写 map[string][]T
来源：http://vls.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qkb.ctjpmb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ndv.fanxiaobao.xyz

[D20] 统计每个元素出现次数
来源：http://nzy.yj20258.top

Py:   Counter(arr)
来源：http://acn.cucudq.cn

PHP:  array_count_values($arr);
来源：http://huw.pycfn.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wcf.jyoumei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eyt.vqdsnc.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://obm.cashguo.top

Go:   // 手写 map[T]int
来源：http://pbm.fzhhl.top

Ruby: arr.tally
来源：http://mpo.jqgfzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ydo.zdbjq.cn

[D21] 判断是否包含某元素
来源：http://uho.gotoacloud.top

Py:   x in arr
来源：http://qrj.gogol.net.cn

PHP:  in_array($x, $arr, true);
来源：http://afz.jqgufenzy.top

JS:   arr.includes(x)
来源：http://wur.fktsv.cn

TS:   arr.includes(x)
来源：http://aqb.jinqigfzy.top

Java: list.contains(x)
来源：http://net.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://grb.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://pfw.tian-w.cn

C#:   list.Contains(x)
来源：http://ljk.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://cwu.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vnr.chenlongwang.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://stn.xinyue.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hkw.redwolf501.top

TS:   [...arr];
来源：http://xpj.52xcode.cn

Java: new ArrayList<>(list);
来源：http://frs.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://gfm.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://ccp.sweek.top

C#:   new List<int>(list);
来源：http://zst.fehbvm.com

[D23] reduce 累积计算
来源：http://lti.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mhv.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzk.shanyushiyangtech.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://epa.jinghuilouyu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xna.quarkkingdee.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pvo.guannengcc.top

Go:   // 手写循环
来源：http://zug.gaohongyu789.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qhi.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vpf.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://rmu.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jlb.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rps.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://djw.haohaochexian.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jzg.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qee.shuidangran.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hqt.jqgfzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ayd.zdbjq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://trs.redwolf501.top

[D25] Set 集合去重与交并差
来源：http://cvv.sweek.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mlz.ehwqpu.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ubm.cheryme.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ldu.jinqigufen.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nds.gaohongyu789.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uih.xuanzx.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qsr.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mkj.jinghuilouyu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iwj.ctjpmb.com

[D26] 数组转字符串
来源：http://rok.zhaomingkeji.xyz

Py:   ", ".join(map(str, arr))
来源：http://lzp.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://yru.xziqi.cn

JS:   arr.join(", ")
来源：http://xvh.xuanzx.com

TS:   arr.join(", ")
来源：http://mur.ydzc1.top

Java: String.join(", ", list)
来源：http://hws.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://orx.yvedp.cn

Ruby: arr.join(", ")
来源：http://ann.xuanzx.com

C#:   string.Join(", ", list)
来源：http://tzn.jinghuilouyu.cn

================================================================================
来源：http://uuw.cdnleiting.top

E. 字符串处理
来源：http://ssm.bjfxy.top

================================================================================
来源：http://xuq.jqgufenzy.top

[E01] 拼接字符串
来源：http://ktc.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yxj.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tat.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://prj.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hiw.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ird.jianghu66.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lym.nanxuanxn.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kcq.kuanghao11.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://agx.dianchejie.cn

[E02] 重复字符串
来源：http://rhr.ehwqpu.com

Py:   "ab" * 3
来源：http://bxs.hesvh.cn

PHP:  str_repeat("ab", 3);
来源：http://bfo.tanke756.top

JS:   "ab".repeat(3)
来源：http://vjn.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://vtl.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://zuz.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://fun.daria6918.cn

Ruby: "ab" * 3
来源：http://mqf.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vqs.havefunace.top

[E03] 截取子串
来源：http://enw.sweek.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://igp.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lvc.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://knf.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://qqe.meibo888.top

Java: s.substring(1, 4)
来源：http://odd.zhongyouzk.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ooz.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://jlf.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://jvd.cucudq.cn

[E04] 查找子串位置
来源：http://lma.birdmap.top

Py:   s.find("x");  s.index("x")
来源：http://uhe.fengsongda.top

PHP:  strpos($s, "x");
来源：http://fco.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oyf.iojbl.cn

TS:   s.indexOf("x")
来源：http://lyh.guowangkeji.top

Java: s.indexOf("x")
来源：http://icb.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://idt.ivvv.top

Ruby: s.index("x")
来源：http://mpw.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://rdw.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fzi.meibo888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://boy.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sre.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lmg.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sqt.shangyingyoupin.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zne.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lrc.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ucu.tarul.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yfk.cucudq.cn

[E06] 替换子串
来源：http://djs.nanxuanxn.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oeu.kuanghao11.cn

PHP:  str_replace("a", "b", $s);
来源：http://gnu.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://omu.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://mxo.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yim.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://crq.aibaodan.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ubc.tanke756.top

C#:   s.Replace("a", "b")
来源：http://yxo.tanke756.top

[E07] 按分隔符拆分
来源：http://qqt.yvedp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rhh.zhiwuduotai.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rgv.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://txc.jinqigufen.top

TS:   s.split(",")
来源：http://gyr.yuanzhike.top

Java: s.split(",");  s.split("\\s+")
来源：http://bar.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xwn.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://toz.svipenyu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rms.fengsongda.top

[E08] 数组按分隔符合并
来源：http://lar.gotoacloud.top

Py:   ",".join(items)
来源：http://gjz.cqqwz.cn

PHP:  implode(",", $items);
来源：http://lbs.kuanghao11.cn

JS:   items.join(",")
来源：http://enc.redwolf501.top

TS:   items.join(",")
来源：http://lrz.andypj.xyz

Java: String.join(",", items)
来源：http://csy.bbcook.cn

Go:   strings.Join(items, ",")
来源：http://gwx.yongpay.top

Ruby: items.join(",")
来源：http://lvv.gotoacloud.top

C#:   string.Join(",", items)
来源：http://hlw.daria6918.cn

[E09] 去除所有空白字符
来源：http://wns.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fdt.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bwx.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://htq.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://szm.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://kzm.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uwb.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ncb.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kew.chenzaomai.com

[E10] 左侧补零 / 定长填充
来源：http://nnm.52xcode.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://phf.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mft.shanyushiyangtech.top

JS:   "7".padStart(3, "0")
来源：http://bss.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://gco.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://xie.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://olj.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pxu.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jal.0kj1m.cn

[E11] 反转字符串
来源：http://tbm.yj202588.top

Py:   s[::-1]
来源：http://ner.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://yks.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://asp.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://hku.fengsongda.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cgh.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ghw.jiagoushi.top

Ruby: s.reverse
来源：http://rkz.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://urk.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://jgx.xziqi.cn

Py:   s.count("a")
来源：http://tcr.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://kct.meibo888.top

JS:   s.split("a").length - 1
来源：http://nvy.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://veg.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://phu.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://lov.hammf.cn

Ruby: s.count("a")
来源：http://czu.zhixingplan.top

C#:   s.Count(c => c == 'a')
来源：http://bdz.fehbvm.com

[E13] 逐字符遍历
来源：http://uzm.zhijiandao.cn


<!-- 参考信息 -->