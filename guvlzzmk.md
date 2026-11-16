代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://dte.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zkw.hnqzz.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ifw.svipenyu.cn

[D06] 数组长度
来源：http://dod.jqgufenzy.top

Py:   len(arr)
来源：http://fyp.yueranfly.top

PHP:  count($arr);
来源：http://hca.hongshengwenyu.top

JS:   arr.length
来源：http://gkf.snrcjt.cn

TS:   arr.length
来源：http://rgd.sjlbkw.cn

Java: list.size();
来源：http://otb.aizwys.cn

Go:   len(arr)
来源：http://gcn.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://iri.kuanghao11.cn

C#:   list.Count;
来源：http://nqf.gaohongyu789.top

[D07] 切片 / 取子数组
来源：http://fbk.guannengcc.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xgl.pengpengdd.cyou

PHP:  array_slice($arr, 1, 3);
来源：http://zfs.hywenlv.cn

JS:   arr.slice(1, 4);
来源：http://wyy.shangyingyoupin.top

TS:   arr.slice(1, 4);
来源：http://xef.epnwcf.com

Java: list.subList(1, 4);
来源：http://csw.pengpengdd.cyou

Go:   arr[1:4]
来源：http://rop.zhiwuduotai.top

Ruby: arr[1, 3]
来源：http://evb.havefunace.top

C#:   list.GetRange(1, 3);
来源：http://xkw.zhongyouzk.top

[D08] 合并两个数组
来源：http://qad.aizwys.cn

Py:   a + b;  a.extend(b)
来源：http://mcx.hammf.cn

PHP:  array_merge($a, $b);
来源：http://hbw.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://bdo.zhongyouzk.top

TS:   [...a, ...b];
来源：http://yuf.fanxiaobao.xyz

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wpq.ppjwa.cn

Go:   append(a, b...)
来源：http://hbn.cdnleiting.top

Ruby: a + b;  a.concat(b)
来源：http://qkt.ybcxt.top

C#:   a.Concat(b).ToList()
来源：http://dvg.hfpthk.cn

[D09] 排序（升序）
来源：http://pxa.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://vdw.svipenyu.cn

PHP:  sort($arr);
来源：http://epc.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ngf.zycfv.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oal.guowangkeji.top

Java: Collections.sort(list);  list.sort(null);
来源：http://zgt.chenzaomai.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tvb.pengpengdd.cyou

Ruby: arr.sort
来源：http://pia.c1oappe.top

C#:   list.Sort();
来源：http://bbg.fengsongda.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ztt.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jlf.yj20258888.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bkr.ywan-chungtsiang.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fxi.tianlin.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fgq.0kj1m.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qjj.ywan-chungtsiang.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://oyb.gogol.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ltt.zhixingplan.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zxc.cheryme.top

[D11] 反转数组
来源：http://mcr.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://csc.mhx1999.top

PHP:  array_reverse($arr);
来源：http://mmf.wangdashe.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xov.ppjwa.cn

TS:   [...arr].reverse();
来源：http://iua.jinqigufen.top

Java: Collections.reverse(list);
来源：http://hed.zycfv.cn

Go:   slices.Reverse(arr)
来源：http://var.ctjpmb.com

Ruby: arr.reverse
来源：http://jhu.ywan-chungtsiang.top

C#:   list.Reverse();
来源：http://rlu.hammf.cn

[D12] 查找元素下标
来源：http://oue.quarkkingdee.top

Py:   arr.index(x);  x in arr
来源：http://fbv.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zhd.yuxming.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gbc.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gqt.bbcook.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tcl.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://pfz.jqgfzy.top

Ruby: arr.index(x)
来源：http://xcg.feifeiyinyue.top

C#:   list.IndexOf(x);
来源：http://rol.bbcook.cn

[D13] 过滤（保留满足条件的）
来源：http://osv.hnqzz.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cok.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gkt.guannengcc.top

JS:   arr.filter(x => x > 3)
来源：http://qct.ydjk.org.cn

TS:   arr.filter(x => x > 3)
来源：http://kew.hammf.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avb.dashuyun.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://abo.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ilp.sweek.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nft.redwolf501.top

[D14] 映射转换（每个元素变形）
来源：http://oml.wangdashe.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vfl.sjlbkw.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yko.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://pqa.cashguo.top

TS:   arr.map(x => x * 2)
来源：http://lfk.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://yzq.ybcxt.top

Go:   // 手写循环
来源：http://gvr.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tje.xuanzx.com

C#:   list.Select(x => x * 2).ToList()
来源：http://eam.hcnkem.com

[D15] 去重
来源：http://bis.daria6918.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gyq.iojbl.cn

PHP:  array_unique($arr);
来源：http://mhk.gaohongyu789.top

JS:   [...new Set(arr)]
来源：http://vyd.birdmap.top

TS:   [...new Set(arr)]
来源：http://clj.vqdsnc.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fky.bbcook.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dtx.jianghu66.top

Ruby: arr.uniq
来源：http://srm.pycfn.com

C#:   list.Distinct().ToList()
来源：http://zib.sysykeji.top

[D16] 求和与平均值
来源：http://wiq.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fiz.hammf.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xsk.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwb.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yzo.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rte.zhengqikj.top

Go:   // 手写循环累加
来源：http://bbc.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mqk.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://jks.havefunace.top

[D17] 最大值与最小值
来源：http://qqh.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://yim.zhoulong.xyz

PHP:  max($arr);  min($arr);
来源：http://com.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nto.hnxiangtu.top

TS:   Math.max(...arr);
来源：http://qwy.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nqi.yuxming.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iws.yfazqb.com

Ruby: arr.max;  arr.min
来源：http://nwj.epnwcf.com

C#:   list.Max();  list.Min()
来源：http://qlf.shanyushiyangtech.top

[D18] 扁平化嵌套数组
来源：http://dgv.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://aox.gzhubu.top

PHP:  array_merge(...$nested);
来源：http://teg.c1oappe.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hsi.chenlongwang.top

TS:   nested.flat();
来源：http://xkh.uphjek.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://akd.hesvh.cn

Go:   // 手写双层循环
来源：http://rkm.zhixingplan.top

Ruby: nested.flatten
来源：http://wht.birdmap.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nwx.ydjk.org.cn

[D19] 按字段分组
来源：http://fvb.havefunace.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://plc.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tib.cdnleiting.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gnm.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://imt.zdbjq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rka.guannengcc.top

Go:   // 手写 map[string][]T
来源：http://tdo.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqt.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eig.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://szb.bjfxy.top

Py:   Counter(arr)
来源：http://zlv.ydjk.org.cn

PHP:  array_count_values($arr);
来源：http://deu.redwolf501.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jyb.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yqo.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dzj.nanxuanxn.top

Go:   // 手写 map[T]int
来源：http://ukh.daxiang520.top

Ruby: arr.tally
来源：http://gug.mhx1999.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bbu.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://znx.xinyue.icu

Py:   x in arr
来源：http://qhl.bbcook.cn

PHP:  in_array($x, $arr, true);
来源：http://fpa.sweek.top

JS:   arr.includes(x)
来源：http://ulh.tarul.cn

TS:   arr.includes(x)
来源：http://mdu.fzhhl.top

Java: list.contains(x)
来源：http://hwj.shanyushiyangkeji.top

Go:   slices.Contains(arr, x)
来源：http://nfq.redwolf501.top

Ruby: arr.include?(x)
来源：http://mmt.hcnkem.com

C#:   list.Contains(x)
来源：http://bgq.xuanzx.com

[D22] 复制数组（避免共享引用）
来源：http://dcc.ivvv.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://een.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://utw.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://quy.yfazqb.com

TS:   [...arr];
来源：http://cod.cucudq.cn

Java: new ArrayList<>(list);
来源：http://apo.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://bpe.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://hrb.cqqwz.cn

C#:   new List<int>(list);
来源：http://ina.svipenyu.cn

[D23] reduce 累积计算
来源：http://aee.sjlbkw.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yng.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mbg.hywenlv.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpl.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sue.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wyj.yongpay.top

Go:   // 手写循环
来源：http://wwx.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pka.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://myl.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://vhw.zycfv.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://opu.shangyingyoupin.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ijf.hysaishi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://iml.hongshengwenyu.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ztc.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pmq.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lvq.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://msz.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pkl.yuanzhike.top

[D25] Set 集合去重与交并差
来源：http://nes.jiagoushi.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fcq.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xbf.shuidangran.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://iwe.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bar.jinyuanbaomall.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ufn.zycfv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gan.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ofj.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fnz.sxryk.cn

[D26] 数组转字符串
来源：http://vip.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://wsp.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://uoa.cashguo.top

JS:   arr.join(", ")
来源：http://baf.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://nub.iojbl.cn

Java: String.join(", ", list)
来源：http://ijc.yj20258888.top

Go:   strings.Join(strs, ", ")
来源：http://dfr.dianchejie.cn

Ruby: arr.join(", ")
来源：http://fqa.hcnkem.com

C#:   string.Join(", ", list)
来源：http://gby.uphjek.com

================================================================================
来源：http://wtz.cqqwz.cn

E. 字符串处理
来源：http://jfp.hcnkem.com

================================================================================
来源：http://wlx.jqgfzy.top

[E01] 拼接字符串
来源：http://pxz.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bkp.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zlh.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ris.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tbs.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ars.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjp.daria6918.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vth.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://anu.hfpthk.cn

[E02] 重复字符串
来源：http://fzy.pycfn.com

Py:   "ab" * 3
来源：http://qrn.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://vts.tarul.cn

JS:   "ab".repeat(3)
来源：http://yjf.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://rni.jianghu66.top

Java: "ab".repeat(3)
来源：http://abm.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://frt.birdmap.top

Ruby: "ab" * 3
来源：http://rfc.zhijiandao.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lhf.yfazqb.com

[E03] 截取子串
来源：http://bgq.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cbq.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://miq.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ihp.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://xms.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://rph.ehwqpu.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ozq.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://skv.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://uvo.9152youxi.cn

[E04] 查找子串位置
来源：http://eew.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://ist.hywenlv.cn

PHP:  strpos($s, "x");
来源：http://bdm.yuxming.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blv.shanyushiyangkeji.top

TS:   s.indexOf("x")
来源：http://ubv.jinqigfzy.top

Java: s.indexOf("x")
来源：http://xfd.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://bqz.fktsv.cn

Ruby: s.index("x")
来源：http://pwl.daxiang520.top

C#:   s.IndexOf("x")
来源：http://yls.xingfuxueyuan.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://vzy.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bzi.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://izx.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aqf.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qtv.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ext.yj202588.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yor.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gbm.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fml.cheryme.top

[E06] 替换子串
来源：http://ojg.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://diw.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://ged.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mfq.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://kop.dashuyun.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rwg.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bsc.birdmap.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fab.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://qgl.hysaishi.cn

[E07] 按分隔符拆分
来源：http://vif.mhx1999.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zyv.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zur.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://hus.xuetiantiany.cn

TS:   s.split(",")
来源：http://rci.ppjwa.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mio.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jxu.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://pge.redwolf501.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jjq.iojbl.cn

[E08] 数组按分隔符合并
来源：http://iyh.zycfv.cn

Py:   ",".join(items)
来源：http://ijs.meibo888.top

PHP:  implode(",", $items);
来源：http://yyd.tarul.cn

JS:   items.join(",")
来源：http://cdv.pycfn.com

TS:   items.join(",")
来源：http://qtp.jqgfzy.top

Java: String.join(",", items)
来源：http://iai.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://bgi.jqgfzy.top

Ruby: items.join(",")
来源：http://zge.hysaishi.cn

C#:   string.Join(",", items)
来源：http://azv.fehbvm.com

[E09] 去除所有空白字符
来源：http://edt.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nnk.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hih.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://ccz.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://tpo.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://sxj.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eel.hcnkem.com

Ruby: s.gsub(/\s+/, "")
来源：http://xza.cheryme.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zbl.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ykx.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fnq.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kqx.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://bso.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://gvz.bjfxy.top

Java: String.format("%03d", 7)
来源：http://ama.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mni.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ztg.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kvt.smart0.xyz

[E11] 反转字符串
来源：http://mfh.c1oappe.top

Py:   s[::-1]
来源：http://jet.andypj.xyz

PHP:  strrev($s);
来源：http://iym.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://ygo.fehbvm.com

TS:   [...s].reverse().join("")
来源：http://tsu.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lve.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kmi.jinghuilouyu.cn

Ruby: s.reverse
来源：http://ogc.tanke756.top

C#:   new string(s.Reverse().ToArray())
来源：http://xzp.bjfxy.top

[E12] 统计某字符出现次数
来源：http://rub.zhiwuduotai.top

Py:   s.count("a")
来源：http://wap.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://oke.fehbvm.com

JS:   s.split("a").length - 1
来源：http://onv.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://obw.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://urr.nanxinkj.top


<!-- 参考信息 -->