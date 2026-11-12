代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tov.nwbrower.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ivy.sxryk.cn

TS:   arr[0]; arr.at(-1);
来源：http://guq.pycfn.com

Java: list.get(0); list.set(0, 9);
来源：http://urg.xinyue.icu

Go:   arr[0]; arr[0] = 9
来源：http://nwy.sufxvd.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://txd.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://deu.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://cnz.birdmap.top

Py:   len(arr)
来源：http://kbr.xuanzx.com

PHP:  count($arr);
来源：http://kop.redwolf501.top

JS:   arr.length
来源：http://ajy.jianghu66.top

TS:   arr.length
来源：http://brf.jinyuanbaomall.cn

Java: list.size();
来源：http://qyw.ppjwa.cn

Go:   len(arr)
来源：http://sms.ywan-chungtsiang.top

Ruby: arr.length; arr.size
来源：http://dlk.xuetiantiany.cn

C#:   list.Count;
来源：http://nfw.iojbl.cn

[D07] 切片 / 取子数组
来源：http://fur.wangdashe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kcv.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cqj.zhixingplan.top

JS:   arr.slice(1, 4);
来源：http://qyy.xylfe.cn

TS:   arr.slice(1, 4);
来源：http://hep.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://vgs.mhx1999.top

Go:   arr[1:4]
来源：http://fci.jinqigfzy.top

Ruby: arr[1, 3]
来源：http://iaj.zdqjudy.top

C#:   list.GetRange(1, 3);
来源：http://fmq.birdmap.top

[D08] 合并两个数组
来源：http://pwx.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://dtd.chenlongwang.top

PHP:  array_merge($a, $b);
来源：http://wcb.haohaochexian.top

JS:   [...a, ...b];  a.concat(b);
来源：http://viu.zdqjudy.top

TS:   [...a, ...b];
来源：http://tlw.chenlongwang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zjx.guowangkeji.top

Go:   append(a, b...)
来源：http://cwt.shuidangran.top

Ruby: a + b;  a.concat(b)
来源：http://sbr.dashuyun.cn

C#:   a.Concat(b).ToList()
来源：http://ano.hcnkem.com

[D09] 排序（升序）
来源：http://zyp.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://uar.chenlongwang.top

PHP:  sort($arr);
来源：http://ltp.smart0.xyz

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://laa.ydzc1.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://yke.quarkkingdee.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gsq.vehdjk.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tyx.guannengcc.top

Ruby: arr.sort
来源：http://psq.chenzaomai.com

C#:   list.Sort();
来源：http://vfi.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://elv.nanxinkj.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rat.hfpthk.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cjb.daxiang520.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://doo.jiagoushi.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blk.andypj.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fmg.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://otd.wangshuangyany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yur.guowangkeji.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bob.xingfuxueyuan.xyz

[D11] 反转数组
来源：http://yqp.zhengqikj.top

Py:   arr[::-1];  arr.reverse()
来源：http://qjg.tianlin.xyz

PHP:  array_reverse($arr);
来源：http://gmf.yuanzhike.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ijc.bjfxy.top

TS:   [...arr].reverse();
来源：http://hzb.yuanzhike.top

Java: Collections.reverse(list);
来源：http://ddy.yvedp.cn

Go:   slices.Reverse(arr)
来源：http://kui.jinqigufen.top

Ruby: arr.reverse
来源：http://egh.guowangkeji.top

C#:   list.Reverse();
来源：http://vrl.tarul.cn

[D12] 查找元素下标
来源：http://srk.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://nig.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zln.yj202588.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xvz.tarul.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qja.jiagoushi.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ifp.zhaomingkeji.xyz

Go:   slices.Index(arr, x)
来源：http://clz.cqqwz.cn

Ruby: arr.index(x)
来源：http://byj.vehdjk.com

C#:   list.IndexOf(x);
来源：http://gbw.pycfn.com

[D13] 过滤（保留满足条件的）
来源：http://vwd.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oot.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nco.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://udy.shzxlz.cn

TS:   arr.filter(x => x > 3)
来源：http://cdv.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://eqs.gotoacloud.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rto.hongshengwenyu.top

Ruby: arr.select { |x| x > 3 }
来源：http://mnv.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rlv.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://aes.andypj.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zfu.zhijiandao.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gpt.meibo888.top

JS:   arr.map(x => x * 2)
来源：http://mey.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://lfs.gzhubu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://wuz.yongpay.top

Go:   // 手写循环
来源：http://ohk.andypj.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://exn.jianghu66.top

C#:   list.Select(x => x * 2).ToList()
来源：http://quk.cucudq.cn

[D15] 去重
来源：http://gqn.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://asd.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://rcj.zdbjq.cn

JS:   [...new Set(arr)]
来源：http://uqu.tarul.cn

TS:   [...new Set(arr)]
来源：http://nai.zhongyouzk.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://djl.fzhhl.top

Go:   // 用 map[T]struct{} 手写
来源：http://cjn.52xcode.cn

Ruby: arr.uniq
来源：http://igh.cdnleiting.top

C#:   list.Distinct().ToList()
来源：http://ckd.c1oappe.top

[D16] 求和与平均值
来源：http://hef.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uba.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://onz.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cav.jqgfzy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eix.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pxq.xinyue.icu

Go:   // 手写循环累加
来源：http://gdx.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kji.yvedp.cn

C#:   list.Sum();  list.Average()
来源：http://vau.jqgufenzy.top

[D17] 最大值与最小值
来源：http://hqs.daria6918.cn

Py:   max(arr);  min(arr)
来源：http://tte.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://uyr.zhaomingkeji.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ulw.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://qix.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://wqh.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lbb.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://tzf.jlsjyb.cn

C#:   list.Max();  list.Min()
来源：http://skm.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://gix.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://chz.ywan-chungtsiang.top

PHP:  array_merge(...$nested);
来源：http://uis.yj20258.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dgf.ctjpmb.com

TS:   nested.flat();
来源：http://ihx.fanxiaobao.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ynn.zhixingplan.top

Go:   // 手写双层循环
来源：http://gbv.gzhubu.top

Ruby: nested.flatten
来源：http://iqq.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qjm.haohaochexian.top

[D19] 按字段分组
来源：http://jbx.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sbr.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dbl.tanke756.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nmc.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ozr.hywenlv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nau.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://nsw.fengsongda.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jpm.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ouy.yj20258.top

[D20] 统计每个元素出现次数
来源：http://kxu.yonumen.top

Py:   Counter(arr)
来源：http://oco.zhongyouzk.top

PHP:  array_count_values($arr);
来源：http://bza.zhongyouzk.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://exg.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://haw.shanyushiyangtech.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://brd.zhongyouzk.top

Go:   // 手写 map[T]int
来源：http://rso.jlsjyb.cn

Ruby: arr.tally
来源：http://bhs.smart0.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fmj.zhengqikj.top

[D21] 判断是否包含某元素
来源：http://qij.andypj.xyz

Py:   x in arr
来源：http://evj.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://vrw.yj20258.top

JS:   arr.includes(x)
来源：http://dng.ctjpmb.com

TS:   arr.includes(x)
来源：http://zig.fehbvm.com

Java: list.contains(x)
来源：http://nhb.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://mrf.zhijiandao.cn

Ruby: arr.include?(x)
来源：http://xvf.yuxming.cn

C#:   list.Contains(x)
来源：http://qsi.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://vwv.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ldi.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gbf.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ydi.pengpengdd.cyou

TS:   [...arr];
来源：http://bok.bbcook.cn

Java: new ArrayList<>(list);
来源：http://mfi.sjlbkw.cn

Go:   copied := append([]int(nil), arr...)
来源：http://buj.guannengcc.top

Ruby: arr.dup;  arr.clone
来源：http://nab.jyoumei.cn

C#:   new List<int>(list);
来源：http://wva.vehdjk.com

[D23] reduce 累积计算
来源：http://vnk.kuanghao11.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yty.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xqg.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gol.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yvx.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://lgp.yanxiufei.cn

Go:   // 手写循环
来源：http://gye.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyu.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cwh.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://cwa.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kqo.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zrw.ctjpmb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://njg.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kpf.wangdashe.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lou.ydjk.org.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nxc.uphjek.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ddv.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rdu.cqqwz.cn

[D25] Set 集合去重与交并差
来源：http://jgb.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qzj.shzxlz.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://usm.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://axb.zhengqikj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tzv.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://niv.xylfe.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pzv.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zjt.pycfn.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://osh.sxryk.cn

[D26] 数组转字符串
来源：http://zqc.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://kpb.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://mlw.nwbrower.top

JS:   arr.join(", ")
来源：http://lfa.cqqwz.cn

TS:   arr.join(", ")
来源：http://noh.nanxuanxn.top

Java: String.join(", ", list)
来源：http://xvu.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://utc.xylfe.cn

Ruby: arr.join(", ")
来源：http://prk.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://cju.zhengqikj.top

================================================================================
来源：http://yht.ivvv.top

E. 字符串处理
来源：http://fco.chenlongwang.top

================================================================================
来源：http://wmi.hywenlv.cn

[E01] 拼接字符串
来源：http://cnx.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://csr.cucudq.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qcm.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tng.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dby.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ert.hnxiangtu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rua.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kbi.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://izx.sysykeji.top

[E02] 重复字符串
来源：http://ihy.kuanghao11.cn

Py:   "ab" * 3
来源：http://bmm.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://rjp.xylfe.cn

JS:   "ab".repeat(3)
来源：http://sxz.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://bxl.xinyue.icu

Java: "ab".repeat(3)
来源：http://jez.ctjpmb.com

Go:   strings.Repeat("ab", 3)
来源：http://azi.zhongyouzk.top

Ruby: "ab" * 3
来源：http://ugy.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ore.uphjek.com

[E03] 截取子串
来源：http://vfe.xziqi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vpx.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jml.fzhhl.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://igy.ctjpmb.com

TS:   s.slice(1, 4)
来源：http://bbx.hnxiangtu.top

Java: s.substring(1, 4)
来源：http://mwi.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ols.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://zgq.mhx1999.top

C#:   s.Substring(1, 3)
来源：http://gcp.xuetiantiany.cn

[E04] 查找子串位置
来源：http://dlv.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://rnm.daxiang520.top

PHP:  strpos($s, "x");
来源：http://gcm.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lbj.shangyingyoupin.top

TS:   s.indexOf("x")
来源：http://tac.0kj1m.cn

Java: s.indexOf("x")
来源：http://vey.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://igl.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://mio.kuanghao11.cn

C#:   s.IndexOf("x")
来源：http://gne.havefunace.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xlc.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bpo.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dxy.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tso.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zqp.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pfi.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ckg.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sxp.tianlin.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pbk.sysykeji.top

[E06] 替换子串
来源：http://tiw.hysaishi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yce.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://pib.yj20258888.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fls.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://otg.snrcjt.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uqq.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bsp.vqdsnc.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gul.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://mgh.tarul.cn

[E07] 按分隔符拆分
来源：http://rby.jqgufenzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://asu.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ywc.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://tnc.jinqigufen.top

TS:   s.split(",")
来源：http://jgz.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://tln.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pxn.316326.xyz

Ruby: s.split(",");  s.split
来源：http://mqk.hysaishi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pif.bjfxy.top

[E08] 数组按分隔符合并
来源：http://lrm.tian-w.cn

Py:   ",".join(items)
来源：http://ysd.yuxming.cn

PHP:  implode(",", $items);
来源：http://nao.epnwcf.com

JS:   items.join(",")
来源：http://ezm.daria6918.cn

TS:   items.join(",")
来源：http://hnb.pengpengdd.cyou

Java: String.join(",", items)
来源：http://imv.cdnleiting.top

Go:   strings.Join(items, ",")
来源：http://cng.zhongyouzk.top

Ruby: items.join(",")
来源：http://lsd.yj20258.top

C#:   string.Join(",", items)
来源：http://dyn.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://kbq.shuidangran.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nhm.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ufv.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://nlg.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://uqc.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://atp.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wuf.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://two.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xfk.9152youxi.cn

[E10] 左侧补零 / 定长填充
来源：http://ttk.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qwn.zhaomingkeji.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jzi.sweek.top

JS:   "7".padStart(3, "0")
来源：http://zeb.zhijiandao.cn

TS:   "7".padStart(3, "0")
来源：http://plx.c1oappe.top

Java: String.format("%03d", 7)
来源：http://qzy.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vpj.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://doe.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://alc.yj20258.top

[E11] 反转字符串
来源：http://fmb.ivvv.top

Py:   s[::-1]
来源：http://hub.smart0.xyz

PHP:  strrev($s);
来源：http://dkb.yangfankeji.com

JS:   [...s].reverse().join("")
来源：http://pxp.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://kge.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nvn.pycfn.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://oly.pycfn.com

Ruby: s.reverse
来源：http://odz.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://gqv.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://azg.uphjek.com

Py:   s.count("a")
来源：http://ewd.zhoulong.xyz


<!-- 参考信息 -->