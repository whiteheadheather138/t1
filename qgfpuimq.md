代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://edq.hcnkem.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qal.cashguo.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nkr.gotoacloud.top

[D06] 数组长度
来源：http://lko.cdnleiting.top

Py:   len(arr)
来源：http://rix.jinqigufen.top

PHP:  count($arr);
来源：http://aou.gaohongyu789.top

JS:   arr.length
来源：http://mkg.zhongyouzk.top

TS:   arr.length
来源：http://uyh.zhaomingkeji.xyz

Java: list.size();
来源：http://nqb.zhijiandao.cn

Go:   len(arr)
来源：http://hht.yueranfly.top

Ruby: arr.length; arr.size
来源：http://kuy.tanke756.top

C#:   list.Count;
来源：http://squ.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://gfh.zdqjudy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dor.daria6918.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ksb.jinqigufen.top

JS:   arr.slice(1, 4);
来源：http://eck.c1oappe.top

TS:   arr.slice(1, 4);
来源：http://gnn.yj20258888.top

Java: list.subList(1, 4);
来源：http://odb.yvedp.cn

Go:   arr[1:4]
来源：http://bhm.shangyingyoupin.top

Ruby: arr[1, 3]
来源：http://iqb.guannengcc.top

C#:   list.GetRange(1, 3);
来源：http://jpk.vqdsnc.cn

[D08] 合并两个数组
来源：http://gpm.yfazqb.com

Py:   a + b;  a.extend(b)
来源：http://jvp.xziqi.cn

PHP:  array_merge($a, $b);
来源：http://hph.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://way.sufxvd.cn

TS:   [...a, ...b];
来源：http://val.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bsk.ehwqpu.com

Go:   append(a, b...)
来源：http://wta.0kj1m.cn

Ruby: a + b;  a.concat(b)
来源：http://lml.hnxiangtu.top

C#:   a.Concat(b).ToList()
来源：http://arb.jinghuilouyu.cn

[D09] 排序（升序）
来源：http://yha.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://nkx.9152youxi.cn

PHP:  sort($arr);
来源：http://emq.ehwqpu.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gsa.pycfn.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://jnv.jinqigufen.top

Java: Collections.sort(list);  list.sort(null);
来源：http://bjz.svipenyu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://nyr.hnxiangtu.top

Ruby: arr.sort
来源：http://lxb.xuetiantiany.cn

C#:   list.Sort();
来源：http://naa.yfazqb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://kva.hammf.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gii.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://beq.havefunace.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pkj.chenjidiqi.icu

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nsf.hammf.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xhu.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nux.pengpengdd.cyou

Ruby: arr.sort_by { |x| x[:age] }
来源：http://erp.xziqi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fkc.zdqjudy.top

[D11] 反转数组
来源：http://aqb.dashuyun.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xmf.hnqzz.top

PHP:  array_reverse($arr);
来源：http://tbq.xylfe.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ici.daria6918.cn

TS:   [...arr].reverse();
来源：http://pse.haohaochexian.top

Java: Collections.reverse(list);
来源：http://mqs.yuanzhike.top

Go:   slices.Reverse(arr)
来源：http://pib.birdmap.top

Ruby: arr.reverse
来源：http://dyr.xylfe.cn

C#:   list.Reverse();
来源：http://ozj.yj20258.top

[D12] 查找元素下标
来源：http://rrl.redwolf501.top

Py:   arr.index(x);  x in arr
来源：http://ymh.pengpengdd.cyou

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zsc.shuidangran.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cyf.mhx1999.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ycn.tian-w.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hst.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://efh.daxiang520.top

Ruby: arr.index(x)
来源：http://jqn.hcnkem.com

C#:   list.IndexOf(x);
来源：http://tfd.zhiwuduotai.top

[D13] 过滤（保留满足条件的）
来源：http://ska.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://avr.zdbjq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kzg.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://kra.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://pye.shangyingyoupin.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rsa.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mih.ctjpmb.com

Ruby: arr.select { |x| x > 3 }
来源：http://aro.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://phs.kuanghao11.cn

[D14] 映射转换（每个元素变形）
来源：http://yxo.sysykeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fwb.dashuyun.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xro.shuidangran.top

JS:   arr.map(x => x * 2)
来源：http://yre.chenlongwang.top

TS:   arr.map(x => x * 2)
来源：http://dav.guannengcc.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://xth.fzhhl.top

Go:   // 手写循环
来源：http://uyf.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://lua.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://qfv.sweek.top

[D15] 去重
来源：http://xbc.iojbl.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://erg.vehdjk.com

PHP:  array_unique($arr);
来源：http://aux.wangdashe.top

JS:   [...new Set(arr)]
来源：http://dtl.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://pls.zhoulong.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vqk.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://hqp.cheryme.top

Ruby: arr.uniq
来源：http://eel.fengsongda.top

C#:   list.Distinct().ToList()
来源：http://yur.tian-w.cn

[D16] 求和与平均值
来源：http://dzx.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qqv.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rmq.9152youxi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yvx.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ncm.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gph.iojbl.cn

Go:   // 手写循环累加
来源：http://ewh.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rym.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://fdx.zhoulong.xyz

[D17] 最大值与最小值
来源：http://hve.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://apa.yueranfly.top

PHP:  max($arr);  min($arr);
来源：http://fmp.gotoacloud.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fly.smart0.xyz

TS:   Math.max(...arr);
来源：http://lqc.ctjpmb.com

Java: Collections.max(list);  Collections.min(list);
来源：http://kck.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ibh.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://lgv.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://ein.shangyingyoupin.top

[D18] 扁平化嵌套数组
来源：http://fzg.svipenyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yeh.jyoumei.cn

PHP:  array_merge(...$nested);
来源：http://elf.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qok.yfazqb.com

TS:   nested.flat();
来源：http://gfa.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wat.hfpthk.cn

Go:   // 手写双层循环
来源：http://uyx.svipenyu.cn

Ruby: nested.flatten
来源：http://jvo.yj20258888.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://exg.jyoumei.cn

[D19] 按字段分组
来源：http://jeq.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://woo.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmz.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://syk.ctjpmb.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://mba.mhx1999.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nli.9152youxi.cn

Go:   // 手写 map[string][]T
来源：http://hmj.hfpthk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mrq.sweek.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uwc.gotoacloud.top

[D20] 统计每个元素出现次数
来源：http://lyg.xuanzx.com

Py:   Counter(arr)
来源：http://gje.hammf.cn

PHP:  array_count_values($arr);
来源：http://ipp.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tyb.jinqigufen.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rtt.yvedp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fgr.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://bpl.bbcook.cn

Ruby: arr.tally
来源：http://kbf.9152youxi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tpy.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://kfe.yj20258888.top

Py:   x in arr
来源：http://luy.dashuyun.cn

PHP:  in_array($x, $arr, true);
来源：http://pcq.kuanghao11.cn

JS:   arr.includes(x)
来源：http://twp.zhixingplan.top

TS:   arr.includes(x)
来源：http://cik.guannengcc.top

Java: list.contains(x)
来源：http://lmw.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://dsi.jqgfzy.top

Ruby: arr.include?(x)
来源：http://wbi.yj20258.top

C#:   list.Contains(x)
来源：http://rri.guannengcc.top

[D22] 复制数组（避免共享引用）
来源：http://gdo.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xnz.yanxiufei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ofy.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mdm.zhongyouzk.top

TS:   [...arr];
来源：http://aiq.yuanzhike.top

Java: new ArrayList<>(list);
来源：http://jqc.tianlin.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://chs.xziqi.cn

Ruby: arr.dup;  arr.clone
来源：http://cwe.chenzaomai.com

C#:   new List<int>(list);
来源：http://nlv.epnwcf.com

[D23] reduce 累积计算
来源：http://rha.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ujg.316326.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://izd.yangfankeji.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yfy.ehwqpu.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dif.haohaochexian.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://fsh.ydjk.org.cn

Go:   // 手写循环
来源：http://jws.316326.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nqd.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qwz.xingfuxueyuan.xyz

[D24] 字典 / Map 基本操作
来源：http://vcb.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zth.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://iuc.9152youxi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xwb.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oby.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://oib.hesvh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ekl.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sru.jqgfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://otc.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://kpy.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://erv.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eet.yongpay.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sjl.zhoulong.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oqz.svipenyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kmu.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ufo.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xoa.chenjidiqi.icu

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gzi.zhixingplan.top

[D26] 数组转字符串
来源：http://hlm.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://rnc.hnxiangtu.top

PHP:  implode(", ", $arr);
来源：http://cwi.smart0.xyz

JS:   arr.join(", ")
来源：http://qvz.vqdsnc.cn

TS:   arr.join(", ")
来源：http://jzw.zdbjq.cn

Java: String.join(", ", list)
来源：http://bzu.kuanghao11.cn

Go:   strings.Join(strs, ", ")
来源：http://euw.yuanzhike.top

Ruby: arr.join(", ")
来源：http://evr.xylfe.cn

C#:   string.Join(", ", list)
来源：http://jbp.cqqwz.cn

================================================================================
来源：http://jsx.jinqigfzy.top

E. 字符串处理
来源：http://jxl.hysaishi.cn

================================================================================
来源：http://jdc.hcnkem.com

[E01] 拼接字符串
来源：http://aev.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vts.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://reh.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ibs.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cma.jianghu66.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kgy.andypj.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hho.sysykeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oek.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qqo.cucudq.cn

[E02] 重复字符串
来源：http://plm.zhixingplan.top

Py:   "ab" * 3
来源：http://mgy.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://vyu.guannengcc.top

JS:   "ab".repeat(3)
来源：http://nla.hysaishi.cn

TS:   "ab".repeat(3)
来源：http://vxx.jiagoushi.top

Java: "ab".repeat(3)
来源：http://kzc.pycfn.com

Go:   strings.Repeat("ab", 3)
来源：http://khh.zhijiandao.cn

Ruby: "ab" * 3
来源：http://mgg.xingfuxueyuan.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fmd.tianlin.xyz

[E03] 截取子串
来源：http://tcv.smart0.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mey.pycfn.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pzg.aizwys.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://evv.aibaodan.cn

TS:   s.slice(1, 4)
来源：http://aqe.cdnleiting.top

Java: s.substring(1, 4)
来源：http://hlw.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ede.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://bpy.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://srv.yonumen.top

[E04] 查找子串位置
来源：http://fvf.shzxlz.cn

Py:   s.find("x");  s.index("x")
来源：http://jqw.smart0.xyz

PHP:  strpos($s, "x");
来源：http://ahv.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ewb.guowangkeji.top

TS:   s.indexOf("x")
来源：http://mnn.zhixingplan.top

Java: s.indexOf("x")
来源：http://isw.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://oas.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://pgp.fzhhl.top

C#:   s.IndexOf("x")
来源：http://vzp.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ato.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pau.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fmu.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lio.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mfw.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyq.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://auf.zdbjq.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aev.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jmc.hongshengwenyu.top

[E06] 替换子串
来源：http://twc.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gfh.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://rjg.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llg.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://udw.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aje.cucudq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kxr.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wrd.nanxuanxn.top

C#:   s.Replace("a", "b")
来源：http://ndu.sxryk.cn

[E07] 按分隔符拆分
来源：http://eku.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rlz.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vyp.yuxming.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dkj.jyoumei.cn

TS:   s.split(",")
来源：http://ghx.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://ewv.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ahg.jinyuanbaomall.cn

Ruby: s.split(",");  s.split
来源：http://egw.mhx1999.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qxo.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://ozq.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://edo.fktsv.cn

PHP:  implode(",", $items);
来源：http://zmw.xuanzx.com

JS:   items.join(",")
来源：http://pae.jianghu66.top

TS:   items.join(",")
来源：http://gmv.gotoacloud.top

Java: String.join(",", items)
来源：http://zfv.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://tfl.sufxvd.cn

Ruby: items.join(",")
来源：http://nfl.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://aye.cashguo.top

[E09] 去除所有空白字符
来源：http://chz.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oyf.tarul.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vgy.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://shl.xuetiantiany.cn

TS:   s.replace(/\s+/g, "")
来源：http://ruq.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://weq.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vup.xziqi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uri.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://onw.mhx1999.top

[E10] 左侧补零 / 定长填充
来源：http://gao.ydzc1.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tzj.pycfn.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rod.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://xpo.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://stq.nwbrower.top

Java: String.format("%03d", 7)
来源：http://kzg.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tit.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dhh.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://naj.jiagoushi.top

[E11] 反转字符串
来源：http://lee.xingfuxueyuan.xyz

Py:   s[::-1]
来源：http://xik.yonumen.top

PHP:  strrev($s);
来源：http://uts.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://xqk.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://obj.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://sfn.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://aqi.epnwcf.com

Ruby: s.reverse
来源：http://gvv.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://vve.bjfxy.top

[E12] 统计某字符出现次数
来源：http://vzr.sxryk.cn

Py:   s.count("a")
来源：http://xoq.meibo888.top

PHP:  substr_count($s, "a");
来源：http://iaj.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://nvp.tarul.cn

TS:   s.split("a").length - 1
来源：http://uke.316326.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yjo.c1oappe.top


<!-- 参考信息 -->