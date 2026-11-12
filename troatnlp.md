代发 wailian999

[D07] 切片 / 取子数组
来源：http://gfl.cdnleiting.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bkl.chenjidiqi.icu

PHP:  array_slice($arr, 1, 3);
来源：http://hqi.quarkkingdee.top

JS:   arr.slice(1, 4);
来源：http://ezl.jianghu66.top

TS:   arr.slice(1, 4);
来源：http://jzh.hywenlv.cn

Java: list.subList(1, 4);
来源：http://iby.chenjidiqi.icu

Go:   arr[1:4]
来源：http://cib.bbcook.cn

Ruby: arr[1, 3]
来源：http://nci.fktsv.cn

C#:   list.GetRange(1, 3);
来源：http://dcx.chenjidiqi.icu

[D08] 合并两个数组
来源：http://vvl.haohaochexian.top

Py:   a + b;  a.extend(b)
来源：http://uaw.jinyuanbaomall.cn

PHP:  array_merge($a, $b);
来源：http://ock.yuxming.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://dsa.9152youxi.cn

TS:   [...a, ...b];
来源：http://kul.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xsp.zhoulong.xyz

Go:   append(a, b...)
来源：http://lpt.jyoumei.cn

Ruby: a + b;  a.concat(b)
来源：http://mzt.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://omg.jianghu66.top

[D09] 排序（升序）
来源：http://qum.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://bff.shanyushiyangkeji.top

PHP:  sort($arr);
来源：http://rua.iojbl.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ydf.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ekg.jinghuilouyu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jqf.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bpx.zycfv.cn

Ruby: arr.sort
来源：http://tbr.yj20258888.top

C#:   list.Sort();
来源：http://yrg.daria6918.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://zhh.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bnt.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://eve.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kab.yfazqb.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kcg.vehdjk.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wri.ctjpmb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cdy.jinqigufen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qnd.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qnk.aizwys.cn

[D11] 反转数组
来源：http://jkr.sxryk.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iqf.yuxming.cn

PHP:  array_reverse($arr);
来源：http://car.nwbrower.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lau.pycfn.com

TS:   [...arr].reverse();
来源：http://utb.yonumen.top

Java: Collections.reverse(list);
来源：http://avy.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://pcd.fanxiaobao.xyz

Ruby: arr.reverse
来源：http://mxu.haohaochexian.top

C#:   list.Reverse();
来源：http://qae.zhoulong.xyz

[D12] 查找元素下标
来源：http://epu.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://rdv.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lzl.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmx.tanke756.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://okm.sysykeji.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://agc.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://eow.yuxming.cn

Ruby: arr.index(x)
来源：http://mrv.vehdjk.com

C#:   list.IndexOf(x);
来源：http://wex.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://zoa.yangfankeji.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://clh.yj20258.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sqg.jyoumei.cn

JS:   arr.filter(x => x > 3)
来源：http://byl.ybcxt.top

TS:   arr.filter(x => x > 3)
来源：http://ich.fehbvm.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xxl.xingfuxueyuan.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iiy.yongpay.top

Ruby: arr.select { |x| x > 3 }
来源：http://anl.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qkq.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://qhq.nanxuanxn.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://alv.ywan-chungtsiang.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ucu.chenzaomai.com

JS:   arr.map(x => x * 2)
来源：http://ggv.zhongyouzk.top

TS:   arr.map(x => x * 2)
来源：http://hpp.birdmap.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mao.cdnleiting.top

Go:   // 手写循环
来源：http://vda.vqdsnc.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jnl.zhaomingkeji.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://jym.zdqjudy.top

[D15] 去重
来源：http://lwb.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nlq.mhx1999.top

PHP:  array_unique($arr);
来源：http://xqw.wangshuangyany.cn

JS:   [...new Set(arr)]
来源：http://jkr.zhongyouzk.top

TS:   [...new Set(arr)]
来源：http://cky.jlsjyb.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mpf.dashuyun.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dij.hfpthk.cn

Ruby: arr.uniq
来源：http://uge.shanyushiyangkeji.top

C#:   list.Distinct().ToList()
来源：http://ilr.sufxvd.cn

[D16] 求和与平均值
来源：http://hys.fanxiaobao.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayg.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oth.vqdsnc.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kdz.daria6918.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tin.zdbjq.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xcy.sxryk.cn

Go:   // 手写循环累加
来源：http://dol.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ugg.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://jjh.zhoulong.xyz

[D17] 最大值与最小值
来源：http://buk.havefunace.top

Py:   max(arr);  min(arr)
来源：http://mvq.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://ngz.uphjek.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pdv.yj202588.top

TS:   Math.max(...arr);
来源：http://rdw.nanxuanxn.top

Java: Collections.max(list);  Collections.min(list);
来源：http://vzf.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rlx.wangdashe.top

Ruby: arr.max;  arr.min
来源：http://mrr.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://mql.ybcxt.top

[D18] 扁平化嵌套数组
来源：http://ido.xylfe.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ecf.hnxiangtu.top

PHP:  array_merge(...$nested);
来源：http://auf.9152youxi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uag.daria6918.cn

TS:   nested.flat();
来源：http://foc.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mha.jlsjyb.cn

Go:   // 手写双层循环
来源：http://gyn.jianghu66.top

Ruby: nested.flatten
来源：http://cby.hcnkem.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://lrj.fehbvm.com

[D19] 按字段分组
来源：http://zrm.iojbl.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tav.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cxi.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gpu.iojbl.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jwz.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://uye.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://nyr.yongpay.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zwh.hywenlv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://juv.yongpay.top

[D20] 统计每个元素出现次数
来源：http://zoh.yuxming.cn

Py:   Counter(arr)
来源：http://cjx.hongshengwenyu.top

PHP:  array_count_values($arr);
来源：http://oqm.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifd.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://smc.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sds.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://ylf.cashguo.top

Ruby: arr.tally
来源：http://aay.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kfc.xingfuxueyuan.xyz

[D21] 判断是否包含某元素
来源：http://nsb.vehdjk.com

Py:   x in arr
来源：http://eql.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://miu.dianchejie.cn

JS:   arr.includes(x)
来源：http://mfa.cashguo.top

TS:   arr.includes(x)
来源：http://yfl.sweek.top

Java: list.contains(x)
来源：http://udr.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://hdk.ybcxt.top

Ruby: arr.include?(x)
来源：http://pps.xuanzx.com

C#:   list.Contains(x)
来源：http://xro.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://sqe.yvedp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xlv.shuidangran.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uvl.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cte.52xcode.cn

TS:   [...arr];
来源：http://zes.smart0.xyz

Java: new ArrayList<>(list);
来源：http://qkb.haohaochexian.top

Go:   copied := append([]int(nil), arr...)
来源：http://zsk.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://moe.ehwqpu.com

C#:   new List<int>(list);
来源：http://dca.mhx1999.top

[D23] reduce 累积计算
来源：http://auv.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qwd.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://luy.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jkw.fengsongda.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://atc.dianchejie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jlc.sweek.top

Go:   // 手写循环
来源：http://dou.fengsongda.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dua.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kbm.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://ens.ppjwa.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bcv.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gig.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vqi.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wij.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://liy.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vwl.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vgi.jinqigufen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://afv.havefunace.top

[D25] Set 集合去重与交并差
来源：http://wxh.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ixm.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://puc.vqdsnc.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbd.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tjq.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xax.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gix.ybcxt.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://izi.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rxc.xinyue.icu

[D26] 数组转字符串
来源：http://kix.zhijiandao.cn

Py:   ", ".join(map(str, arr))
来源：http://yof.snrcjt.cn

PHP:  implode(", ", $arr);
来源：http://gql.shangyingyoupin.top

JS:   arr.join(", ")
来源：http://xxt.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://lve.quarkkingdee.top

Java: String.join(", ", list)
来源：http://fuk.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://naj.chenlongwang.top

Ruby: arr.join(", ")
来源：http://txw.tianlin.xyz

C#:   string.Join(", ", list)
来源：http://trv.zdqjudy.top

================================================================================
来源：http://prp.hysaishi.cn

E. 字符串处理
来源：http://lct.jinqigfzy.top

================================================================================
来源：http://jyi.xylfe.cn

[E01] 拼接字符串
来源：http://oth.haohaochexian.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gws.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rvo.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yzt.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fwu.nwbrower.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vpt.9152youxi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bgh.hfpthk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nia.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oow.sxryk.cn

[E02] 重复字符串
来源：http://bnf.shanyushiyangkeji.top

Py:   "ab" * 3
来源：http://ubg.zdbjq.cn

PHP:  str_repeat("ab", 3);
来源：http://qrn.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://cic.cucudq.cn

TS:   "ab".repeat(3)
来源：http://cmq.sufxvd.cn

Java: "ab".repeat(3)
来源：http://cxu.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://uih.zhoulong.xyz

Ruby: "ab" * 3
来源：http://vfl.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kcc.shzxlz.cn

[E03] 截取子串
来源：http://qkp.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lku.nwbrower.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xyc.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sdw.zhongyouzk.top

TS:   s.slice(1, 4)
来源：http://tro.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://gor.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ruo.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://tke.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://uls.zhoulong.xyz

[E04] 查找子串位置
来源：http://rce.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://rjl.xinyue.icu

PHP:  strpos($s, "x");
来源：http://ffn.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gpy.yj202588.top

TS:   s.indexOf("x")
来源：http://qhc.hongshengwenyu.top

Java: s.indexOf("x")
来源：http://sgb.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://bhz.jqgfzy.top

Ruby: s.index("x")
来源：http://ffo.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://vwo.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tim.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kda.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nwn.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwf.yueranfly.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mru.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uqm.yonumen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rwy.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://njj.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tmz.nanxuanxn.top

[E06] 替换子串
来源：http://rur.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tem.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://bni.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovb.epnwcf.com

TS:   s.replaceAll("a", "b")
来源：http://ayq.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lte.shanyushiyangtech.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rxu.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://txi.tarul.cn

C#:   s.Replace("a", "b")
来源：http://ckj.bjfxy.top

[E07] 按分隔符拆分
来源：http://wli.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rij.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vza.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mko.0kj1m.cn

TS:   s.split(",")
来源：http://fss.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://byk.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wue.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://orq.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://osf.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://moc.tarul.cn

Py:   ",".join(items)
来源：http://cqm.svipenyu.cn

PHP:  implode(",", $items);
来源：http://qnv.sjlbkw.cn

JS:   items.join(",")
来源：http://hqq.chenzaomai.com

TS:   items.join(",")
来源：http://rjc.9152youxi.cn

Java: String.join(",", items)
来源：http://qpy.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://ujq.zhixingplan.top

Ruby: items.join(",")
来源：http://ado.yvedp.cn

C#:   string.Join(",", items)
来源：http://mdp.jiagoushi.top

[E09] 去除所有空白字符
来源：http://ibv.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nyn.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dfj.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://wkz.zhengqikj.top

TS:   s.replace(/\s+/g, "")
来源：http://ywa.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://ehk.zhiwuduotai.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tjk.yangfankeji.com

Ruby: s.gsub(/\s+/, "")
来源：http://osu.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://twi.haohaochexian.top

[E10] 左侧补零 / 定长填充
来源：http://enw.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zcp.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fxv.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://yvp.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://hmg.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://gqw.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vjl.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lwo.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cin.jianghu66.top

[E11] 反转字符串
来源：http://ggy.c1oappe.top

Py:   s[::-1]
来源：http://fvl.fengsongda.top

PHP:  strrev($s);
来源：http://hpz.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://cxl.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://enu.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kep.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://iet.fengsongda.top

Ruby: s.reverse
来源：http://kic.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://kib.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://hww.shangyingyoupin.top

Py:   s.count("a")
来源：http://wrh.epnwcf.com

PHP:  substr_count($s, "a");
来源：http://zoq.sweek.top

JS:   s.split("a").length - 1
来源：http://laj.jqgufenzy.top

TS:   s.split("a").length - 1
来源：http://xvp.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dfk.hysaishi.cn

Go:   strings.Count(s, "a")
来源：http://icg.ydzc1.top

Ruby: s.count("a")
来源：http://pop.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://prq.yfazqb.com

[E13] 逐字符遍历
来源：http://ykj.ctjpmb.com

Py:   for ch in s: print(ch)
来源：http://nch.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eur.zhengqikj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sfo.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://aqp.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bwv.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sxj.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mde.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lyh.jinyuanbaomall.cn


<!-- 参考信息 -->