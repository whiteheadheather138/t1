代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://erg.zhixingplan.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wlq.sweek.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bts.zhijiandao.cn

[D06] 数组长度
来源：http://ojd.tarul.cn

Py:   len(arr)
来源：http://npw.dianchejie.cn

PHP:  count($arr);
来源：http://fhs.gogol.net.cn

JS:   arr.length
来源：http://ldn.0kj1m.cn

TS:   arr.length
来源：http://jbi.gzhubu.top

Java: list.size();
来源：http://pau.hcnkem.com

Go:   len(arr)
来源：http://znr.vehdjk.com

Ruby: arr.length; arr.size
来源：http://qsn.c1oappe.top

C#:   list.Count;
来源：http://rqb.zdbjq.cn

[D07] 切片 / 取子数组
来源：http://bom.svipenyu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://coj.xuanzx.com

PHP:  array_slice($arr, 1, 3);
来源：http://nnd.gaohongyu789.top

JS:   arr.slice(1, 4);
来源：http://kpz.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://hfv.iojbl.cn

Java: list.subList(1, 4);
来源：http://eac.wangdashe.top

Go:   arr[1:4]
来源：http://exd.kuanghao11.cn

Ruby: arr[1, 3]
来源：http://mvc.cqqwz.cn

C#:   list.GetRange(1, 3);
来源：http://sbb.xziqi.cn

[D08] 合并两个数组
来源：http://bhn.shzxlz.cn

Py:   a + b;  a.extend(b)
来源：http://sbp.ywan-chungtsiang.top

PHP:  array_merge($a, $b);
来源：http://ylu.tian-w.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://xce.yangfankeji.com

TS:   [...a, ...b];
来源：http://axn.sysykeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wol.svipenyu.cn

Go:   append(a, b...)
来源：http://uaf.tianlin.xyz

Ruby: a + b;  a.concat(b)
来源：http://bzt.cqqwz.cn

C#:   a.Concat(b).ToList()
来源：http://fbn.hammf.cn

[D09] 排序（升序）
来源：http://rcz.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://uzg.ivvv.top

PHP:  sort($arr);
来源：http://eqd.cqqwz.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wop.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qmc.zhengqikj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ayq.zhoulong.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rur.smart0.xyz

Ruby: arr.sort
来源：http://uki.shzxlz.cn

C#:   list.Sort();
来源：http://cvx.feifeiyinyue.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://nam.pycfn.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vlo.zycfv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wqd.dashuyun.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pns.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pyb.daria6918.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aso.hongshengwenyu.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://awk.zycfv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yzp.nanxinkj.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://suk.fehbvm.com

[D11] 反转数组
来源：http://yre.snrcjt.cn

Py:   arr[::-1];  arr.reverse()
来源：http://btk.yj20258888.top

PHP:  array_reverse($arr);
来源：http://cni.sjlbkw.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uhf.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://wer.chenzaomai.com

Java: Collections.reverse(list);
来源：http://udf.daxiang520.top

Go:   slices.Reverse(arr)
来源：http://eet.chenjidiqi.icu

Ruby: arr.reverse
来源：http://fme.aizwys.cn

C#:   list.Reverse();
来源：http://rhm.hongshengwenyu.top

[D12] 查找元素下标
来源：http://cbj.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://xzd.shanyushiyangtech.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bjq.chenzaomai.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mis.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://edq.fehbvm.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cde.yonumen.top

Go:   slices.Index(arr, x)
来源：http://epw.shangyingyoupin.top

Ruby: arr.index(x)
来源：http://wkl.bjfxy.top

C#:   list.IndexOf(x);
来源：http://fxi.zhijiandao.cn

[D13] 过滤（保留满足条件的）
来源：http://pvc.hnxiangtu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cme.xingfuxueyuan.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sat.shanyushiyangtech.top

JS:   arr.filter(x => x > 3)
来源：http://qnw.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://kpe.shzxlz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xzt.sufxvd.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ahx.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://nhv.zhoulong.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://tvs.cheryme.top

[D14] 映射转换（每个元素变形）
来源：http://bnx.yfazqb.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cvl.andypj.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pez.yangfankeji.com

JS:   arr.map(x => x * 2)
来源：http://cit.ehwqpu.com

TS:   arr.map(x => x * 2)
来源：http://jlm.vehdjk.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://mnq.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://xwt.cqqwz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vhz.aibaodan.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ygr.ppjwa.cn

[D15] 去重
来源：http://rea.chenzaomai.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wjo.tarul.cn

PHP:  array_unique($arr);
来源：http://ioj.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://mql.yj202588.top

TS:   [...new Set(arr)]
来源：http://cjz.tarul.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ced.ctjpmb.com

Go:   // 用 map[T]struct{} 手写
来源：http://iod.shangyingyoupin.top

Ruby: arr.uniq
来源：http://oqe.aibaodan.cn

C#:   list.Distinct().ToList()
来源：http://hkm.kuanghao11.cn

[D16] 求和与平均值
来源：http://bil.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ayh.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://epl.vehdjk.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dfn.cucudq.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://syj.redwolf501.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://brr.sysykeji.top

Go:   // 手写循环累加
来源：http://yrc.jinghuilouyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lyb.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://ldq.nwbrower.top

[D17] 最大值与最小值
来源：http://nat.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://fhx.cqqwz.cn

PHP:  max($arr);  min($arr);
来源：http://xtm.smart0.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://luu.bjfxy.top

TS:   Math.max(...arr);
来源：http://kzg.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nav.jinqigfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rcm.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://jpw.ydzc1.top

C#:   list.Max();  list.Min()
来源：http://rdl.shzxlz.cn

[D18] 扁平化嵌套数组
来源：http://bmn.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://djx.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://asg.guannengcc.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qrk.shanyushiyangkeji.top

TS:   nested.flat();
来源：http://ccg.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wgn.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://wqh.redwolf501.top

Ruby: nested.flatten
来源：http://wee.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ohe.quarkkingdee.top

[D19] 按字段分组
来源：http://zcf.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://bmy.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zkb.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uyn.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hcf.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lrw.birdmap.top

Go:   // 手写 map[string][]T
来源：http://csh.pengpengdd.cyou

Ruby: arr.group_by { |x| x[:type] }
来源：http://zas.yfazqb.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hez.9152youxi.cn

[D20] 统计每个元素出现次数
来源：http://aph.c1oappe.top

Py:   Counter(arr)
来源：http://uxb.jinqigufen.top

PHP:  array_count_values($arr);
来源：http://qdv.jqgufenzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dft.tian-w.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fdh.xziqi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pia.gzhubu.top

Go:   // 手写 map[T]int
来源：http://obo.fehbvm.com

Ruby: arr.tally
来源：http://oku.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tpn.vqdsnc.cn

[D21] 判断是否包含某元素
来源：http://xlb.zdqjudy.top

Py:   x in arr
来源：http://bpj.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://edu.9152youxi.cn

JS:   arr.includes(x)
来源：http://omt.dashuyun.cn

TS:   arr.includes(x)
来源：http://ofi.c1oappe.top

Java: list.contains(x)
来源：http://apl.tian-w.cn

Go:   slices.Contains(arr, x)
来源：http://hll.vehdjk.com

Ruby: arr.include?(x)
来源：http://noa.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://qdu.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://vgg.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gwc.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mgq.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wdd.xinyue.icu

TS:   [...arr];
来源：http://euj.ctjpmb.com

Java: new ArrayList<>(list);
来源：http://nns.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fwb.gogol.net.cn

Ruby: arr.dup;  arr.clone
来源：http://mti.hnqzz.top

C#:   new List<int>(list);
来源：http://nno.jqgufenzy.top

[D23] reduce 累积计算
来源：http://dkf.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bmo.hesvh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qeu.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ypp.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jer.shuidangran.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://aog.redwolf501.top

Go:   // 手写循环
来源：http://xjb.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hsc.shanyushiyangtech.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lcc.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://ros.andypj.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://knc.yj20258.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzu.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kxm.xuetiantiany.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vhz.chenjidiqi.icu

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ekf.52xcode.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://itb.daxiang520.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qjm.chenzaomai.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cbm.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://coc.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bcd.zhoulong.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xuk.sxryk.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xef.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yhk.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ksi.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rws.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gcr.yvedp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://obi.zdbjq.cn

[D26] 数组转字符串
来源：http://fll.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://jdc.pycfn.com

PHP:  implode(", ", $arr);
来源：http://hxq.tarul.cn

JS:   arr.join(", ")
来源：http://ngr.aibaodan.cn

TS:   arr.join(", ")
来源：http://zeo.nanxuanxn.top

Java: String.join(", ", list)
来源：http://ect.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://rsq.hammf.cn

Ruby: arr.join(", ")
来源：http://cyb.birdmap.top

C#:   string.Join(", ", list)
来源：http://bbs.hfpthk.cn

================================================================================
来源：http://nme.yangfankeji.com

E. 字符串处理
来源：http://yld.sjlbkw.cn

================================================================================
来源：http://xfs.hesvh.cn

[E01] 拼接字符串
来源：http://xxm.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rly.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://muk.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kwi.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vsd.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vsz.gotoacloud.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mdz.zhaomingkeji.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wws.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nmd.feifeiyinyue.top

[E02] 重复字符串
来源：http://lez.tian-w.cn

Py:   "ab" * 3
来源：http://hpo.shanyushiyangtech.top

PHP:  str_repeat("ab", 3);
来源：http://som.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://hsy.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://acq.yuxming.cn

Java: "ab".repeat(3)
来源：http://lem.havefunace.top

Go:   strings.Repeat("ab", 3)
来源：http://eeq.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://frt.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://coh.yongpay.top

[E03] 截取子串
来源：http://epk.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://txm.tarul.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://toh.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://irw.xuanzx.com

TS:   s.slice(1, 4)
来源：http://pvy.0kj1m.cn

Java: s.substring(1, 4)
来源：http://lsj.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bqm.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://jka.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://czv.gaohongyu789.top

[E04] 查找子串位置
来源：http://vvj.jinqigufen.top

Py:   s.find("x");  s.index("x")
来源：http://pdd.xylfe.cn

PHP:  strpos($s, "x");
来源：http://rer.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xaq.vehdjk.com

TS:   s.indexOf("x")
来源：http://mfw.jqgfzy.top

Java: s.indexOf("x")
来源：http://chv.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://wfv.jqgfzy.top

Ruby: s.index("x")
来源：http://knx.ydjk.org.cn

C#:   s.IndexOf("x")
来源：http://wjq.fanxiaobao.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://dsy.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zoc.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jwr.jianghu66.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppl.cheryme.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dal.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://snz.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qht.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hhh.cdnleiting.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rqv.nanxinkj.top

[E06] 替换子串
来源：http://wbl.jinghuilouyu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jas.andypj.xyz

PHP:  str_replace("a", "b", $s);
来源：http://zak.sweek.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqr.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://ddj.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kas.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://itj.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wmt.316326.xyz

C#:   s.Replace("a", "b")
来源：http://agm.c1oappe.top

[E07] 按分隔符拆分
来源：http://yqq.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zka.52xcode.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oyw.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://uxm.nanxuanxn.top

TS:   s.split(",")
来源：http://odn.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://apb.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ncd.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://lfk.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fjd.52xcode.cn

[E08] 数组按分隔符合并
来源：http://tfz.wangdashe.top

Py:   ",".join(items)
来源：http://jre.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://ack.yangfankeji.com

JS:   items.join(",")
来源：http://zay.nwbrower.top

TS:   items.join(",")
来源：http://rcf.tanke756.top

Java: String.join(",", items)
来源：http://hrg.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://noy.xuetiantiany.cn

Ruby: items.join(",")
来源：http://vpx.uphjek.com

C#:   string.Join(",", items)
来源：http://fng.cheryme.top

[E09] 去除所有空白字符
来源：http://qlv.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nky.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://keq.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://irn.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://apz.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://qiz.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vxu.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://qve.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ioa.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://iyn.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://syp.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wqj.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://dww.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://bty.shuidangran.top

Java: String.format("%03d", 7)
来源：http://gat.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jjz.jinqigfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fuq.guowangkeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pcb.wangdashe.top

[E11] 反转字符串
来源：http://vom.dashuyun.cn

Py:   s[::-1]
来源：http://utm.shangyingyoupin.top

PHP:  strrev($s);
来源：http://qfd.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://yxh.hesvh.cn

TS:   [...s].reverse().join("")
来源：http://hfs.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wjs.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://dry.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://tlr.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://gdd.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://lor.gaohongyu789.top

Py:   s.count("a")
来源：http://emn.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://yxq.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://mcs.epnwcf.com

TS:   s.split("a").length - 1
来源：http://aqc.jinqigfzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jrc.zhongyouzk.top


<!-- 参考信息 -->