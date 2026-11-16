代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ipr.bjfxy.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ngf.zdqjudy.top

[D05] 访问与修改元素
来源：http://vsr.jinyuanbaomall.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://obo.guannengcc.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vky.wangdashe.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://syr.xylfe.cn

TS:   arr[0]; arr.at(-1);
来源：http://svc.wangdashe.top

Java: list.get(0); list.set(0, 9);
来源：http://oqb.aibaodan.cn

Go:   arr[0]; arr[0] = 9
来源：http://dak.hywenlv.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dky.xuanzx.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dhj.sufxvd.cn

[D06] 数组长度
来源：http://btj.cheryme.top

Py:   len(arr)
来源：http://zhi.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://pjo.hfpthk.cn

JS:   arr.length
来源：http://diy.jlsjyb.cn

TS:   arr.length
来源：http://gdb.xuanzx.com

Java: list.size();
来源：http://btg.ydzc1.top

Go:   len(arr)
来源：http://zye.xuanzx.com

Ruby: arr.length; arr.size
来源：http://vwm.zdqjudy.top

C#:   list.Count;
来源：http://elz.uphjek.com

[D07] 切片 / 取子数组
来源：http://nab.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ept.sufxvd.cn

PHP:  array_slice($arr, 1, 3);
来源：http://srn.zhoulong.xyz

JS:   arr.slice(1, 4);
来源：http://ela.vehdjk.com

TS:   arr.slice(1, 4);
来源：http://qki.yueranfly.top

Java: list.subList(1, 4);
来源：http://apu.sysykeji.top

Go:   arr[1:4]
来源：http://dnn.gogol.net.cn

Ruby: arr[1, 3]
来源：http://meu.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://dng.fzhhl.top

[D08] 合并两个数组
来源：http://rgn.nanxuanxn.top

Py:   a + b;  a.extend(b)
来源：http://ytu.zdbjq.cn

PHP:  array_merge($a, $b);
来源：http://cjq.yj20258888.top

JS:   [...a, ...b];  a.concat(b);
来源：http://okh.iojbl.cn

TS:   [...a, ...b];
来源：http://hgi.316326.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ypi.xinyue.icu

Go:   append(a, b...)
来源：http://pzc.jinyuanbaomall.cn

Ruby: a + b;  a.concat(b)
来源：http://pue.shanyushiyangtech.top

C#:   a.Concat(b).ToList()
来源：http://jpb.hcnkem.com

[D09] 排序（升序）
来源：http://nrn.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://kvf.zdbjq.cn

PHP:  sort($arr);
来源：http://zlm.yj20258.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tpz.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://cgk.xuetiantiany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ctw.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rfj.tanke756.top

Ruby: arr.sort
来源：http://ydi.zhongyouzk.top

C#:   list.Sort();
来源：http://tzl.shuidangran.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://wqu.snrcjt.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://grs.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kuz.fktsv.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ihs.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wdl.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fun.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ufv.meibo888.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wtt.hfpthk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baa.zhoulong.xyz

[D11] 反转数组
来源：http://ozn.hammf.cn

Py:   arr[::-1];  arr.reverse()
来源：http://njo.xinyue.icu

PHP:  array_reverse($arr);
来源：http://xkj.hesvh.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gms.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://qsc.gzhubu.top

Java: Collections.reverse(list);
来源：http://xmh.kuanghao11.cn

Go:   slices.Reverse(arr)
来源：http://kxw.hywenlv.cn

Ruby: arr.reverse
来源：http://peh.ydjk.org.cn

C#:   list.Reverse();
来源：http://wga.dashuyun.cn

[D12] 查找元素下标
来源：http://rbe.yanxiufei.cn

Py:   arr.index(x);  x in arr
来源：http://zmo.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kxt.meibo888.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dbe.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://scu.gotoacloud.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kzb.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://nrp.sxryk.cn

Ruby: arr.index(x)
来源：http://syc.zhijiandao.cn

C#:   list.IndexOf(x);
来源：http://khn.cqqwz.cn

[D13] 过滤（保留满足条件的）
来源：http://kdk.yongpay.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cpt.uphjek.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://znw.hysaishi.cn

JS:   arr.filter(x => x > 3)
来源：http://qid.fengsongda.top

TS:   arr.filter(x => x > 3)
来源：http://nqv.redwolf501.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://peu.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vqg.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qud.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://evt.jiagoushi.top

[D14] 映射转换（每个元素变形）
来源：http://mlz.chenlongwang.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cdx.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zjk.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://csa.zycfv.cn

TS:   arr.map(x => x * 2)
来源：http://gsl.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ggk.zhengqikj.top

Go:   // 手写循环
来源：http://rom.fanxiaobao.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ucu.zhoulong.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://sin.jinghuilouyu.cn

[D15] 去重
来源：http://jgp.jlsjyb.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ygn.chenzaomai.com

PHP:  array_unique($arr);
来源：http://gcm.snrcjt.cn

JS:   [...new Set(arr)]
来源：http://iir.jinyuanbaomall.cn

TS:   [...new Set(arr)]
来源：http://rpu.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mbs.mhx1999.top

Go:   // 用 map[T]struct{} 手写
来源：http://gnq.cheryme.top

Ruby: arr.uniq
来源：http://fgy.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://wit.yj20258.top

[D16] 求和与平均值
来源：http://ssj.xylfe.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bpz.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nsa.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dyq.cashguo.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bqt.9152youxi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hco.birdmap.top

Go:   // 手写循环累加
来源：http://hmb.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lmo.yuanzhike.top

C#:   list.Sum();  list.Average()
来源：http://aqa.zdqjudy.top

[D17] 最大值与最小值
来源：http://ejw.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://bmu.jianghu66.top

PHP:  max($arr);  min($arr);
来源：http://ldk.xziqi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uma.c1oappe.top

TS:   Math.max(...arr);
来源：http://uju.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://imi.hongshengwenyu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zvf.cashguo.top

Ruby: arr.max;  arr.min
来源：http://ppn.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://lgb.sysykeji.top

[D18] 扁平化嵌套数组
来源：http://noa.guowangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ftx.shuidangran.top

PHP:  array_merge(...$nested);
来源：http://svi.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nlv.tian-w.cn

TS:   nested.flat();
来源：http://csb.gaohongyu789.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://suu.bjfxy.top

Go:   // 手写双层循环
来源：http://aad.hnqzz.top

Ruby: nested.flatten
来源：http://lid.jinqigufen.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cdt.tarul.cn

[D19] 按字段分组
来源：http://skv.yj20258888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://lzm.uphjek.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kls.hesvh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jft.havefunace.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://dcc.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xun.aibaodan.cn

Go:   // 手写 map[string][]T
来源：http://bgr.aizwys.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://lvo.wangshuangyany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rtn.dianchejie.cn

[D20] 统计每个元素出现次数
来源：http://yhe.yonumen.top

Py:   Counter(arr)
来源：http://vbc.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://xtp.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jzf.sjlbkw.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ebp.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vcr.52xcode.cn

Go:   // 手写 map[T]int
来源：http://ntp.sweek.top

Ruby: arr.tally
来源：http://xiv.ywan-chungtsiang.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dat.ydjk.org.cn

[D21] 判断是否包含某元素
来源：http://ihw.kuanghao11.cn

Py:   x in arr
来源：http://wwt.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://brg.sxryk.cn

JS:   arr.includes(x)
来源：http://lys.sxryk.cn

TS:   arr.includes(x)
来源：http://lya.xuetiantiany.cn

Java: list.contains(x)
来源：http://kjv.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://zuv.jqgufenzy.top

Ruby: arr.include?(x)
来源：http://zpo.yanxiufei.cn

C#:   list.Contains(x)
来源：http://kpw.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://fht.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ili.52xcode.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vzl.fktsv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kfb.zhijiandao.cn

TS:   [...arr];
来源：http://ggk.bjfxy.top

Java: new ArrayList<>(list);
来源：http://irf.fzhhl.top

Go:   copied := append([]int(nil), arr...)
来源：http://ypv.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://aoy.kuanghao11.cn

C#:   new List<int>(list);
来源：http://aax.xinyue.icu

[D23] reduce 累积计算
来源：http://szg.xylfe.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mct.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yle.fengsongda.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mwj.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogi.gaohongyu789.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wle.zhixingplan.top

Go:   // 手写循环
来源：http://udf.aizwys.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zhf.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hgj.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://iie.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vge.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://glf.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ivv.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tjz.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sfw.316326.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://msm.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://afr.ivvv.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fch.vqdsnc.cn

[D25] Set 集合去重与交并差
来源：http://esu.zdbjq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fat.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pnc.52xcode.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ktr.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ghs.vehdjk.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qhl.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vzl.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vfh.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bwx.feifeiyinyue.top

[D26] 数组转字符串
来源：http://owl.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://bry.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://ern.jianghu66.top

JS:   arr.join(", ")
来源：http://fuq.yuxming.cn

TS:   arr.join(", ")
来源：http://ppb.yonumen.top

Java: String.join(", ", list)
来源：http://nbx.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://nyx.sxryk.cn

Ruby: arr.join(", ")
来源：http://kyk.jyoumei.cn

C#:   string.Join(", ", list)
来源：http://gak.zhiwuduotai.top

================================================================================
来源：http://uqf.meibo888.top

E. 字符串处理
来源：http://hbq.jinyuanbaomall.cn

================================================================================
来源：http://cxj.zhixingplan.top

[E01] 拼接字符串
来源：http://tey.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ice.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yxs.tanke756.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jbe.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://btz.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hwn.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ugt.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cdw.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://owr.gotoacloud.top

[E02] 重复字符串
来源：http://uux.feifeiyinyue.top

Py:   "ab" * 3
来源：http://ssv.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://jpy.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://qlz.pycfn.com

TS:   "ab".repeat(3)
来源：http://tga.yuanzhike.top

Java: "ab".repeat(3)
来源：http://tbp.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://ahz.uphjek.com

Ruby: "ab" * 3
来源：http://wzq.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mof.fengsongda.top

[E03] 截取子串
来源：http://vke.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://flc.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ylz.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wvo.fzhhl.top

TS:   s.slice(1, 4)
来源：http://wiz.gzhubu.top

Java: s.substring(1, 4)
来源：http://ddk.yuxming.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ltj.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://hnj.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://ntz.zhongyouzk.top

[E04] 查找子串位置
来源：http://lxd.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://ktj.yongpay.top

PHP:  strpos($s, "x");
来源：http://hmo.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jvp.hysaishi.cn

TS:   s.indexOf("x")
来源：http://nxh.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://ime.pycfn.com

Go:   strings.Index(s, "x")
来源：http://mux.cdnleiting.top

Ruby: s.index("x")
来源：http://ols.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://wtn.vqdsnc.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xoh.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qrz.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zcw.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hsj.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://cws.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yvj.aizwys.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fca.nwbrower.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jex.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vhy.jinqigufen.top

[E06] 替换子串
来源：http://prl.zhijiandao.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://snn.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://cmm.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsd.uphjek.com

TS:   s.replaceAll("a", "b")
来源：http://gkc.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://upv.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sep.tianlin.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xrw.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://oia.ctjpmb.com

[E07] 按分隔符拆分
来源：http://hxg.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://aye.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://obn.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://grk.yongpay.top

TS:   s.split(",")
来源：http://wgq.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://vyi.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://adr.jqgfzy.top

Ruby: s.split(",");  s.split
来源：http://vkh.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qyb.xziqi.cn

[E08] 数组按分隔符合并
来源：http://ngk.andypj.xyz

Py:   ",".join(items)
来源：http://jta.gotoacloud.top

PHP:  implode(",", $items);
来源：http://cmc.bbcook.cn

JS:   items.join(",")
来源：http://mjd.xziqi.cn

TS:   items.join(",")
来源：http://yaz.yj20258888.top

Java: String.join(",", items)
来源：http://qcs.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://dgv.cqqwz.cn

Ruby: items.join(",")
来源：http://xjx.gotoacloud.top

C#:   string.Join(",", items)
来源：http://plf.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://coq.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fes.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hst.andypj.xyz

JS:   s.replace(/\s+/g, "")
来源：http://iga.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://hjx.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://gjk.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bpf.dianchejie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vhy.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://emj.yongpay.top

[E10] 左侧补零 / 定长填充
来源：http://ani.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://iax.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ken.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://rgv.zhixingplan.top

TS:   "7".padStart(3, "0")
来源：http://ziz.mhx1999.top

Java: String.format("%03d", 7)
来源：http://xln.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kdx.ctjpmb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pwj.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mtx.yuxming.cn

[E11] 反转字符串
来源：http://wwy.wangshuangyany.cn

Py:   s[::-1]
来源：http://rwv.zhixingplan.top

PHP:  strrev($s);
来源：http://wiy.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://jkd.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://dxn.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zbp.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eew.chenjidiqi.icu


<!-- 参考信息 -->