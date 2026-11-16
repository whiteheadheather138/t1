代发 wailian999

Py:   len(arr)
来源：http://vli.ywan-chungtsiang.top

PHP:  count($arr);
来源：http://rbm.meibo888.top

JS:   arr.length
来源：http://vjf.zhaomingkeji.xyz

TS:   arr.length
来源：http://iss.guowangkeji.top

Java: list.size();
来源：http://asc.zhaomingkeji.xyz

Go:   len(arr)
来源：http://rfq.shanyushiyangtech.top

Ruby: arr.length; arr.size
来源：http://pge.ehwqpu.com

C#:   list.Count;
来源：http://syj.yuanzhike.top

[D07] 切片 / 取子数组
来源：http://qyf.jiagoushi.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kbk.ehwqpu.com

PHP:  array_slice($arr, 1, 3);
来源：http://zex.jqgufenzy.top

JS:   arr.slice(1, 4);
来源：http://ncu.gotoacloud.top

TS:   arr.slice(1, 4);
来源：http://jri.cqqwz.cn

Java: list.subList(1, 4);
来源：http://dpv.zhixingplan.top

Go:   arr[1:4]
来源：http://sdn.jianghu66.top

Ruby: arr[1, 3]
来源：http://rpr.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://tzo.svipenyu.cn

[D08] 合并两个数组
来源：http://jmx.dianchejie.cn

Py:   a + b;  a.extend(b)
来源：http://ahq.pengpengdd.cyou

PHP:  array_merge($a, $b);
来源：http://jyu.jqgfzy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://dvl.zdbjq.cn

TS:   [...a, ...b];
来源：http://znr.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bwr.fktsv.cn

Go:   append(a, b...)
来源：http://xtj.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://lby.cashguo.top

C#:   a.Concat(b).ToList()
来源：http://ocr.0kj1m.cn

[D09] 排序（升序）
来源：http://cvv.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://djc.xuetiantiany.cn

PHP:  sort($arr);
来源：http://zxo.yongpay.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://scm.yfazqb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://wnd.jiagoushi.top

Java: Collections.sort(list);  list.sort(null);
来源：http://apz.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://asm.ydzc1.top

Ruby: arr.sort
来源：http://dvd.hnxiangtu.top

C#:   list.Sort();
来源：http://fsj.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jie.nwbrower.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://uwj.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rsm.gogol.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://alm.shzxlz.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yad.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gfq.tanke756.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wve.haohaochexian.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://roj.jinyuanbaomall.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hep.tian-w.cn

[D11] 反转数组
来源：http://pyu.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vwv.jinqigfzy.top

PHP:  array_reverse($arr);
来源：http://nkh.tarul.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hpl.hnxiangtu.top

TS:   [...arr].reverse();
来源：http://cci.daxiang520.top

Java: Collections.reverse(list);
来源：http://skf.gaohongyu789.top

Go:   slices.Reverse(arr)
来源：http://bml.ehwqpu.com

Ruby: arr.reverse
来源：http://rwe.chenzaomai.com

C#:   list.Reverse();
来源：http://syc.tarul.cn

[D12] 查找元素下标
来源：http://vli.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://kfd.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pqx.jqgufenzy.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gou.sufxvd.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fbk.jlsjyb.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uhq.hesvh.cn

Go:   slices.Index(arr, x)
来源：http://sbw.sweek.top

Ruby: arr.index(x)
来源：http://msv.yueranfly.top

C#:   list.IndexOf(x);
来源：http://juv.zhixingplan.top

[D13] 过滤（保留满足条件的）
来源：http://pqo.yj20258888.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avo.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mvv.shzxlz.cn

JS:   arr.filter(x => x > 3)
来源：http://ins.kuanghao11.cn

TS:   arr.filter(x => x > 3)
来源：http://htz.tian-w.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://egh.hcnkem.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://unr.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://crb.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://jwr.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://rsj.cqqwz.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hcj.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://non.ywan-chungtsiang.top

JS:   arr.map(x => x * 2)
来源：http://fse.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://llp.zdqjudy.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ark.fanxiaobao.xyz

Go:   // 手写循环
来源：http://jbq.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rkk.fanxiaobao.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://ewx.xingfuxueyuan.xyz

[D15] 去重
来源：http://jqj.tianlin.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hnv.zdqjudy.top

PHP:  array_unique($arr);
来源：http://nyx.jinyuanbaomall.cn

JS:   [...new Set(arr)]
来源：http://ogc.zhixingplan.top

TS:   [...new Set(arr)]
来源：http://evj.cucudq.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lqu.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://wji.dashuyun.cn

Ruby: arr.uniq
来源：http://nbr.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://exi.yvedp.cn

[D16] 求和与平均值
来源：http://zag.yonumen.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oow.cqqwz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://eqq.jinyuanbaomall.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ebj.c1oappe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zho.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgp.xuanzx.com

Go:   // 手写循环累加
来源：http://vao.chenzaomai.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ynx.yongpay.top

C#:   list.Sum();  list.Average()
来源：http://vsa.zhiwuduotai.top

[D17] 最大值与最小值
来源：http://kkd.feifeiyinyue.top

Py:   max(arr);  min(arr)
来源：http://xtm.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://pol.birdmap.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://suy.xuanzx.com

TS:   Math.max(...arr);
来源：http://bgi.xuanzx.com

Java: Collections.max(list);  Collections.min(list);
来源：http://xgp.jqgfzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bhu.316326.xyz

Ruby: arr.max;  arr.min
来源：http://uef.cashguo.top

C#:   list.Max();  list.Min()
来源：http://vqb.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://iio.shangyingyoupin.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jdp.ivvv.top

PHP:  array_merge(...$nested);
来源：http://ghg.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yqb.dianchejie.cn

TS:   nested.flat();
来源：http://jer.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://slg.tianlin.xyz

Go:   // 手写双层循环
来源：http://uuk.vqdsnc.cn

Ruby: nested.flatten
来源：http://mgg.yuanzhike.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://wbs.zdqjudy.top

[D19] 按字段分组
来源：http://jar.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fwg.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rpy.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhf.ywan-chungtsiang.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cnd.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eop.shanyushiyangkeji.top

Go:   // 手写 map[string][]T
来源：http://ipq.zdbjq.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ixk.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vtj.feifeiyinyue.top

[D20] 统计每个元素出现次数
来源：http://zuc.xylfe.cn

Py:   Counter(arr)
来源：http://jux.zhengqikj.top

PHP:  array_count_values($arr);
来源：http://see.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aen.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgy.fanxiaobao.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bdy.hnqzz.top

Go:   // 手写 map[T]int
来源：http://xly.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://puh.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qew.aibaodan.cn

[D21] 判断是否包含某元素
来源：http://ucq.yongpay.top

Py:   x in arr
来源：http://siu.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://tdi.ehwqpu.com

JS:   arr.includes(x)
来源：http://cqw.andypj.xyz

TS:   arr.includes(x)
来源：http://ozl.gaohongyu789.top

Java: list.contains(x)
来源：http://jdr.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://duc.yj20258888.top

Ruby: arr.include?(x)
来源：http://dyi.zhijiandao.cn

C#:   list.Contains(x)
来源：http://max.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://mtx.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lxb.zycfv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ulu.ctjpmb.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hnk.chenlongwang.top

TS:   [...arr];
来源：http://uef.sysykeji.top

Java: new ArrayList<>(list);
来源：http://hwt.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://yyk.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://zmt.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://yfu.nanxuanxn.top

[D23] reduce 累积计算
来源：http://gjl.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cwk.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nbk.gotoacloud.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rrt.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxv.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pxi.yfazqb.com

Go:   // 手写循环
来源：http://ctd.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pih.yonumen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cow.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://aki.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tkw.yj202588.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xch.zhixingplan.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://btu.hnxiangtu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vee.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lrs.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ldn.ctjpmb.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bsl.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ceq.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://wmx.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mrd.wangdashe.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gpo.pycfn.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hir.pengpengdd.cyou

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://btl.shangyingyoupin.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ouf.cashguo.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ecm.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eel.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hhz.zhiwuduotai.top

[D26] 数组转字符串
来源：http://xpb.fehbvm.com

Py:   ", ".join(map(str, arr))
来源：http://jjy.316326.xyz

PHP:  implode(", ", $arr);
来源：http://mpj.quarkkingdee.top

JS:   arr.join(", ")
来源：http://knp.hesvh.cn

TS:   arr.join(", ")
来源：http://kop.gogol.net.cn

Java: String.join(", ", list)
来源：http://jiv.tarul.cn

Go:   strings.Join(strs, ", ")
来源：http://bzj.sjlbkw.cn

Ruby: arr.join(", ")
来源：http://lfj.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://rzr.ydzc1.top

================================================================================
来源：http://tec.c1oappe.top

E. 字符串处理
来源：http://dwm.cqqwz.cn

================================================================================
来源：http://iiq.jlsjyb.cn

[E01] 拼接字符串
来源：http://kca.zhongyouzk.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bss.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tvw.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jgz.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://huh.zhijiandao.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://djl.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hfg.pycfn.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ugt.jyoumei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cit.tian-w.cn

[E02] 重复字符串
来源：http://och.jqgfzy.top

Py:   "ab" * 3
来源：http://asb.quarkkingdee.top

PHP:  str_repeat("ab", 3);
来源：http://xpq.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://nal.sysykeji.top

TS:   "ab".repeat(3)
来源：http://wtz.cheryme.top

Java: "ab".repeat(3)
来源：http://lhb.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://yfj.c1oappe.top

Ruby: "ab" * 3
来源：http://ryd.hysaishi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pfu.shanyushiyangtech.top

[E03] 截取子串
来源：http://dmc.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lqp.yonumen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tqi.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kzg.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://lsq.ctjpmb.com

Java: s.substring(1, 4)
来源：http://ayq.iojbl.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pug.tian-w.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qph.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://wdf.wangdashe.top

[E04] 查找子串位置
来源：http://dkb.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://zsq.sweek.top

PHP:  strpos($s, "x");
来源：http://gow.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lyj.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://wcu.yfazqb.com

Java: s.indexOf("x")
来源：http://zrj.nanxuanxn.top

Go:   strings.Index(s, "x")
来源：http://gdq.zycfv.cn

Ruby: s.index("x")
来源：http://wkt.quarkkingdee.top

C#:   s.IndexOf("x")
来源：http://zyn.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pgp.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lxg.xziqi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gre.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://roa.9152youxi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tkg.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qmi.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fje.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lgu.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hpr.sjlbkw.cn

[E06] 替换子串
来源：http://rjb.dashuyun.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wyw.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://utf.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hqq.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://tnf.hysaishi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iah.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rbe.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iub.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://gmj.xinyue.icu

[E07] 按分隔符拆分
来源：http://iys.birdmap.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eqo.fktsv.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dcp.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ssp.hnxiangtu.top

TS:   s.split(",")
来源：http://cvq.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://vom.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://apl.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://pqs.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ifv.316326.xyz

[E08] 数组按分隔符合并
来源：http://nlm.316326.xyz

Py:   ",".join(items)
来源：http://lfa.yvedp.cn

PHP:  implode(",", $items);
来源：http://iea.uphjek.com

JS:   items.join(",")
来源：http://jrz.meibo888.top

TS:   items.join(",")
来源：http://qxn.nwbrower.top

Java: String.join(",", items)
来源：http://mok.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://chf.mhx1999.top

Ruby: items.join(",")
来源：http://amo.c1oappe.top

C#:   string.Join(",", items)
来源：http://grf.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://cie.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wtk.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://exj.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://hmm.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://ndr.redwolf501.top

Java: s.replaceAll("\\s+", "")
来源：http://adb.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://njg.52xcode.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ths.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ggu.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://jzn.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ohq.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xch.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://knt.jinqigufen.top

TS:   "7".padStart(3, "0")
来源：http://yad.fehbvm.com

Java: String.format("%03d", 7)
来源：http://lsu.0kj1m.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://shz.fzhhl.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xpn.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cge.sxryk.cn

[E11] 反转字符串
来源：http://uwz.cashguo.top

Py:   s[::-1]
来源：http://rzl.316326.xyz

PHP:  strrev($s);
来源：http://znz.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://djl.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://uzj.zycfv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bpx.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dws.xylfe.cn

Ruby: s.reverse
来源：http://ged.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://uhk.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://wmq.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://duu.havefunace.top

PHP:  substr_count($s, "a");
来源：http://whp.yuxming.cn

JS:   s.split("a").length - 1
来源：http://cuz.daxiang520.top

TS:   s.split("a").length - 1
来源：http://plb.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://anx.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://byk.zycfv.cn

Ruby: s.count("a")
来源：http://ssd.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://kot.tian-w.cn

[E13] 逐字符遍历
来源：http://gtb.birdmap.top


<!-- 参考信息 -->