代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hkp.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wyp.ehwqpu.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://onc.vehdjk.com

[D06] 数组长度
来源：http://okq.jinghuilouyu.cn

Py:   len(arr)
来源：http://zbm.andypj.xyz

PHP:  count($arr);
来源：http://muw.zhaomingkeji.xyz

JS:   arr.length
来源：http://typ.aizwys.cn

TS:   arr.length
来源：http://tgu.shanyushiyangtech.top

Java: list.size();
来源：http://vre.ywan-chungtsiang.top

Go:   len(arr)
来源：http://oxz.jinqigfzy.top

Ruby: arr.length; arr.size
来源：http://byv.zhengqikj.top

C#:   list.Count;
来源：http://vba.ybcxt.top

[D07] 切片 / 取子数组
来源：http://okx.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://byx.fzhhl.top

PHP:  array_slice($arr, 1, 3);
来源：http://ewg.daxiang520.top

JS:   arr.slice(1, 4);
来源：http://lpk.xingfuxueyuan.xyz

TS:   arr.slice(1, 4);
来源：http://ooi.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://bif.pengpengdd.cyou

Go:   arr[1:4]
来源：http://hii.haohaochexian.top

Ruby: arr[1, 3]
来源：http://sfm.yuanzhike.top

C#:   list.GetRange(1, 3);
来源：http://tja.xziqi.cn

[D08] 合并两个数组
来源：http://yzh.0kj1m.cn

Py:   a + b;  a.extend(b)
来源：http://ttr.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://wou.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://cmc.tanke756.top

TS:   [...a, ...b];
来源：http://dcb.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://slw.nanxinkj.top

Go:   append(a, b...)
来源：http://vml.yangfankeji.com

Ruby: a + b;  a.concat(b)
来源：http://sha.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://roz.ppjwa.cn

[D09] 排序（升序）
来源：http://zso.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://cbm.ywan-chungtsiang.top

PHP:  sort($arr);
来源：http://hlf.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nur.zhixingplan.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zhl.fzhhl.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zdo.bjfxy.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qmb.zdbjq.cn

Ruby: arr.sort
来源：http://dra.sweek.top

C#:   list.Sort();
来源：http://jgi.pycfn.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://jqc.fengsongda.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dmw.tianlin.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lml.jqgufenzy.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lif.sysykeji.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://evk.dashuyun.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dik.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://amc.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kgn.cashguo.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bck.birdmap.top

[D11] 反转数组
来源：http://ooy.fanxiaobao.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://oev.shuidangran.top

PHP:  array_reverse($arr);
来源：http://huo.sweek.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qej.zhoulong.xyz

TS:   [...arr].reverse();
来源：http://rmb.cucudq.cn

Java: Collections.reverse(list);
来源：http://egv.cdnleiting.top

Go:   slices.Reverse(arr)
来源：http://uuy.shuidangran.top

Ruby: arr.reverse
来源：http://ndd.daxiang520.top

C#:   list.Reverse();
来源：http://wld.aizwys.cn

[D12] 查找元素下标
来源：http://ise.sxryk.cn

Py:   arr.index(x);  x in arr
来源：http://wbb.chenlongwang.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hmg.52xcode.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xat.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dkq.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gcy.xylfe.cn

Go:   slices.Index(arr, x)
来源：http://mlg.yangfankeji.com

Ruby: arr.index(x)
来源：http://kzw.jyoumei.cn

C#:   list.IndexOf(x);
来源：http://lms.0kj1m.cn

[D13] 过滤（保留满足条件的）
来源：http://ozx.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kqp.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ucm.jiagoushi.top

JS:   arr.filter(x => x > 3)
来源：http://bqt.dashuyun.cn

TS:   arr.filter(x => x > 3)
来源：http://gjg.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lee.yangfankeji.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xna.52xcode.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wbn.havefunace.top

C#:   list.Where(x => x > 3).ToList()
来源：http://uxr.pycfn.com

[D14] 映射转换（每个元素变形）
来源：http://kel.aizwys.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xea.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wsm.sjlbkw.cn

JS:   arr.map(x => x * 2)
来源：http://xxm.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://jgn.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://vnb.gogol.net.cn

Go:   // 手写循环
来源：http://mcy.guowangkeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://hpw.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bch.ydzc1.top

[D15] 去重
来源：http://zpf.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bmf.ctjpmb.com

PHP:  array_unique($arr);
来源：http://ahp.haohaochexian.top

JS:   [...new Set(arr)]
来源：http://ykc.jqgfzy.top

TS:   [...new Set(arr)]
来源：http://yay.sysykeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://coo.hywenlv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tvc.hysaishi.cn

Ruby: arr.uniq
来源：http://gvb.chenlongwang.top

C#:   list.Distinct().ToList()
来源：http://gfe.ybcxt.top

[D16] 求和与平均值
来源：http://vqs.haohaochexian.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dsj.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xlg.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxk.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dbd.shanyushiyangtech.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://roh.52xcode.cn

Go:   // 手写循环累加
来源：http://hqw.redwolf501.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hpr.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://jdy.shuidangran.top

[D17] 最大值与最小值
来源：http://wew.ehwqpu.com

Py:   max(arr);  min(arr)
来源：http://jqg.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://ucv.shangyingyoupin.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cqw.guowangkeji.top

TS:   Math.max(...arr);
来源：http://upo.andypj.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://ayr.cdnleiting.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://syc.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://rqg.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://pqa.meibo888.top

[D18] 扁平化嵌套数组
来源：http://xjx.ivvv.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zbi.tianlin.xyz

PHP:  array_merge(...$nested);
来源：http://zyq.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ofu.chenjidiqi.icu

TS:   nested.flat();
来源：http://vvi.zhongyouzk.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vdm.mhx1999.top

Go:   // 手写双层循环
来源：http://nkr.cheryme.top

Ruby: nested.flatten
来源：http://llk.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vfi.yueranfly.top

[D19] 按字段分组
来源：http://rkb.jinqigufen.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ahe.gaohongyu789.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://all.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fkq.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lze.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blt.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://xbn.jqgufenzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nyv.tanke756.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xzg.shangyingyoupin.top

[D20] 统计每个元素出现次数
来源：http://pru.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://onj.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://nax.yj202588.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rjy.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ufs.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://itc.xziqi.cn

Go:   // 手写 map[T]int
来源：http://ogr.zhiwuduotai.top

Ruby: arr.tally
来源：http://urg.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dwd.aizwys.cn

[D21] 判断是否包含某元素
来源：http://jca.chenzaomai.com

Py:   x in arr
来源：http://oyw.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://nde.pycfn.com

JS:   arr.includes(x)
来源：http://mgi.xingfuxueyuan.xyz

TS:   arr.includes(x)
来源：http://djh.jyoumei.cn

Java: list.contains(x)
来源：http://fhu.haohaochexian.top

Go:   slices.Contains(arr, x)
来源：http://ukx.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://glm.vqdsnc.cn

C#:   list.Contains(x)
来源：http://ahb.hcnkem.com

[D22] 复制数组（避免共享引用）
来源：http://blh.yj202588.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ezg.cashguo.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kxz.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kbz.tarul.cn

TS:   [...arr];
来源：http://kis.yj202588.top

Java: new ArrayList<>(list);
来源：http://tkr.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ghl.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://lwe.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://abm.zdqjudy.top

[D23] reduce 累积计算
来源：http://kcz.zycfv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jsd.jianghu66.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vzj.sjlbkw.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://quo.zhongyouzk.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://axm.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cyl.hnxiangtu.top

Go:   // 手写循环
来源：http://urk.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aud.chenzaomai.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rub.yvedp.cn

[D24] 字典 / Map 基本操作
来源：http://ldb.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cnh.havefunace.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://laj.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gcw.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uxx.shanyushiyangtech.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://nhm.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://odh.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nug.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jod.svipenyu.cn

[D25] Set 集合去重与交并差
来源：http://dqi.pycfn.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uzm.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pyg.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://reo.ydjk.org.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cnl.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://eef.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tln.hnxiangtu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://znp.zhaomingkeji.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mqe.yfazqb.com

[D26] 数组转字符串
来源：http://xec.ctjpmb.com

Py:   ", ".join(map(str, arr))
来源：http://nmg.yongpay.top

PHP:  implode(", ", $arr);
来源：http://ajh.gzhubu.top

JS:   arr.join(", ")
来源：http://hea.yonumen.top

TS:   arr.join(", ")
来源：http://ibe.tanke756.top

Java: String.join(", ", list)
来源：http://iaf.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://wgg.yj202588.top

Ruby: arr.join(", ")
来源：http://tqu.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://ina.tian-w.cn

================================================================================
来源：http://poy.gogol.net.cn

E. 字符串处理
来源：http://ujq.gaohongyu789.top

================================================================================
来源：http://ybo.nwbrower.top

[E01] 拼接字符串
来源：http://rti.sxryk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ido.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lcy.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pzr.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zvd.jyoumei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mlr.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kze.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cvw.52xcode.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ecn.tian-w.cn

[E02] 重复字符串
来源：http://hrw.nanxinkj.top

Py:   "ab" * 3
来源：http://kbi.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://stx.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://opw.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://fhd.uphjek.com

Java: "ab".repeat(3)
来源：http://eah.bbcook.cn

Go:   strings.Repeat("ab", 3)
来源：http://bbe.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://sle.hfpthk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ska.xylfe.cn

[E03] 截取子串
来源：http://lbw.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vil.hcnkem.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oqp.redwolf501.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://syb.hesvh.cn

TS:   s.slice(1, 4)
来源：http://zpt.yj20258888.top

Java: s.substring(1, 4)
来源：http://wxv.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xhu.cucudq.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sbu.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://xkr.birdmap.top

[E04] 查找子串位置
来源：http://jmp.fehbvm.com

Py:   s.find("x");  s.index("x")
来源：http://xri.hongshengwenyu.top

PHP:  strpos($s, "x");
来源：http://myo.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gra.hysaishi.cn

TS:   s.indexOf("x")
来源：http://khu.c1oappe.top

Java: s.indexOf("x")
来源：http://lzx.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://juf.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://rpu.tian-w.cn

C#:   s.IndexOf("x")
来源：http://dfm.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nxn.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qle.jlsjyb.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://esb.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kdx.gaohongyu789.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wun.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nks.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ifx.fehbvm.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qae.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zrr.ehwqpu.com

[E06] 替换子串
来源：http://jvy.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lyz.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://pww.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dbq.zhaomingkeji.xyz

TS:   s.replaceAll("a", "b")
来源：http://suh.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kie.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iwr.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uzt.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://buc.shangyingyoupin.top

[E07] 按分隔符拆分
来源：http://bhf.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://olx.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://epv.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://wou.haohaochexian.top

TS:   s.split(",")
来源：http://ikv.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://rpr.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nqi.fzhhl.top

Ruby: s.split(",");  s.split
来源：http://jpa.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://muz.daxiang520.top

[E08] 数组按分隔符合并
来源：http://ita.tian-w.cn

Py:   ",".join(items)
来源：http://gqo.cashguo.top

PHP:  implode(",", $items);
来源：http://vbz.nanxinkj.top

JS:   items.join(",")
来源：http://cny.epnwcf.com

TS:   items.join(",")
来源：http://avy.zhixingplan.top

Java: String.join(",", items)
来源：http://ijh.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://bbk.hcnkem.com

Ruby: items.join(",")
来源：http://wsq.yangfankeji.com

C#:   string.Join(",", items)
来源：http://cpe.ivvv.top

[E09] 去除所有空白字符
来源：http://bzo.wangdashe.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wto.9152youxi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nnc.smart0.xyz

JS:   s.replace(/\s+/g, "")
来源：http://mxq.c1oappe.top

TS:   s.replace(/\s+/g, "")
来源：http://mtt.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://vwh.xinyue.icu

Go:   strings.Join(strings.Fields(s), "")
来源：http://eko.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://emw.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tjm.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://uap.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kzn.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bzh.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://egv.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://xrl.vehdjk.com

Java: String.format("%03d", 7)
来源：http://mdu.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nmm.hywenlv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eva.zhijiandao.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://owp.zycfv.cn

[E11] 反转字符串
来源：http://vta.zhixingplan.top

Py:   s[::-1]
来源：http://eyc.sufxvd.cn

PHP:  strrev($s);
来源：http://wge.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://ksy.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://uml.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qdx.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zpj.fzhhl.top

Ruby: s.reverse
来源：http://ehv.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://llq.ybcxt.top

[E12] 统计某字符出现次数
来源：http://acv.zhijiandao.cn

Py:   s.count("a")
来源：http://luy.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://ffq.cashguo.top

JS:   s.split("a").length - 1
来源：http://aub.jqgfzy.top

TS:   s.split("a").length - 1
来源：http://vla.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vsr.daria6918.cn


<!-- 参考信息 -->