代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kba.chenzaomai.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tgq.jlsjyb.cn

TS:   arr[0]; arr.at(-1);
来源：http://ync.316326.xyz

Java: list.get(0); list.set(0, 9);
来源：http://xnp.sufxvd.cn

Go:   arr[0]; arr[0] = 9
来源：http://nud.zdbjq.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ycp.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://rgv.cashguo.top

[D06] 数组长度
来源：http://xcn.52xcode.cn

Py:   len(arr)
来源：http://dxy.gaohongyu789.top

PHP:  count($arr);
来源：http://uht.tanke756.top

JS:   arr.length
来源：http://wpq.jianghu66.top

TS:   arr.length
来源：http://ikm.zhixingplan.top

Java: list.size();
来源：http://ipe.hesvh.cn

Go:   len(arr)
来源：http://jcc.iojbl.cn

Ruby: arr.length; arr.size
来源：http://gpm.ppjwa.cn

C#:   list.Count;
来源：http://sfx.birdmap.top

[D07] 切片 / 取子数组
来源：http://hkx.zycfv.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rqh.316326.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://qlc.sysykeji.top

JS:   arr.slice(1, 4);
来源：http://low.yj202588.top

TS:   arr.slice(1, 4);
来源：http://olz.yvedp.cn

Java: list.subList(1, 4);
来源：http://avc.vqdsnc.cn

Go:   arr[1:4]
来源：http://cnn.ybcxt.top

Ruby: arr[1, 3]
来源：http://hep.chenzaomai.com

C#:   list.GetRange(1, 3);
来源：http://fgj.jinqigufen.top

[D08] 合并两个数组
来源：http://kmp.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://mqg.ehwqpu.com

PHP:  array_merge($a, $b);
来源：http://uol.jinghuilouyu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vpn.sxryk.cn

TS:   [...a, ...b];
来源：http://hxc.cheryme.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bfu.zhixingplan.top

Go:   append(a, b...)
来源：http://yli.sjlbkw.cn

Ruby: a + b;  a.concat(b)
来源：http://cpt.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://gpn.shanyushiyangtech.top

[D09] 排序（升序）
来源：http://hqr.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://odq.smart0.xyz

PHP:  sort($arr);
来源：http://afd.jinyuanbaomall.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ahv.yj20258888.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://fop.havefunace.top

Java: Collections.sort(list);  list.sort(null);
来源：http://gtr.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ndw.yuanzhike.top

Ruby: arr.sort
来源：http://rjs.cqqwz.cn

C#:   list.Sort();
来源：http://etq.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://has.jqgufenzy.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://his.svipenyu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vmq.svipenyu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tvd.aizwys.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://uoj.yj20258.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dyo.jinyuanbaomall.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ujz.fzhhl.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://edm.jianghu66.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vmt.cdnleiting.top

[D11] 反转数组
来源：http://xcm.jinyuanbaomall.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nzg.ydzc1.top

PHP:  array_reverse($arr);
来源：http://cqx.bjfxy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://and.shanyushiyangtech.top

TS:   [...arr].reverse();
来源：http://qgp.gotoacloud.top

Java: Collections.reverse(list);
来源：http://mwo.316326.xyz

Go:   slices.Reverse(arr)
来源：http://vpv.gogol.net.cn

Ruby: arr.reverse
来源：http://pmc.pycfn.com

C#:   list.Reverse();
来源：http://jsf.meibo888.top

[D12] 查找元素下标
来源：http://zum.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://xxy.zhaomingkeji.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jog.hysaishi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bgj.yj20258.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mhk.xylfe.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oem.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://evt.gzhubu.top

Ruby: arr.index(x)
来源：http://rik.quarkkingdee.top

C#:   list.IndexOf(x);
来源：http://idr.xylfe.cn

[D13] 过滤（保留满足条件的）
来源：http://qnp.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kmo.gogol.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gbm.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://oiz.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://yec.fzhhl.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://djf.jinyuanbaomall.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://prc.hesvh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jed.316326.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://mcp.shuidangran.top

[D14] 映射转换（每个元素变形）
来源：http://ojm.hesvh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://irf.shanyushiyangtech.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fgt.jyoumei.cn

JS:   arr.map(x => x * 2)
来源：http://qsk.nanxinkj.top

TS:   arr.map(x => x * 2)
来源：http://dot.yj202588.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://agx.dashuyun.cn

Go:   // 手写循环
来源：http://nlq.meibo888.top

Ruby: arr.map { |x| x * 2 }
来源：http://tfg.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://hki.tanke756.top

[D15] 去重
来源：http://bvv.ppjwa.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ahe.jinqigfzy.top

PHP:  array_unique($arr);
来源：http://fep.yangfankeji.com

JS:   [...new Set(arr)]
来源：http://ouh.zhiwuduotai.top

TS:   [...new Set(arr)]
来源：http://ynm.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bnz.shuidangran.top

Go:   // 用 map[T]struct{} 手写
来源：http://jgz.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://vpj.zhijiandao.cn

C#:   list.Distinct().ToList()
来源：http://wwx.ydjk.org.cn

[D16] 求和与平均值
来源：http://usf.gaohongyu789.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lvk.svipenyu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://llp.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://esv.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zgi.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kja.daxiang520.top

Go:   // 手写循环累加
来源：http://ecu.fzhhl.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emt.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://jug.chenjidiqi.icu

[D17] 最大值与最小值
来源：http://wcv.wangdashe.top

Py:   max(arr);  min(arr)
来源：http://veg.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://wcr.zhijiandao.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ezw.guowangkeji.top

TS:   Math.max(...arr);
来源：http://nfk.hnxiangtu.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pwa.nanxuanxn.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kic.yuxming.cn

Ruby: arr.max;  arr.min
来源：http://idv.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://jjh.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://dzu.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nqa.redwolf501.top

PHP:  array_merge(...$nested);
来源：http://amf.tanke756.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hfg.vqdsnc.cn

TS:   nested.flat();
来源：http://waa.mhx1999.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cjo.fktsv.cn

Go:   // 手写双层循环
来源：http://pcd.yanxiufei.cn

Ruby: nested.flatten
来源：http://jfv.jlsjyb.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ald.andypj.xyz

[D19] 按字段分组
来源：http://qgl.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://skj.sxryk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nce.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tyn.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://vdt.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wuj.ehwqpu.com

Go:   // 手写 map[string][]T
来源：http://ycg.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ukb.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lyy.chenjidiqi.icu

[D20] 统计每个元素出现次数
来源：http://iwo.shangyingyoupin.top

Py:   Counter(arr)
来源：http://phj.yueranfly.top

PHP:  array_count_values($arr);
来源：http://fzn.jyoumei.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skq.cdnleiting.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zfi.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://glj.xuanzx.com

Go:   // 手写 map[T]int
来源：http://sev.vqdsnc.cn

Ruby: arr.tally
来源：http://kmf.tian-w.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rgy.cashguo.top

[D21] 判断是否包含某元素
来源：http://ilo.hnxiangtu.top

Py:   x in arr
来源：http://dub.aibaodan.cn

PHP:  in_array($x, $arr, true);
来源：http://ffq.fanxiaobao.xyz

JS:   arr.includes(x)
来源：http://qcl.yueranfly.top

TS:   arr.includes(x)
来源：http://wxb.bbcook.cn

Java: list.contains(x)
来源：http://evw.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://oyx.zhengqikj.top

Ruby: arr.include?(x)
来源：http://srw.ydzc1.top

C#:   list.Contains(x)
来源：http://lpa.hesvh.cn

[D22] 复制数组（避免共享引用）
来源：http://sqv.jlsjyb.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gre.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xvu.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://oki.dashuyun.cn

TS:   [...arr];
来源：http://hhg.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://oxn.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://blr.xingfuxueyuan.xyz

Ruby: arr.dup;  arr.clone
来源：http://vqu.jqgufenzy.top

C#:   new List<int>(list);
来源：http://tsx.52xcode.cn

[D23] reduce 累积计算
来源：http://prn.zhixingplan.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mft.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qag.hnqzz.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nkf.meibo888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ibu.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://lxq.jinghuilouyu.cn

Go:   // 手写循环
来源：http://hgr.bbcook.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://smr.iojbl.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gvb.mhx1999.top

[D24] 字典 / Map 基本操作
来源：http://kwu.hnxiangtu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bou.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xyi.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cay.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ivr.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xnv.zhiwuduotai.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dsc.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://klr.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gns.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://mgx.jinqigfzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tqf.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://emf.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vil.wangshuangyany.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cad.cheryme.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yci.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yli.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ldu.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://awb.ppjwa.cn

[D26] 数组转字符串
来源：http://vny.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://abp.guannengcc.top

PHP:  implode(", ", $arr);
来源：http://tvh.xingfuxueyuan.xyz

JS:   arr.join(", ")
来源：http://qqv.ydjk.org.cn

TS:   arr.join(", ")
来源：http://tfx.meibo888.top

Java: String.join(", ", list)
来源：http://jxk.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://uon.shanyushiyangkeji.top

Ruby: arr.join(", ")
来源：http://dim.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://xnk.tanke756.top

================================================================================
来源：http://eom.snrcjt.cn

E. 字符串处理
来源：http://suj.zycfv.cn

================================================================================
来源：http://twb.ydzc1.top

[E01] 拼接字符串
来源：http://ase.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pts.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://opd.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bev.feifeiyinyue.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qnx.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kye.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://chl.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://huz.yuxming.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bir.smart0.xyz

[E02] 重复字符串
来源：http://iun.snrcjt.cn

Py:   "ab" * 3
来源：http://hla.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://qac.smart0.xyz

JS:   "ab".repeat(3)
来源：http://hxb.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://abf.yj202588.top

Java: "ab".repeat(3)
来源：http://sik.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://ztn.zhixingplan.top

Ruby: "ab" * 3
来源：http://pjn.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vrl.shzxlz.cn

[E03] 截取子串
来源：http://wkc.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zxv.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vwz.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ehz.yj202588.top

TS:   s.slice(1, 4)
来源：http://khd.yangfankeji.com

Java: s.substring(1, 4)
来源：http://yaq.jyoumei.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fjs.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://kvf.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://wzp.nanxinkj.top

[E04] 查找子串位置
来源：http://ccs.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://eis.ybcxt.top

PHP:  strpos($s, "x");
来源：http://ubm.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dmc.bbcook.cn

TS:   s.indexOf("x")
来源：http://kzx.dashuyun.cn

Java: s.indexOf("x")
来源：http://yas.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://gwl.ehwqpu.com

Ruby: s.index("x")
来源：http://oah.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://kor.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nfe.yfazqb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vys.epnwcf.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fht.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wlc.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://qxk.xuanzx.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xxo.guannengcc.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kfz.gotoacloud.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dng.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bgv.hnqzz.top

[E06] 替换子串
来源：http://kxj.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dhb.hywenlv.cn

PHP:  str_replace("a", "b", $s);
来源：http://kzs.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mop.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://stq.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edb.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kqd.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xun.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://ndx.yvedp.cn

[E07] 按分隔符拆分
来源：http://jyf.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qog.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gtq.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zpm.hfpthk.cn

TS:   s.split(",")
来源：http://sya.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://llp.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://czk.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://was.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wkp.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://gwr.9152youxi.cn

Py:   ",".join(items)
来源：http://net.andypj.xyz

PHP:  implode(",", $items);
来源：http://xxu.havefunace.top

JS:   items.join(",")
来源：http://tsp.nwbrower.top

TS:   items.join(",")
来源：http://sjb.xziqi.cn

Java: String.join(",", items)
来源：http://xqx.zhengqikj.top

Go:   strings.Join(items, ",")
来源：http://byf.shuidangran.top

Ruby: items.join(",")
来源：http://bde.bjfxy.top

C#:   string.Join(",", items)
来源：http://oha.ctjpmb.com

[E09] 去除所有空白字符
来源：http://pbx.jiagoushi.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://elg.svipenyu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ljt.xinyue.icu

JS:   s.replace(/\s+/g, "")
来源：http://fco.vqdsnc.cn

TS:   s.replace(/\s+/g, "")
来源：http://dyg.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://idg.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://qjk.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iwu.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otx.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://aoi.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wvw.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qos.xuetiantiany.cn

JS:   "7".padStart(3, "0")
来源：http://hcy.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://opi.sweek.top

Java: String.format("%03d", 7)
来源：http://yte.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://skq.dianchejie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fgn.yj20258.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mie.sysykeji.top

[E11] 反转字符串
来源：http://raf.yj202588.top

Py:   s[::-1]
来源：http://bsw.snrcjt.cn

PHP:  strrev($s);
来源：http://bau.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://qup.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://ysx.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aor.52xcode.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zzs.hnxiangtu.top

Ruby: s.reverse
来源：http://smd.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://son.zdbjq.cn

[E12] 统计某字符出现次数
来源：http://wfq.c1oappe.top

Py:   s.count("a")
来源：http://may.yueranfly.top


<!-- 参考信息 -->