代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://duc.sysykeji.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ype.ydjk.org.cn

[D05] 访问与修改元素
来源：http://pmv.zycfv.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zpv.yueranfly.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://rrj.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gog.smart0.xyz

TS:   arr[0]; arr.at(-1);
来源：http://cjf.52xcode.cn

Java: list.get(0); list.set(0, 9);
来源：http://yme.dashuyun.cn

Go:   arr[0]; arr[0] = 9
来源：http://ixq.jinqigfzy.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pyx.pycfn.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://llt.shanyushiyangtech.top

[D06] 数组长度
来源：http://otx.redwolf501.top

Py:   len(arr)
来源：http://jwx.aizwys.cn

PHP:  count($arr);
来源：http://qis.guannengcc.top

JS:   arr.length
来源：http://kgg.cucudq.cn

TS:   arr.length
来源：http://apl.tarul.cn

Java: list.size();
来源：http://pod.fktsv.cn

Go:   len(arr)
来源：http://abr.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://ort.yuxming.cn

C#:   list.Count;
来源：http://smp.bbcook.cn

[D07] 切片 / 取子数组
来源：http://hdu.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cll.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://xme.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://xmu.jlsjyb.cn

TS:   arr.slice(1, 4);
来源：http://vey.yj202588.top

Java: list.subList(1, 4);
来源：http://hvh.svipenyu.cn

Go:   arr[1:4]
来源：http://kin.uphjek.com

Ruby: arr[1, 3]
来源：http://bcq.jqgfzy.top

C#:   list.GetRange(1, 3);
来源：http://sqj.zhijiandao.cn

[D08] 合并两个数组
来源：http://xyd.ywan-chungtsiang.top

Py:   a + b;  a.extend(b)
来源：http://dxx.snrcjt.cn

PHP:  array_merge($a, $b);
来源：http://kde.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://jyy.havefunace.top

TS:   [...a, ...b];
来源：http://lnk.shangyingyoupin.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qis.0kj1m.cn

Go:   append(a, b...)
来源：http://lqe.dashuyun.cn

Ruby: a + b;  a.concat(b)
来源：http://syf.daxiang520.top

C#:   a.Concat(b).ToList()
来源：http://nfn.yongpay.top

[D09] 排序（升序）
来源：http://qzm.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://xgf.wangdashe.top

PHP:  sort($arr);
来源：http://erj.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fxx.chenzaomai.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tse.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://apt.nwbrower.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lao.haohaochexian.top

Ruby: arr.sort
来源：http://htb.cqqwz.cn

C#:   list.Sort();
来源：http://kry.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pmy.daxiang520.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://igc.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zcs.xuanzx.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ecx.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bts.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hoc.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bme.xingfuxueyuan.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zpz.cdnleiting.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lwa.mhx1999.top

[D11] 反转数组
来源：http://eys.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://bid.smart0.xyz

PHP:  array_reverse($arr);
来源：http://baz.cheryme.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mnt.daxiang520.top

TS:   [...arr].reverse();
来源：http://xop.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://hkm.sxryk.cn

Go:   slices.Reverse(arr)
来源：http://ogv.shuidangran.top

Ruby: arr.reverse
来源：http://smy.yj202588.top

C#:   list.Reverse();
来源：http://qvd.wangshuangyany.cn

[D12] 查找元素下标
来源：http://szm.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://awi.jlsjyb.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pan.shanyushiyangtech.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dam.dianchejie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tyg.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sru.fzhhl.top

Go:   slices.Index(arr, x)
来源：http://joj.kuanghao11.cn

Ruby: arr.index(x)
来源：http://kjq.wangdashe.top

C#:   list.IndexOf(x);
来源：http://qjq.shanyushiyangkeji.top

[D13] 过滤（保留满足条件的）
来源：http://shk.dianchejie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mhn.hnxiangtu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ffe.316326.xyz

JS:   arr.filter(x => x > 3)
来源：http://ual.birdmap.top

TS:   arr.filter(x => x > 3)
来源：http://kyq.epnwcf.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fwt.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uyy.fktsv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://dfk.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pyc.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://suu.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wtq.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lse.wangshuangyany.cn

JS:   arr.map(x => x * 2)
来源：http://ecl.ctjpmb.com

TS:   arr.map(x => x * 2)
来源：http://jmc.aibaodan.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fmu.hesvh.cn

Go:   // 手写循环
来源：http://bjh.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://phi.nwbrower.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cmc.xylfe.cn

[D15] 去重
来源：http://sxb.yonumen.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://elk.shuidangran.top

PHP:  array_unique($arr);
来源：http://pyh.hnxiangtu.top

JS:   [...new Set(arr)]
来源：http://ynp.hnqzz.top

TS:   [...new Set(arr)]
来源：http://afi.shangyingyoupin.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jds.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://jhe.vqdsnc.cn

Ruby: arr.uniq
来源：http://lam.nanxinkj.top

C#:   list.Distinct().ToList()
来源：http://sou.yj202588.top

[D16] 求和与平均值
来源：http://hgf.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gzo.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uvj.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjv.snrcjt.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://alr.jlsjyb.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://val.hnxiangtu.top

Go:   // 手写循环累加
来源：http://ahv.hnqzz.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://skh.cashguo.top

C#:   list.Sum();  list.Average()
来源：http://uas.9152youxi.cn

[D17] 最大值与最小值
来源：http://dnr.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://bfb.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://zxk.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://keo.hfpthk.cn

TS:   Math.max(...arr);
来源：http://eaf.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://fty.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mmx.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://icq.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://vzn.cashguo.top

[D18] 扁平化嵌套数组
来源：http://fwj.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://woe.gaohongyu789.top

PHP:  array_merge(...$nested);
来源：http://yoi.shangyingyoupin.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sps.chenlongwang.top

TS:   nested.flat();
来源：http://nbi.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://alt.jinqigfzy.top

Go:   // 手写双层循环
来源：http://mbh.c1oappe.top

Ruby: nested.flatten
来源：http://muu.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://biv.gaohongyu789.top

[D19] 按字段分组
来源：http://nzr.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kbo.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eid.ivvv.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oko.fanxiaobao.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://zzx.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ffs.shuidangran.top

Go:   // 手写 map[string][]T
来源：http://kuo.yueranfly.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://hkn.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cuc.zhongyouzk.top

[D20] 统计每个元素出现次数
来源：http://fkh.chenlongwang.top

Py:   Counter(arr)
来源：http://upp.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://ocb.svipenyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ifo.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbf.fehbvm.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fhp.smart0.xyz

Go:   // 手写 map[T]int
来源：http://hxv.zycfv.cn

Ruby: arr.tally
来源：http://pxm.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bjm.cdnleiting.top

[D21] 判断是否包含某元素
来源：http://inf.feifeiyinyue.top

Py:   x in arr
来源：http://ynn.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://oab.tarul.cn

JS:   arr.includes(x)
来源：http://czq.bjfxy.top

TS:   arr.includes(x)
来源：http://tfy.fanxiaobao.xyz

Java: list.contains(x)
来源：http://xbq.ydjk.org.cn

Go:   slices.Contains(arr, x)
来源：http://zos.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://mqv.fzhhl.top

C#:   list.Contains(x)
来源：http://rxm.ivvv.top

[D22] 复制数组（避免共享引用）
来源：http://eln.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lgn.ctjpmb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zen.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wdm.vehdjk.com

TS:   [...arr];
来源：http://xth.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://cbb.jinghuilouyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wyy.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://hml.bjfxy.top

C#:   new List<int>(list);
来源：http://fls.guannengcc.top

[D23] reduce 累积计算
来源：http://rih.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://trl.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gzs.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pyj.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjn.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://poe.redwolf501.top

Go:   // 手写循环
来源：http://bkb.ivvv.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dsh.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qgw.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://qpr.hysaishi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pcy.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gng.ehwqpu.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://djd.jinqigufen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rkw.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pfq.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cbz.hesvh.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://for.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejj.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://kba.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ini.zhaomingkeji.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pld.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ttb.zycfv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bau.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blt.jqgfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wde.yj202588.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fwc.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qla.yangfankeji.com

[D26] 数组转字符串
来源：http://snu.xylfe.cn

Py:   ", ".join(map(str, arr))
来源：http://aim.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://xek.shanyushiyangtech.top

JS:   arr.join(", ")
来源：http://tim.fengsongda.top

TS:   arr.join(", ")
来源：http://nus.ehwqpu.com

Java: String.join(", ", list)
来源：http://voa.ehwqpu.com

Go:   strings.Join(strs, ", ")
来源：http://rea.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://fiu.wangdashe.top

C#:   string.Join(", ", list)
来源：http://gtq.xuanzx.com

================================================================================
来源：http://cky.mhx1999.top

E. 字符串处理
来源：http://lor.pycfn.com

================================================================================
来源：http://dhj.tianlin.xyz

[E01] 拼接字符串
来源：http://jou.gaohongyu789.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ytj.yvedp.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fzz.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://clv.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pmc.zhengqikj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://osu.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qwt.mhx1999.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hvk.xuanzx.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bvh.pycfn.com

[E02] 重复字符串
来源：http://tng.cashguo.top

Py:   "ab" * 3
来源：http://lxx.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://hhj.mhx1999.top

JS:   "ab".repeat(3)
来源：http://ers.meibo888.top

TS:   "ab".repeat(3)
来源：http://hea.yj202588.top

Java: "ab".repeat(3)
来源：http://pte.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://fwk.52xcode.cn

Ruby: "ab" * 3
来源：http://pqo.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hze.zhiwuduotai.top

[E03] 截取子串
来源：http://hji.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jdc.snrcjt.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://klk.smart0.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bxj.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://slc.epnwcf.com

Java: s.substring(1, 4)
来源：http://ojt.mhx1999.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ndj.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://ljc.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://jdq.tian-w.cn

[E04] 查找子串位置
来源：http://gjj.yanxiufei.cn

Py:   s.find("x");  s.index("x")
来源：http://rmz.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://rlz.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mld.316326.xyz

TS:   s.indexOf("x")
来源：http://afj.xuanzx.com

Java: s.indexOf("x")
来源：http://art.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://aqd.mhx1999.top

Ruby: s.index("x")
来源：http://myb.pycfn.com

C#:   s.IndexOf("x")
来源：http://xcl.jlsjyb.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://whp.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fcw.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yht.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vwl.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://ivs.yanxiufei.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mrr.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eyb.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xuk.snrcjt.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://igu.epnwcf.com

[E06] 替换子串
来源：http://hgf.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iic.jqgufenzy.top

PHP:  str_replace("a", "b", $s);
来源：http://oxh.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iep.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://uze.fzhhl.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbz.sysykeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hqr.fzhhl.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yba.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://ies.yongpay.top

[E07] 按分隔符拆分
来源：http://edu.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://goj.yanxiufei.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bkc.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vwq.52xcode.cn

TS:   s.split(",")
来源：http://cdy.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://blg.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pke.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://jcm.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcg.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://udg.quarkkingdee.top

Py:   ",".join(items)
来源：http://jdr.pengpengdd.cyou

PHP:  implode(",", $items);
来源：http://mrq.redwolf501.top

JS:   items.join(",")
来源：http://urj.nanxuanxn.top

TS:   items.join(",")
来源：http://xpd.cashguo.top

Java: String.join(",", items)
来源：http://vax.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://cpc.gaohongyu789.top

Ruby: items.join(",")
来源：http://rra.redwolf501.top

C#:   string.Join(",", items)
来源：http://eqk.tianlin.xyz

[E09] 去除所有空白字符
来源：http://dmy.kuanghao11.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mns.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xlg.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://dvz.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://pox.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://otz.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://efj.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ycd.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://guv.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://oul.chenlongwang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hzv.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://skf.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://zhh.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://hnj.hesvh.cn

Java: String.format("%03d", 7)
来源：http://saq.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qvi.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uyk.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mip.52xcode.cn

[E11] 反转字符串
来源：http://jqd.hnqzz.top

Py:   s[::-1]
来源：http://kgb.zhongyouzk.top

PHP:  strrev($s);
来源：http://pqn.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://lct.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://ijf.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://akj.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ykm.xuanzx.com


<!-- 参考信息 -->