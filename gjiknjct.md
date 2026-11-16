代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ewr.jlsjyb.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ntn.sufxvd.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dpj.zhixingplan.top

[D06] 数组长度
来源：http://vun.yfazqb.com

Py:   len(arr)
来源：http://hcb.shzxlz.cn

PHP:  count($arr);
来源：http://zrc.nwbrower.top

JS:   arr.length
来源：http://jzr.c1oappe.top

TS:   arr.length
来源：http://wes.tian-w.cn

Java: list.size();
来源：http://zaa.yj202588.top

Go:   len(arr)
来源：http://nwk.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://ilj.hongshengwenyu.top

C#:   list.Count;
来源：http://xks.yj20258.top

[D07] 切片 / 取子数组
来源：http://azs.ywan-chungtsiang.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://cof.yongpay.top

PHP:  array_slice($arr, 1, 3);
来源：http://vxl.yonumen.top

JS:   arr.slice(1, 4);
来源：http://mwd.fktsv.cn

TS:   arr.slice(1, 4);
来源：http://lrl.cqqwz.cn

Java: list.subList(1, 4);
来源：http://btn.jinqigfzy.top

Go:   arr[1:4]
来源：http://xzt.ppjwa.cn

Ruby: arr[1, 3]
来源：http://mjs.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://pfi.fehbvm.com

[D08] 合并两个数组
来源：http://hjs.sjlbkw.cn

Py:   a + b;  a.extend(b)
来源：http://pkg.zhijiandao.cn

PHP:  array_merge($a, $b);
来源：http://bcb.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://dzz.fehbvm.com

TS:   [...a, ...b];
来源：http://qsf.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gzr.hesvh.cn

Go:   append(a, b...)
来源：http://xlp.aizwys.cn

Ruby: a + b;  a.concat(b)
来源：http://out.birdmap.top

C#:   a.Concat(b).ToList()
来源：http://xvh.vehdjk.com

[D09] 排序（升序）
来源：http://evb.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://dtg.nanxinkj.top

PHP:  sort($arr);
来源：http://npp.jinghuilouyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://dlw.wangdashe.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://rvg.hnxiangtu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://cdp.zhongyouzk.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tlq.yfazqb.com

Ruby: arr.sort
来源：http://nye.ywan-chungtsiang.top

C#:   list.Sort();
来源：http://ucn.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jlk.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qtm.chenzaomai.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xhg.cdnleiting.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pna.shuidangran.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://evl.aizwys.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nfb.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vqk.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ylx.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tsz.jqgfzy.top

[D11] 反转数组
来源：http://uwu.xziqi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ppn.guannengcc.top

PHP:  array_reverse($arr);
来源：http://bhj.bbcook.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qhc.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://lar.fzhhl.top

Java: Collections.reverse(list);
来源：http://aio.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://drg.jqgufenzy.top

Ruby: arr.reverse
来源：http://lxv.haohaochexian.top

C#:   list.Reverse();
来源：http://rdh.shanyushiyangkeji.top

[D12] 查找元素下标
来源：http://wgq.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://qmr.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dku.shzxlz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sgy.yj20258888.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ykh.ydjk.org.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oou.chenlongwang.top

Go:   slices.Index(arr, x)
来源：http://syb.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://upu.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://nts.ivvv.top

[D13] 过滤（保留满足条件的）
来源：http://skz.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tsl.redwolf501.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://heu.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://dfa.shanyushiyangkeji.top

TS:   arr.filter(x => x > 3)
来源：http://qje.hnxiangtu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aup.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbw.fehbvm.com

Ruby: arr.select { |x| x > 3 }
来源：http://pnd.xuetiantiany.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://djg.xylfe.cn

[D14] 映射转换（每个元素变形）
来源：http://xdq.tarul.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gjl.c1oappe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cfw.haohaochexian.top

JS:   arr.map(x => x * 2)
来源：http://ruk.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://htj.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qbd.daria6918.cn

Go:   // 手写循环
来源：http://kqm.yanxiufei.cn

Ruby: arr.map { |x| x * 2 }
来源：http://kbu.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uux.ctjpmb.com

[D15] 去重
来源：http://koc.smart0.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qte.sysykeji.top

PHP:  array_unique($arr);
来源：http://gdz.fengsongda.top

JS:   [...new Set(arr)]
来源：http://tta.yvedp.cn

TS:   [...new Set(arr)]
来源：http://vtr.0kj1m.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://agq.fehbvm.com

Go:   // 用 map[T]struct{} 手写
来源：http://mnu.epnwcf.com

Ruby: arr.uniq
来源：http://oue.aizwys.cn

C#:   list.Distinct().ToList()
来源：http://wvk.shangyingyoupin.top

[D16] 求和与平均值
来源：http://nqg.ydjk.org.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zae.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qoy.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://opl.9152youxi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kzw.zhengqikj.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pnb.guowangkeji.top

Go:   // 手写循环累加
来源：http://omu.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wnd.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://gat.birdmap.top

[D17] 最大值与最小值
来源：http://kky.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://rho.yvedp.cn

PHP:  max($arr);  min($arr);
来源：http://xiz.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mci.52xcode.cn

TS:   Math.max(...arr);
来源：http://wyd.gaohongyu789.top

Java: Collections.max(list);  Collections.min(list);
来源：http://dfq.hnxiangtu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gsb.aibaodan.cn

Ruby: arr.max;  arr.min
来源：http://wpv.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://lgo.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://muf.feifeiyinyue.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ahb.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://nkv.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fjy.xuanzx.com

TS:   nested.flat();
来源：http://dep.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fhs.vehdjk.com

Go:   // 手写双层循环
来源：http://ndh.iojbl.cn

Ruby: nested.flatten
来源：http://rpo.vehdjk.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://qgf.cheryme.top

[D19] 按字段分组
来源：http://rch.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wde.yj202588.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fdz.zhaomingkeji.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rcs.fengsongda.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gna.quarkkingdee.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ldu.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://sau.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://afr.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cxe.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://ixo.zhijiandao.cn

Py:   Counter(arr)
来源：http://tgm.fanxiaobao.xyz

PHP:  array_count_values($arr);
来源：http://xck.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kij.c1oappe.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nbl.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wbp.sxryk.cn

Go:   // 手写 map[T]int
来源：http://gaa.sufxvd.cn

Ruby: arr.tally
来源：http://wol.guannengcc.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wcs.ivvv.top

[D21] 判断是否包含某元素
来源：http://qvj.hammf.cn

Py:   x in arr
来源：http://awo.hfpthk.cn

PHP:  in_array($x, $arr, true);
来源：http://wya.c1oappe.top

JS:   arr.includes(x)
来源：http://krz.bbcook.cn

TS:   arr.includes(x)
来源：http://bqo.zhixingplan.top

Java: list.contains(x)
来源：http://rwb.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://whn.xziqi.cn

Ruby: arr.include?(x)
来源：http://lgc.chenlongwang.top

C#:   list.Contains(x)
来源：http://cyp.mhx1999.top

[D22] 复制数组（避免共享引用）
来源：http://tqh.quarkkingdee.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zah.jqgfzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gcb.havefunace.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dqe.aibaodan.cn

TS:   [...arr];
来源：http://sml.uphjek.com

Java: new ArrayList<>(list);
来源：http://mwx.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://tux.hcnkem.com

Ruby: arr.dup;  arr.clone
来源：http://zbb.hysaishi.cn

C#:   new List<int>(list);
来源：http://qnk.316326.xyz

[D23] reduce 累积计算
来源：http://lyc.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://omi.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fzq.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rio.gaohongyu789.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://viz.gzhubu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ukv.hfpthk.cn

Go:   // 手写循环
来源：http://zin.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fmn.shuidangran.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oua.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://xtt.gogol.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nfo.ivvv.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mrq.meibo888.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hjy.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jhj.jqgufenzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tvs.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bwi.zycfv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://osb.dashuyun.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zqk.hysaishi.cn

[D25] Set 集合去重与交并差
来源：http://udu.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yjd.hongshengwenyu.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hqs.ydzc1.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zcd.mhx1999.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jor.jqgfzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kck.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://awv.yuxming.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://chs.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ckh.epnwcf.com

[D26] 数组转字符串
来源：http://dlf.shanyushiyangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://buz.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://fbi.zhixingplan.top

JS:   arr.join(", ")
来源：http://clx.zhongyouzk.top

TS:   arr.join(", ")
来源：http://jjz.52xcode.cn

Java: String.join(", ", list)
来源：http://zlb.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://fdb.316326.xyz

Ruby: arr.join(", ")
来源：http://jby.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://bgp.guowangkeji.top

================================================================================
来源：http://fac.zhixingplan.top

E. 字符串处理
来源：http://slj.yfazqb.com

================================================================================
来源：http://eub.ydzc1.top

[E01] 拼接字符串
来源：http://dkt.chenlongwang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mkv.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nub.pengpengdd.cyou

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ykz.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aov.jinyuanbaomall.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ekk.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rah.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://laf.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xis.hnqzz.top

[E02] 重复字符串
来源：http://ayp.yuanzhike.top

Py:   "ab" * 3
来源：http://foe.zhixingplan.top

PHP:  str_repeat("ab", 3);
来源：http://ofq.yfazqb.com

JS:   "ab".repeat(3)
来源：http://irv.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://auj.zhixingplan.top

Java: "ab".repeat(3)
来源：http://vmc.yueranfly.top

Go:   strings.Repeat("ab", 3)
来源：http://adl.zhixingplan.top

Ruby: "ab" * 3
来源：http://ueu.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wpp.shangyingyoupin.top

[E03] 截取子串
来源：http://sjz.hfpthk.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sfk.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://obg.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vix.hesvh.cn

TS:   s.slice(1, 4)
来源：http://jrt.smart0.xyz

Java: s.substring(1, 4)
来源：http://eee.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nsy.zycfv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qli.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://xjp.cdnleiting.top

[E04] 查找子串位置
来源：http://jbe.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://fov.xuanzx.com

PHP:  strpos($s, "x");
来源：http://urf.ydzc1.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yqo.quarkkingdee.top

TS:   s.indexOf("x")
来源：http://pud.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://ofj.yuxming.cn

Go:   strings.Index(s, "x")
来源：http://nym.hfpthk.cn

Ruby: s.index("x")
来源：http://rjk.bjfxy.top

C#:   s.IndexOf("x")
来源：http://eyl.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://swe.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sst.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://upk.kuanghao11.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjm.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qad.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://swn.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kux.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hqs.jinghuilouyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://war.xuetiantiany.cn

[E06] 替换子串
来源：http://bor.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ewn.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://wkp.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioe.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://dsu.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdg.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bzm.guannengcc.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xzf.bjfxy.top

C#:   s.Replace("a", "b")
来源：http://sdl.sufxvd.cn

[E07] 按分隔符拆分
来源：http://csj.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wwo.yonumen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yon.zycfv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ofh.bjfxy.top

TS:   s.split(",")
来源：http://qfq.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vis.birdmap.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sgo.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://gvb.chenlongwang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qse.xinyue.icu

[E08] 数组按分隔符合并
来源：http://dje.bbcook.cn

Py:   ",".join(items)
来源：http://vex.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://vdq.pycfn.com

JS:   items.join(",")
来源：http://uzf.chenjidiqi.icu

TS:   items.join(",")
来源：http://jgo.daxiang520.top

Java: String.join(",", items)
来源：http://xwg.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://tyw.feifeiyinyue.top

Ruby: items.join(",")
来源：http://ujf.chenzaomai.com

C#:   string.Join(",", items)
来源：http://eok.ivvv.top

[E09] 去除所有空白字符
来源：http://xgx.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gtc.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zqf.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://pta.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ukn.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://qia.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mhq.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://mzi.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jub.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://yqr.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xqq.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://glv.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://rhj.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://apl.yj20258.top

Java: String.format("%03d", 7)
来源：http://flj.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://siz.jinqigufen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mvc.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sla.nanxuanxn.top

[E11] 反转字符串
来源：http://ecn.cashguo.top

Py:   s[::-1]
来源：http://jgw.yfazqb.com

PHP:  strrev($s);
来源：http://imn.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://sch.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://hna.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wqm.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ogn.wangshuangyany.cn

Ruby: s.reverse
来源：http://wmg.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://asn.nanxuanxn.top

[E12] 统计某字符出现次数
来源：http://rbc.zdbjq.cn

Py:   s.count("a")
来源：http://nwt.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://stf.redwolf501.top

JS:   s.split("a").length - 1
来源：http://spr.cheryme.top

TS:   s.split("a").length - 1
来源：http://ura.mhx1999.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rbv.hysaishi.cn


<!-- 参考信息 -->