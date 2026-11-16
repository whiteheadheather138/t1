代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://shi.gzhubu.top

TS:   [...a, ...b];
来源：http://psi.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://psg.ehwqpu.com

Go:   append(a, b...)
来源：http://gew.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://qxq.quarkkingdee.top

C#:   a.Concat(b).ToList()
来源：http://kwx.52xcode.cn

[D09] 排序（升序）
来源：http://rup.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://wyh.aizwys.cn

PHP:  sort($arr);
来源：http://jrl.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qzm.sxryk.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pdu.andypj.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://unz.smart0.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uys.sjlbkw.cn

Ruby: arr.sort
来源：http://gro.zhiwuduotai.top

C#:   list.Sort();
来源：http://gun.zhijiandao.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nci.sweek.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://swc.jinghuilouyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zai.hammf.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rwq.wangshuangyany.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zgn.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://por.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://edf.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://odq.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aau.yongpay.top

[D11] 反转数组
来源：http://hjx.fzhhl.top

Py:   arr[::-1];  arr.reverse()
来源：http://dfx.shanyushiyangtech.top

PHP:  array_reverse($arr);
来源：http://tdl.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sse.cheryme.top

TS:   [...arr].reverse();
来源：http://krw.ppjwa.cn

Java: Collections.reverse(list);
来源：http://dvb.ivvv.top

Go:   slices.Reverse(arr)
来源：http://bfh.zdbjq.cn

Ruby: arr.reverse
来源：http://wtx.fehbvm.com

C#:   list.Reverse();
来源：http://qit.jqgufenzy.top

[D12] 查找元素下标
来源：http://mmw.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://vow.shuidangran.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tjz.xinyue.icu

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://aoz.yonumen.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dzr.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vtn.hongshengwenyu.top

Go:   slices.Index(arr, x)
来源：http://kjz.zhongyouzk.top

Ruby: arr.index(x)
来源：http://piw.sufxvd.cn

C#:   list.IndexOf(x);
来源：http://ohm.jqgfzy.top

[D13] 过滤（保留满足条件的）
来源：http://kcs.nanxinkj.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pvs.cashguo.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bdw.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://dwt.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://axa.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://glw.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://coe.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://cbs.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ppi.zhiwuduotai.top

[D14] 映射转换（每个元素变形）
来源：http://fyz.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mli.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://axq.zhiwuduotai.top

JS:   arr.map(x => x * 2)
来源：http://mjn.hesvh.cn

TS:   arr.map(x => x * 2)
来源：http://ytt.yueranfly.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://mjn.jianghu66.top

Go:   // 手写循环
来源：http://oiu.wangshuangyany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jfh.chenzaomai.com

C#:   list.Select(x => x * 2).ToList()
来源：http://mck.hnxiangtu.top

[D15] 去重
来源：http://lov.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tns.c1oappe.top

PHP:  array_unique($arr);
来源：http://tiz.xuanzx.com

JS:   [...new Set(arr)]
来源：http://eef.ydjk.org.cn

TS:   [...new Set(arr)]
来源：http://ypr.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pfl.haohaochexian.top

Go:   // 用 map[T]struct{} 手写
来源：http://jjv.pengpengdd.cyou

Ruby: arr.uniq
来源：http://vgi.fzhhl.top

C#:   list.Distinct().ToList()
来源：http://nwe.yangfankeji.com

[D16] 求和与平均值
来源：http://coi.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ncq.yj202588.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nar.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vub.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bec.zhongyouzk.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qkj.daria6918.cn

Go:   // 手写循环累加
来源：http://dxf.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qrw.aizwys.cn

C#:   list.Sum();  list.Average()
来源：http://wul.xylfe.cn

[D17] 最大值与最小值
来源：http://kum.cheryme.top

Py:   max(arr);  min(arr)
来源：http://wli.shanyushiyangkeji.top

PHP:  max($arr);  min($arr);
来源：http://wvt.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jlr.jiagoushi.top

TS:   Math.max(...arr);
来源：http://wuu.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hbx.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://syz.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://uvv.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://edh.aibaodan.cn

[D18] 扁平化嵌套数组
来源：http://hew.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lds.yj202588.top

PHP:  array_merge(...$nested);
来源：http://yyh.hywenlv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://krn.xylfe.cn

TS:   nested.flat();
来源：http://cls.jqgufenzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://weg.guowangkeji.top

Go:   // 手写双层循环
来源：http://yks.nwbrower.top

Ruby: nested.flatten
来源：http://vuy.zdbjq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xfp.316326.xyz

[D19] 按字段分组
来源：http://hlm.haohaochexian.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://icc.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://paf.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aeo.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ltm.havefunace.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oph.bbcook.cn

Go:   // 手写 map[string][]T
来源：http://rsw.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://evg.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zfn.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://afz.snrcjt.cn

Py:   Counter(arr)
来源：http://qrn.iojbl.cn

PHP:  array_count_values($arr);
来源：http://oxo.jinqigfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jqr.fehbvm.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ewb.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ehc.jinqigfzy.top

Go:   // 手写 map[T]int
来源：http://ekz.zhiwuduotai.top

Ruby: arr.tally
来源：http://vkh.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tiv.quarkkingdee.top

[D21] 判断是否包含某元素
来源：http://fnb.shuidangran.top

Py:   x in arr
来源：http://atm.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://rfs.jinghuilouyu.cn

JS:   arr.includes(x)
来源：http://grc.fzhhl.top

TS:   arr.includes(x)
来源：http://ldr.cqqwz.cn

Java: list.contains(x)
来源：http://zai.tarul.cn

Go:   slices.Contains(arr, x)
来源：http://arc.hysaishi.cn

Ruby: arr.include?(x)
来源：http://tdi.guowangkeji.top

C#:   list.Contains(x)
来源：http://xhl.yj20258.top

[D22] 复制数组（避免共享引用）
来源：http://auw.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fqc.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sym.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://flx.jqgufenzy.top

TS:   [...arr];
来源：http://sni.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://bjk.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fjk.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://ygn.feifeiyinyue.top

C#:   new List<int>(list);
来源：http://hev.52xcode.cn

[D23] reduce 累积计算
来源：http://tkc.jinqigfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nrs.jyoumei.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sjk.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sun.nanxuanxn.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sxp.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gnk.chenzaomai.com

Go:   // 手写循环
来源：http://eqi.pycfn.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kvk.zdbjq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://twm.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://vfr.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hes.mhx1999.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zlz.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hgn.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oid.birdmap.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://evs.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ybl.ivvv.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iki.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sik.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://qkf.yj20258.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ctn.chenzaomai.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qor.jinghuilouyu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hxj.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zuj.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://voz.svipenyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://imh.zhengqikj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://onm.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://apu.yuxming.cn

[D26] 数组转字符串
来源：http://tpt.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://uon.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://unw.feifeiyinyue.top

JS:   arr.join(", ")
来源：http://xko.yj20258.top

TS:   arr.join(", ")
来源：http://utx.xziqi.cn

Java: String.join(", ", list)
来源：http://njd.yj202588.top

Go:   strings.Join(strs, ", ")
来源：http://shx.cheryme.top

Ruby: arr.join(", ")
来源：http://seo.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://ouy.cheryme.top

================================================================================
来源：http://gju.ivvv.top

E. 字符串处理
来源：http://oky.bjfxy.top

================================================================================
来源：http://yyb.sweek.top

[E01] 拼接字符串
来源：http://zvu.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vqb.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://duf.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jjh.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://izn.yueranfly.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ogn.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zmp.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jos.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ztc.tanke756.top

[E02] 重复字符串
来源：http://glo.0kj1m.cn

Py:   "ab" * 3
来源：http://ukb.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://afv.tianlin.xyz

JS:   "ab".repeat(3)
来源：http://chx.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://uem.jinqigufen.top

Java: "ab".repeat(3)
来源：http://hkn.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://lzc.fktsv.cn

Ruby: "ab" * 3
来源：http://grx.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wmj.gogol.net.cn

[E03] 截取子串
来源：http://isc.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gst.chenzaomai.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dcm.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cow.jinghuilouyu.cn

TS:   s.slice(1, 4)
来源：http://eyc.zdqjudy.top

Java: s.substring(1, 4)
来源：http://sqg.zdqjudy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xon.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://psw.yanxiufei.cn

C#:   s.Substring(1, 3)
来源：http://kce.daria6918.cn

[E04] 查找子串位置
来源：http://axj.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://rze.uphjek.com

PHP:  strpos($s, "x");
来源：http://qzz.yangfankeji.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pdg.zycfv.cn

TS:   s.indexOf("x")
来源：http://eup.ppjwa.cn

Java: s.indexOf("x")
来源：http://ldq.ivvv.top

Go:   strings.Index(s, "x")
来源：http://vma.dashuyun.cn

Ruby: s.index("x")
来源：http://yzi.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://cue.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oqg.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lzl.sxryk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qzy.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://moj.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ccv.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjp.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fim.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lna.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ujk.cucudq.cn

[E06] 替换子串
来源：http://vgh.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mtt.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://qru.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rsd.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://jzj.ivvv.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uzf.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hvd.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rpz.havefunace.top

C#:   s.Replace("a", "b")
来源：http://qcw.yuanzhike.top

[E07] 按分隔符拆分
来源：http://fva.daria6918.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mbk.shanyushiyangtech.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yis.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hfh.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://ikl.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lka.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bpy.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://oht.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vma.zhongyouzk.top

[E08] 数组按分隔符合并
来源：http://meg.snrcjt.cn

Py:   ",".join(items)
来源：http://knp.sysykeji.top

PHP:  implode(",", $items);
来源：http://pgn.sysykeji.top

JS:   items.join(",")
来源：http://apb.yanxiufei.cn

TS:   items.join(",")
来源：http://ffr.mhx1999.top

Java: String.join(",", items)
来源：http://zoy.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://tnz.shanyushiyangkeji.top

Ruby: items.join(",")
来源：http://qbg.ehwqpu.com

C#:   string.Join(",", items)
来源：http://kaq.jlsjyb.cn

[E09] 去除所有空白字符
来源：http://ajs.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mbb.quarkkingdee.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ckr.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://zlp.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://oqb.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://umc.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://xhl.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ehy.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rxb.iojbl.cn

[E10] 左侧补零 / 定长填充
来源：http://pfw.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://znc.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://czt.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://ivn.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://lpp.redwolf501.top

Java: String.format("%03d", 7)
来源：http://csd.fehbvm.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lir.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rky.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ysc.52xcode.cn

[E11] 反转字符串
来源：http://ocr.pycfn.com

Py:   s[::-1]
来源：http://eet.guowangkeji.top

PHP:  strrev($s);
来源：http://zeh.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://iry.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://cph.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hbu.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gjc.52xcode.cn

Ruby: s.reverse
来源：http://ljk.316326.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://yda.sxryk.cn

[E12] 统计某字符出现次数
来源：http://wqi.tanke756.top

Py:   s.count("a")
来源：http://ckh.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://ubw.jianghu66.top

JS:   s.split("a").length - 1
来源：http://eza.bjfxy.top

TS:   s.split("a").length - 1
来源：http://qsq.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hry.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://cxv.9152youxi.cn

Ruby: s.count("a")
来源：http://epq.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://yhu.cheryme.top

[E13] 逐字符遍历
来源：http://bbc.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://avs.0kj1m.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ssd.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lmr.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://knc.zhaomingkeji.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bqu.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://may.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fwz.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tdd.nwbrower.top

[E14] URL 编码与 Base64
来源：http://dgu.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uca.mhx1999.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kwf.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jmn.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xrq.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jay.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dmy.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://swc.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ptl.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://ind.guannengcc.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eel.zhongyouzk.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wqz.mhx1999.top


<!-- 参考信息 -->