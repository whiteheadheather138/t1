代发 wailian999

Java: list.size();
来源：http://ydp.dianchejie.cn

Go:   len(arr)
来源：http://ann.fanxiaobao.xyz

Ruby: arr.length; arr.size
来源：http://rzc.ydzc1.top

C#:   list.Count;
来源：http://lvk.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://kxv.hammf.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qvl.chenzaomai.com

PHP:  array_slice($arr, 1, 3);
来源：http://kfw.wangshuangyany.cn

JS:   arr.slice(1, 4);
来源：http://qck.yanxiufei.cn

TS:   arr.slice(1, 4);
来源：http://kdq.sweek.top

Java: list.subList(1, 4);
来源：http://mzd.yueranfly.top

Go:   arr[1:4]
来源：http://akt.yonumen.top

Ruby: arr[1, 3]
来源：http://pgk.pengpengdd.cyou

C#:   list.GetRange(1, 3);
来源：http://qry.zhaomingkeji.xyz

[D08] 合并两个数组
来源：http://yuw.feifeiyinyue.top

Py:   a + b;  a.extend(b)
来源：http://duu.cqqwz.cn

PHP:  array_merge($a, $b);
来源：http://ndf.sweek.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fcm.hnxiangtu.top

TS:   [...a, ...b];
来源：http://lhj.haohaochexian.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xqc.hnqzz.top

Go:   append(a, b...)
来源：http://fim.jlsjyb.cn

Ruby: a + b;  a.concat(b)
来源：http://cis.pengpengdd.cyou

C#:   a.Concat(b).ToList()
来源：http://dgq.zhongyouzk.top

[D09] 排序（升序）
来源：http://lzi.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://vrp.pycfn.com

PHP:  sort($arr);
来源：http://ves.yonumen.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zbe.aizwys.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gqs.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oci.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rzg.vehdjk.com

Ruby: arr.sort
来源：http://cch.hnxiangtu.top

C#:   list.Sort();
来源：http://ifs.shzxlz.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://rqk.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vhn.gogol.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://unj.fanxiaobao.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hbb.zhoulong.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lrh.hongshengwenyu.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://rom.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hxq.gotoacloud.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gop.shzxlz.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ssn.hfpthk.cn

[D11] 反转数组
来源：http://dif.hywenlv.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wlj.c1oappe.top

PHP:  array_reverse($arr);
来源：http://exf.316326.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vrd.yuanzhike.top

TS:   [...arr].reverse();
来源：http://hww.zhengqikj.top

Java: Collections.reverse(list);
来源：http://tqf.jinghuilouyu.cn

Go:   slices.Reverse(arr)
来源：http://hhq.zhongyouzk.top

Ruby: arr.reverse
来源：http://pnc.smart0.xyz

C#:   list.Reverse();
来源：http://nqu.gaohongyu789.top

[D12] 查找元素下标
来源：http://vlz.haohaochexian.top

Py:   arr.index(x);  x in arr
来源：http://qur.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vjl.havefunace.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikc.zycfv.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mwv.hfpthk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sqr.jiagoushi.top

Go:   slices.Index(arr, x)
来源：http://jsj.wangdashe.top

Ruby: arr.index(x)
来源：http://rmz.dashuyun.cn

C#:   list.IndexOf(x);
来源：http://zky.xinyue.icu

[D13] 过滤（保留满足条件的）
来源：http://xda.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://onr.cheryme.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kxf.xinyue.icu

JS:   arr.filter(x => x > 3)
来源：http://pev.zhongyouzk.top

TS:   arr.filter(x => x > 3)
来源：http://uhl.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pox.meibo888.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kzx.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vac.jiagoushi.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zkl.gzhubu.top

[D14] 映射转换（每个元素变形）
来源：http://ete.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ckw.iojbl.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pyi.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://xge.sweek.top

TS:   arr.map(x => x * 2)
来源：http://epl.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://fpc.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://zhi.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://bdz.cqqwz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xlb.zdqjudy.top

[D15] 去重
来源：http://ial.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rkz.havefunace.top

PHP:  array_unique($arr);
来源：http://gzz.nanxuanxn.top

JS:   [...new Set(arr)]
来源：http://gww.52xcode.cn

TS:   [...new Set(arr)]
来源：http://olg.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pwz.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://gdt.ydzc1.top

Ruby: arr.uniq
来源：http://utk.gaohongyu789.top

C#:   list.Distinct().ToList()
来源：http://fhn.sxryk.cn

[D16] 求和与平均值
来源：http://csm.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ecp.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wmh.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fks.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://cis.52xcode.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://raw.zhijiandao.cn

Go:   // 手写循环累加
来源：http://ptn.tanke756.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hdw.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://ols.bbcook.cn

[D17] 最大值与最小值
来源：http://nkj.316326.xyz

Py:   max(arr);  min(arr)
来源：http://raj.iojbl.cn

PHP:  max($arr);  min($arr);
来源：http://teb.yuanzhike.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wre.jyoumei.cn

TS:   Math.max(...arr);
来源：http://nrp.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://loe.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nyq.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://xat.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://vcl.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://xnr.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ach.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://ozw.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mte.yuanzhike.top

TS:   nested.flat();
来源：http://ejx.cashguo.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://enx.sweek.top

Go:   // 手写双层循环
来源：http://ctu.iojbl.cn

Ruby: nested.flatten
来源：http://gef.zhixingplan.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hll.yuanzhike.top

[D19] 按字段分组
来源：http://fdq.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://exj.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://miy.jiagoushi.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gzm.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://aje.chenlongwang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dpc.birdmap.top

Go:   // 手写 map[string][]T
来源：http://nfu.guannengcc.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://nfo.ivvv.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wlb.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://zpl.vqdsnc.cn

Py:   Counter(arr)
来源：http://fuh.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://qgj.wangdashe.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fla.zhengqikj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vib.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wxx.birdmap.top

Go:   // 手写 map[T]int
来源：http://owo.bjfxy.top

Ruby: arr.tally
来源：http://oss.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ogh.jinyuanbaomall.cn

[D21] 判断是否包含某元素
来源：http://rya.jqgufenzy.top

Py:   x in arr
来源：http://fqw.zhixingplan.top

PHP:  in_array($x, $arr, true);
来源：http://jao.zhengqikj.top

JS:   arr.includes(x)
来源：http://ldt.sxryk.cn

TS:   arr.includes(x)
来源：http://hqh.0kj1m.cn

Java: list.contains(x)
来源：http://otm.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://dbc.smart0.xyz

Ruby: arr.include?(x)
来源：http://dua.ehwqpu.com

C#:   list.Contains(x)
来源：http://rfk.nanxinkj.top

[D22] 复制数组（避免共享引用）
来源：http://wes.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fwp.chenjidiqi.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ohz.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ukr.xziqi.cn

TS:   [...arr];
来源：http://rsr.gotoacloud.top

Java: new ArrayList<>(list);
来源：http://fea.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://mah.hywenlv.cn

Ruby: arr.dup;  arr.clone
来源：http://eqr.daxiang520.top

C#:   new List<int>(list);
来源：http://hqn.cdnleiting.top

[D23] reduce 累积计算
来源：http://kar.hammf.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qkz.ydjk.org.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://eug.52xcode.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nbl.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rso.feifeiyinyue.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qjc.xuanzx.com

Go:   // 手写循环
来源：http://wmj.fktsv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hth.hnqzz.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nlx.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://tku.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qnm.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yqe.shanyushiyangtech.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yox.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pwx.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xth.hfpthk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cqk.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bvb.wangshuangyany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sqr.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://mtx.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wmp.tarul.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bcg.bbcook.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://irp.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zkn.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dsn.jinqigufen.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pcq.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dvf.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jtp.daria6918.cn

[D26] 数组转字符串
来源：http://ddj.jiagoushi.top

Py:   ", ".join(map(str, arr))
来源：http://zif.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://sgl.bbcook.cn

JS:   arr.join(", ")
来源：http://kiq.gaohongyu789.top

TS:   arr.join(", ")
来源：http://kzt.c1oappe.top

Java: String.join(", ", list)
来源：http://mzb.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://tqd.zhengqikj.top

Ruby: arr.join(", ")
来源：http://uex.quarkkingdee.top

C#:   string.Join(", ", list)
来源：http://wva.ivvv.top

================================================================================
来源：http://zps.vehdjk.com

E. 字符串处理
来源：http://hwd.hcnkem.com

================================================================================
来源：http://ydr.feifeiyinyue.top

[E01] 拼接字符串
来源：http://nsg.gzhubu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jac.fengsongda.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mxk.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wom.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fiq.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iun.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bnl.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xmf.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fgc.wangshuangyany.cn

[E02] 重复字符串
来源：http://zgg.hnqzz.top

Py:   "ab" * 3
来源：http://pod.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://dxs.zhixingplan.top

JS:   "ab".repeat(3)
来源：http://cmn.chenzaomai.com

TS:   "ab".repeat(3)
来源：http://jqo.bjfxy.top

Java: "ab".repeat(3)
来源：http://ylz.xuetiantiany.cn

Go:   strings.Repeat("ab", 3)
来源：http://bje.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://vmx.tian-w.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lbk.bbcook.cn

[E03] 截取子串
来源：http://dff.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mxa.cheryme.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://prs.sweek.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xsh.ivvv.top

TS:   s.slice(1, 4)
来源：http://kjy.xuanzx.com

Java: s.substring(1, 4)
来源：http://eco.chenzaomai.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rfz.vehdjk.com

Ruby: s[1, 3];  s[1..3]
来源：http://fxh.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://whm.sxryk.cn

[E04] 查找子串位置
来源：http://ryw.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://zla.andypj.xyz

PHP:  strpos($s, "x");
来源：http://oiu.fengsongda.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gxk.jianghu66.top

TS:   s.indexOf("x")
来源：http://yst.yfazqb.com

Java: s.indexOf("x")
来源：http://ucs.tarul.cn

Go:   strings.Index(s, "x")
来源：http://jni.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://wyz.yuanzhike.top

C#:   s.IndexOf("x")
来源：http://dms.daxiang520.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ofn.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yuq.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vis.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qso.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://eny.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gja.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qje.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vat.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yfl.zhijiandao.cn

[E06] 替换子串
来源：http://vym.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rqv.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://snk.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eib.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://ukx.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bqo.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://guv.chenlongwang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://clt.meibo888.top

C#:   s.Replace("a", "b")
来源：http://hww.mhx1999.top

[E07] 按分隔符拆分
来源：http://tnn.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hjx.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xhq.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://pby.sysykeji.top

TS:   s.split(",")
来源：http://vek.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://wti.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jeo.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://mdv.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nmj.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://kip.shuidangran.top

Py:   ",".join(items)
来源：http://tkd.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://zpr.andypj.xyz

JS:   items.join(",")
来源：http://ldg.jyoumei.cn

TS:   items.join(",")
来源：http://sww.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://tyi.jqgufenzy.top

Go:   strings.Join(items, ",")
来源：http://elx.ybcxt.top

Ruby: items.join(",")
来源：http://itg.hywenlv.cn

C#:   string.Join(",", items)
来源：http://mag.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://exn.havefunace.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yrz.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://msm.pengpengdd.cyou

JS:   s.replace(/\s+/g, "")
来源：http://dwt.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://tsf.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ojj.guowangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sdo.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://fhv.hnxiangtu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bpx.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://tls.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://euj.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vxd.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://jqb.hnxiangtu.top

TS:   "7".padStart(3, "0")
来源：http://dsm.meibo888.top

Java: String.format("%03d", 7)
来源：http://tqj.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://azx.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gnx.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qxd.aibaodan.cn

[E11] 反转字符串
来源：http://omv.daxiang520.top

Py:   s[::-1]
来源：http://ehg.aibaodan.cn

PHP:  strrev($s);
来源：http://aaa.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://xtn.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://wkc.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tkj.jinyuanbaomall.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qfn.pycfn.com

Ruby: s.reverse
来源：http://tio.tianlin.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://flt.yfazqb.com

[E12] 统计某字符出现次数
来源：http://jla.nwbrower.top

Py:   s.count("a")
来源：http://hkn.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://aie.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://gnd.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://pbm.pengpengdd.cyou

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tij.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://epv.svipenyu.cn

Ruby: s.count("a")
来源：http://yxk.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://ylr.redwolf501.top

[E13] 逐字符遍历
来源：http://aco.sweek.top

Py:   for ch in s: print(ch)
来源：http://swt.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cyn.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rqq.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uyz.jyoumei.cn


<!-- 参考信息 -->