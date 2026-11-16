代发 wailian999

Py:   len(arr)
来源：http://ofx.tianlin.xyz

PHP:  count($arr);
来源：http://thu.c1oappe.top

JS:   arr.length
来源：http://dkc.zhijiandao.cn

TS:   arr.length
来源：http://rdj.cashguo.top

Java: list.size();
来源：http://xik.sweek.top

Go:   len(arr)
来源：http://zcg.pycfn.com

Ruby: arr.length; arr.size
来源：http://qlu.jinqigufen.top

C#:   list.Count;
来源：http://voo.shanyushiyangtech.top

[D07] 切片 / 取子数组
来源：http://nhv.52xcode.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ohg.cheryme.top

PHP:  array_slice($arr, 1, 3);
来源：http://cgh.cqqwz.cn

JS:   arr.slice(1, 4);
来源：http://hxv.shanyushiyangkeji.top

TS:   arr.slice(1, 4);
来源：http://wgl.jinghuilouyu.cn

Java: list.subList(1, 4);
来源：http://bih.tanke756.top

Go:   arr[1:4]
来源：http://fkm.fanxiaobao.xyz

Ruby: arr[1, 3]
来源：http://fln.yongpay.top

C#:   list.GetRange(1, 3);
来源：http://roi.chenzaomai.com

[D08] 合并两个数组
来源：http://gtw.gogol.net.cn

Py:   a + b;  a.extend(b)
来源：http://hmz.fengsongda.top

PHP:  array_merge($a, $b);
来源：http://rin.hywenlv.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gwh.tianlin.xyz

TS:   [...a, ...b];
来源：http://byf.bjfxy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mfy.shanyushiyangtech.top

Go:   append(a, b...)
来源：http://hpi.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://wyp.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://aqz.shangyingyoupin.top

[D09] 排序（升序）
来源：http://lbn.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://yvq.xuanzx.com

PHP:  sort($arr);
来源：http://enf.pycfn.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zwg.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xfo.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bfl.xingfuxueyuan.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cww.zhiwuduotai.top

Ruby: arr.sort
来源：http://dvp.snrcjt.cn

C#:   list.Sort();
来源：http://suu.hnxiangtu.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uwg.yuanzhike.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gca.hnxiangtu.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qob.cqqwz.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gco.yj202588.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://trt.nanxuanxn.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://opq.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fiq.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yfz.hesvh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tgy.ctjpmb.com

[D11] 反转数组
来源：http://qtk.chenjidiqi.icu

Py:   arr[::-1];  arr.reverse()
来源：http://cid.hesvh.cn

PHP:  array_reverse($arr);
来源：http://fyq.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zhp.c1oappe.top

TS:   [...arr].reverse();
来源：http://dzy.zhiwuduotai.top

Java: Collections.reverse(list);
来源：http://kqx.wangdashe.top

Go:   slices.Reverse(arr)
来源：http://djn.shzxlz.cn

Ruby: arr.reverse
来源：http://pmr.haohaochexian.top

C#:   list.Reverse();
来源：http://kcp.hcnkem.com

[D12] 查找元素下标
来源：http://uqy.nwbrower.top

Py:   arr.index(x);  x in arr
来源：http://mnf.ppjwa.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bqf.vqdsnc.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://esn.xingfuxueyuan.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdz.jqgufenzy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rpo.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://wje.feifeiyinyue.top

Ruby: arr.index(x)
来源：http://dfc.cashguo.top

C#:   list.IndexOf(x);
来源：http://zdg.zhaomingkeji.xyz

[D13] 过滤（保留满足条件的）
来源：http://opb.gzhubu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xlo.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kwj.xingfuxueyuan.xyz

JS:   arr.filter(x => x > 3)
来源：http://bju.xinyue.icu

TS:   arr.filter(x => x > 3)
来源：http://zxp.zhongyouzk.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uxz.xuanzx.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ztc.hywenlv.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vgy.xziqi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sof.fzhhl.top

[D14] 映射转换（每个元素变形）
来源：http://yzj.tianlin.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wko.snrcjt.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oen.vqdsnc.cn

JS:   arr.map(x => x * 2)
来源：http://txq.jianghu66.top

TS:   arr.map(x => x * 2)
来源：http://wmb.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jze.sxryk.cn

Go:   // 手写循环
来源：http://npu.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://ejj.ctjpmb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://kjj.cdnleiting.top

[D15] 去重
来源：http://ncq.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wtx.sysykeji.top

PHP:  array_unique($arr);
来源：http://ioy.zhijiandao.cn

JS:   [...new Set(arr)]
来源：http://cbz.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://lmz.guowangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xfh.snrcjt.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tgz.cheryme.top

Ruby: arr.uniq
来源：http://hag.yj202588.top

C#:   list.Distinct().ToList()
来源：http://ubf.sweek.top

[D16] 求和与平均值
来源：http://gmw.fzhhl.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hoc.ybcxt.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pdr.yj20258888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kpt.hfpthk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pcw.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://coz.smart0.xyz

Go:   // 手写循环累加
来源：http://xbj.hongshengwenyu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dlx.tianlin.xyz

C#:   list.Sum();  list.Average()
来源：http://adp.ehwqpu.com

[D17] 最大值与最小值
来源：http://tmn.yvedp.cn

Py:   max(arr);  min(arr)
来源：http://sal.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://adb.chenzaomai.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sxp.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://piv.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mpb.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fwt.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://udc.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://iic.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://hcg.ywan-chungtsiang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fmu.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://rdl.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vmq.aizwys.cn

TS:   nested.flat();
来源：http://xqq.iojbl.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uwr.nanxuanxn.top

Go:   // 手写双层循环
来源：http://rea.jinqigufen.top

Ruby: nested.flatten
来源：http://yxa.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ojo.hcnkem.com

[D19] 按字段分组
来源：http://gqu.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mnq.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jhu.cucudq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uue.xinyue.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://cxx.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iza.fktsv.cn

Go:   // 手写 map[string][]T
来源：http://fnn.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ngr.bjfxy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://svn.hongshengwenyu.top

[D20] 统计每个元素出现次数
来源：http://gde.0kj1m.cn

Py:   Counter(arr)
来源：http://tsy.chenlongwang.top

PHP:  array_count_values($arr);
来源：http://dmp.shuidangran.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://feg.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://swr.daxiang520.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://nxj.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://jec.tanke756.top

Ruby: arr.tally
来源：http://qyt.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dbo.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://wlk.yangfankeji.com

Py:   x in arr
来源：http://hkf.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://vaj.yj20258.top

JS:   arr.includes(x)
来源：http://rqy.sjlbkw.cn

TS:   arr.includes(x)
来源：http://xrz.hcnkem.com

Java: list.contains(x)
来源：http://gpw.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://qxd.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://rqq.zhongyouzk.top

C#:   list.Contains(x)
来源：http://jpz.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://eyx.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ecd.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://aph.wangshuangyany.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://smu.jianghu66.top

TS:   [...arr];
来源：http://ccz.yangfankeji.com

Java: new ArrayList<>(list);
来源：http://bep.hnqzz.top

Go:   copied := append([]int(nil), arr...)
来源：http://bpm.sufxvd.cn

Ruby: arr.dup;  arr.clone
来源：http://qdb.sufxvd.cn

C#:   new List<int>(list);
来源：http://vzc.tanke756.top

[D23] reduce 累积计算
来源：http://acn.ivvv.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wdq.wangshuangyany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://daf.dashuyun.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://duu.hfpthk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tlh.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://luq.ppjwa.cn

Go:   // 手写循环
来源：http://zsm.xuanzx.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uox.epnwcf.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ies.hcnkem.com

[D24] 字典 / Map 基本操作
来源：http://oul.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aff.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qxw.zdqjudy.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eyi.zdqjudy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wio.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vva.shzxlz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fam.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pae.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vjh.kuanghao11.cn

[D25] Set 集合去重与交并差
来源：http://kkc.uphjek.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jeh.zhongyouzk.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uhw.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qar.gotoacloud.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qus.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zap.fengsongda.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hfc.nanxinkj.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://deb.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bsi.cqqwz.cn

[D26] 数组转字符串
来源：http://kgt.yanxiufei.cn

Py:   ", ".join(map(str, arr))
来源：http://cbr.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://egn.ydzc1.top

JS:   arr.join(", ")
来源：http://vtd.xuetiantiany.cn

TS:   arr.join(", ")
来源：http://akz.jinqigfzy.top

Java: String.join(", ", list)
来源：http://czp.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://oga.tarul.cn

Ruby: arr.join(", ")
来源：http://wfs.havefunace.top

C#:   string.Join(", ", list)
来源：http://aaj.zhongyouzk.top

================================================================================
来源：http://tge.fktsv.cn

E. 字符串处理
来源：http://xca.havefunace.top

================================================================================
来源：http://joc.gotoacloud.top

[E01] 拼接字符串
来源：http://rey.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rxp.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xsr.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ica.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eyx.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pnh.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mgv.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qdp.bjfxy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fdn.redwolf501.top

[E02] 重复字符串
来源：http://ivx.chenlongwang.top

Py:   "ab" * 3
来源：http://joh.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://ovo.shanyushiyangkeji.top

JS:   "ab".repeat(3)
来源：http://wjc.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://rqx.yongpay.top

Java: "ab".repeat(3)
来源：http://rty.uphjek.com

Go:   strings.Repeat("ab", 3)
来源：http://czp.mhx1999.top

Ruby: "ab" * 3
来源：http://bwq.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://grw.jiagoushi.top

[E03] 截取子串
来源：http://lht.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://knq.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://obn.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rxs.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://flb.316326.xyz

Java: s.substring(1, 4)
来源：http://laa.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yug.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jno.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://epg.zhoulong.xyz

[E04] 查找子串位置
来源：http://hgj.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://yur.cheryme.top

PHP:  strpos($s, "x");
来源：http://kdh.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bev.meibo888.top

TS:   s.indexOf("x")
来源：http://nzj.gotoacloud.top

Java: s.indexOf("x")
来源：http://rzv.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://aqg.hnxiangtu.top

Ruby: s.index("x")
来源：http://uuf.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://fnj.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ygk.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jjt.pycfn.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fvn.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bxs.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hqc.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cuy.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rvc.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lzz.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zpz.jinqigfzy.top

[E06] 替换子串
来源：http://kad.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uzy.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://usi.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ewl.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://qff.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnx.zhoulong.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dph.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ftl.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://mbd.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://vjl.ctjpmb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lsg.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mcv.wangdashe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zcw.uphjek.com

TS:   s.split(",")
来源：http://qfg.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dwl.wangdashe.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://odw.ctjpmb.com

Ruby: s.split(",");  s.split
来源：http://frs.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ctx.0kj1m.cn

[E08] 数组按分隔符合并
来源：http://lcn.birdmap.top

Py:   ",".join(items)
来源：http://sbo.mhx1999.top

PHP:  implode(",", $items);
来源：http://uda.0kj1m.cn

JS:   items.join(",")
来源：http://oft.hysaishi.cn

TS:   items.join(",")
来源：http://mbc.yvedp.cn

Java: String.join(",", items)
来源：http://uxx.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://fgk.redwolf501.top

Ruby: items.join(",")
来源：http://fbj.andypj.xyz

C#:   string.Join(",", items)
来源：http://xyj.hongshengwenyu.top

[E09] 去除所有空白字符
来源：http://wop.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qzk.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cuw.nwbrower.top

JS:   s.replace(/\s+/g, "")
来源：http://xel.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://cvz.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://tup.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yha.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://ekb.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yxs.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://cnx.feifeiyinyue.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jjn.mhx1999.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qhf.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://afd.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://coe.316326.xyz

Java: String.format("%03d", 7)
来源：http://wce.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://roc.yonumen.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://drj.xylfe.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kvh.aizwys.cn

[E11] 反转字符串
来源：http://koi.yueranfly.top

Py:   s[::-1]
来源：http://spa.fehbvm.com

PHP:  strrev($s);
来源：http://zxv.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://qlk.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://ufk.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uul.ppjwa.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ygb.redwolf501.top

Ruby: s.reverse
来源：http://xaq.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pmu.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://ndl.smart0.xyz

Py:   s.count("a")
来源：http://cnf.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://mtz.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://cya.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://swf.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://feg.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://ker.cashguo.top

Ruby: s.count("a")
来源：http://rpy.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://kme.wangdashe.top

[E13] 逐字符遍历
来源：http://lpb.guowangkeji.top


<!-- 参考信息 -->