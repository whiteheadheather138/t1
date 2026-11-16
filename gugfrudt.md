代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yvc.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qro.0kj1m.cn

TS:   arr[0]; arr.at(-1);
来源：http://spj.zhixingplan.top

Java: list.get(0); list.set(0, 9);
来源：http://ywn.gzhubu.top

Go:   arr[0]; arr[0] = 9
来源：http://tjo.yj20258.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dvw.yueranfly.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://htu.meibo888.top

[D06] 数组长度
来源：http://xns.tian-w.cn

Py:   len(arr)
来源：http://bzr.zhoulong.xyz

PHP:  count($arr);
来源：http://cvh.yfazqb.com

JS:   arr.length
来源：http://uhg.zhiwuduotai.top

TS:   arr.length
来源：http://xdx.fehbvm.com

Java: list.size();
来源：http://tis.zhiwuduotai.top

Go:   len(arr)
来源：http://fmg.zhongyouzk.top

Ruby: arr.length; arr.size
来源：http://gve.jinqigufen.top

C#:   list.Count;
来源：http://dls.hcnkem.com

[D07] 切片 / 取子数组
来源：http://nyh.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://njm.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://sin.havefunace.top

JS:   arr.slice(1, 4);
来源：http://cyv.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://hds.zhongyouzk.top

Java: list.subList(1, 4);
来源：http://xlu.tian-w.cn

Go:   arr[1:4]
来源：http://znp.cdnleiting.top

Ruby: arr[1, 3]
来源：http://rjj.hesvh.cn

C#:   list.GetRange(1, 3);
来源：http://ezn.shzxlz.cn

[D08] 合并两个数组
来源：http://lsu.nwbrower.top

Py:   a + b;  a.extend(b)
来源：http://yfw.hnxiangtu.top

PHP:  array_merge($a, $b);
来源：http://sri.dashuyun.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kuq.andypj.xyz

TS:   [...a, ...b];
来源：http://qdt.jianghu66.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bgr.zdqjudy.top

Go:   append(a, b...)
来源：http://vxj.zhengqikj.top

Ruby: a + b;  a.concat(b)
来源：http://fib.yvedp.cn

C#:   a.Concat(b).ToList()
来源：http://kat.birdmap.top

[D09] 排序（升序）
来源：http://smx.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lfr.bbcook.cn

PHP:  sort($arr);
来源：http://hzu.zhengqikj.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qob.hnqzz.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://vvb.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://lwb.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://atz.mhx1999.top

Ruby: arr.sort
来源：http://ryj.fzhhl.top

C#:   list.Sort();
来源：http://eyz.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uaj.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://unu.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fuo.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://acx.zdbjq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fzk.jinyuanbaomall.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zea.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kdb.mhx1999.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lwj.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://txi.hnqzz.top

[D11] 反转数组
来源：http://vrd.yangfankeji.com

Py:   arr[::-1];  arr.reverse()
来源：http://eni.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://rfz.yongpay.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oag.zhiwuduotai.top

TS:   [...arr].reverse();
来源：http://puk.52xcode.cn

Java: Collections.reverse(list);
来源：http://xrv.chenjidiqi.icu

Go:   slices.Reverse(arr)
来源：http://tcd.aizwys.cn

Ruby: arr.reverse
来源：http://mye.tian-w.cn

C#:   list.Reverse();
来源：http://eoj.aizwys.cn

[D12] 查找元素下标
来源：http://mwv.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://qre.snrcjt.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iyz.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jrz.ppjwa.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mow.cheryme.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mdy.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://nlp.tarul.cn

Ruby: arr.index(x)
来源：http://lgt.chenzaomai.com

C#:   list.IndexOf(x);
来源：http://slo.haohaochexian.top

[D13] 过滤（保留满足条件的）
来源：http://uue.zycfv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wiq.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nzu.chenzaomai.com

JS:   arr.filter(x => x > 3)
来源：http://diq.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://alb.daria6918.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cto.c1oappe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mky.vehdjk.com

Ruby: arr.select { |x| x > 3 }
来源：http://ovf.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://viu.smart0.xyz

[D14] 映射转换（每个元素变形）
来源：http://wum.xziqi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ukn.xuanzx.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qqs.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://euh.daxiang520.top

TS:   arr.map(x => x * 2)
来源：http://zrp.hammf.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gwp.fzhhl.top

Go:   // 手写循环
来源：http://axe.daxiang520.top

Ruby: arr.map { |x| x * 2 }
来源：http://lwf.jinghuilouyu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zpx.andypj.xyz

[D15] 去重
来源：http://dix.cucudq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://udj.hnxiangtu.top

PHP:  array_unique($arr);
来源：http://dqf.shanyushiyangtech.top

JS:   [...new Set(arr)]
来源：http://dzk.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://hxm.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ytf.nanxuanxn.top

Go:   // 用 map[T]struct{} 手写
来源：http://gzp.chenlongwang.top

Ruby: arr.uniq
来源：http://vau.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://fme.haohaochexian.top

[D16] 求和与平均值
来源：http://zjq.vqdsnc.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kbz.smart0.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qck.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sjt.hysaishi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://god.ehwqpu.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rxb.zhengqikj.top

Go:   // 手写循环累加
来源：http://mgb.sjlbkw.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nrt.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://vfe.andypj.xyz

[D17] 最大值与最小值
来源：http://awf.cheryme.top

Py:   max(arr);  min(arr)
来源：http://ogp.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://znz.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fld.aizwys.cn

TS:   Math.max(...arr);
来源：http://uzo.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://akf.ivvv.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ggo.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://esb.yj202588.top

C#:   list.Max();  list.Min()
来源：http://ozp.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://lke.gaohongyu789.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kko.tanke756.top

PHP:  array_merge(...$nested);
来源：http://yhz.ydjk.org.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rng.xuanzx.com

TS:   nested.flat();
来源：http://rwi.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dbg.meibo888.top

Go:   // 手写双层循环
来源：http://krb.yvedp.cn

Ruby: nested.flatten
来源：http://krk.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hdh.yfazqb.com

[D19] 按字段分组
来源：http://jdn.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://prd.316326.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lpu.tian-w.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cwm.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vcz.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wvx.yonumen.top

Go:   // 手写 map[string][]T
来源：http://jkw.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gnr.quarkkingdee.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ipd.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://kvd.ydjk.org.cn

Py:   Counter(arr)
来源：http://vcj.fengsongda.top

PHP:  array_count_values($arr);
来源：http://hah.tarul.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nkg.yuxming.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mfi.xingfuxueyuan.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zxq.jqgfzy.top

Go:   // 手写 map[T]int
来源：http://sng.cashguo.top

Ruby: arr.tally
来源：http://lin.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pmo.fehbvm.com

[D21] 判断是否包含某元素
来源：http://kbz.sysykeji.top

Py:   x in arr
来源：http://zkk.vehdjk.com

PHP:  in_array($x, $arr, true);
来源：http://txw.vehdjk.com

JS:   arr.includes(x)
来源：http://aac.daxiang520.top

TS:   arr.includes(x)
来源：http://xzg.daxiang520.top

Java: list.contains(x)
来源：http://rya.gzhubu.top

Go:   slices.Contains(arr, x)
来源：http://eqi.jinqigufen.top

Ruby: arr.include?(x)
来源：http://wvr.hcnkem.com

C#:   list.Contains(x)
来源：http://xko.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://nst.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mwu.jqgufenzy.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ufp.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nnx.hcnkem.com

TS:   [...arr];
来源：http://jda.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://jcv.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbi.c1oappe.top

Ruby: arr.dup;  arr.clone
来源：http://mkz.ppjwa.cn

C#:   new List<int>(list);
来源：http://lnk.zdbjq.cn

[D23] reduce 累积计算
来源：http://oya.ybcxt.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uvs.chenlongwang.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gah.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vvs.zhixingplan.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jec.fengsongda.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://pfg.sysykeji.top

Go:   // 手写循环
来源：http://cxd.meibo888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xad.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rcg.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://sdv.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yjq.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://olg.jqgufenzy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pgp.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jol.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rvw.zdbjq.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wcm.xziqi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cyz.shuidangran.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qro.316326.xyz

[D25] Set 集合去重与交并差
来源：http://gyp.sxryk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yht.fzhhl.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hbk.dianchejie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jqq.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vcl.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://noa.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pln.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zdw.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nuk.smart0.xyz

[D26] 数组转字符串
来源：http://rhz.cucudq.cn

Py:   ", ".join(map(str, arr))
来源：http://lvn.52xcode.cn

PHP:  implode(", ", $arr);
来源：http://ldx.guannengcc.top

JS:   arr.join(", ")
来源：http://tra.aizwys.cn

TS:   arr.join(", ")
来源：http://ghm.sjlbkw.cn

Java: String.join(", ", list)
来源：http://adx.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://gyv.jqgfzy.top

Ruby: arr.join(", ")
来源：http://qwi.daxiang520.top

C#:   string.Join(", ", list)
来源：http://juy.ctjpmb.com

================================================================================
来源：http://jac.epnwcf.com

E. 字符串处理
来源：http://dsv.daxiang520.top

================================================================================
来源：http://pwo.jlsjyb.cn

[E01] 拼接字符串
来源：http://pzh.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xyx.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yye.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://alr.jqgfzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://thk.meibo888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqt.nanxinkj.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yto.cucudq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dtl.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bkl.ydzc1.top

[E02] 重复字符串
来源：http://kqk.zhengqikj.top

Py:   "ab" * 3
来源：http://lqv.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://pws.ydzc1.top

JS:   "ab".repeat(3)
来源：http://jyk.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://aqt.dianchejie.cn

Java: "ab".repeat(3)
来源：http://pea.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://hcc.daxiang520.top

Ruby: "ab" * 3
来源：http://hjz.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://npd.smart0.xyz

[E03] 截取子串
来源：http://zeh.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lxp.nanxuanxn.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yca.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfq.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://bgr.aibaodan.cn

Java: s.substring(1, 4)
来源：http://dla.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xfq.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://ngz.uphjek.com

C#:   s.Substring(1, 3)
来源：http://tuq.tianlin.xyz

[E04] 查找子串位置
来源：http://ylu.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://njv.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://pdg.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://sag.hysaishi.cn

TS:   s.indexOf("x")
来源：http://aco.bjfxy.top

Java: s.indexOf("x")
来源：http://nli.uphjek.com

Go:   strings.Index(s, "x")
来源：http://ios.bjfxy.top

Ruby: s.index("x")
来源：http://ruk.52xcode.cn

C#:   s.IndexOf("x")
来源：http://lkf.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://drp.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fnw.tian-w.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vlu.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qny.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://uhw.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pms.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jgt.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jbb.zhiwuduotai.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ifu.zhijiandao.cn

[E06] 替换子串
来源：http://yts.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zqu.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://gjd.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vft.xziqi.cn

TS:   s.replaceAll("a", "b")
来源：http://tse.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qtn.yangfankeji.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mkj.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bhz.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://pzx.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://gmp.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://key.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nfq.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://obs.sufxvd.cn

TS:   s.split(",")
来源：http://mjb.jqgufenzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://djh.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iop.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://uot.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ova.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://dym.52xcode.cn

Py:   ",".join(items)
来源：http://qpj.fzhhl.top

PHP:  implode(",", $items);
来源：http://ssp.cqqwz.cn

JS:   items.join(",")
来源：http://abr.cashguo.top

TS:   items.join(",")
来源：http://uti.iojbl.cn

Java: String.join(",", items)
来源：http://cxj.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://ofx.zhongyouzk.top

Ruby: items.join(",")
来源：http://vko.jinqigufen.top

C#:   string.Join(",", items)
来源：http://oaf.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://ubv.haohaochexian.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oig.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://awl.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://yba.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://eja.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://pve.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xzi.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rsr.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ilc.chenlongwang.top

[E10] 左侧补零 / 定长填充
来源：http://zgp.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mvy.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lwc.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://bbo.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://adr.fktsv.cn

Java: String.format("%03d", 7)
来源：http://wzl.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qic.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fqx.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rir.316326.xyz

[E11] 反转字符串
来源：http://mys.yj20258888.top

Py:   s[::-1]
来源：http://fjv.ydjk.org.cn

PHP:  strrev($s);
来源：http://lpx.bbcook.cn

JS:   [...s].reverse().join("")
来源：http://aet.dashuyun.cn

TS:   [...s].reverse().join("")
来源：http://tje.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rkg.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzk.tarul.cn

Ruby: s.reverse
来源：http://iqh.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rcb.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://lzd.feifeiyinyue.top

Py:   s.count("a")
来源：http://duj.chenlongwang.top


<!-- 参考信息 -->