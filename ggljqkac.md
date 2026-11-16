代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dew.0kj1m.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fjv.daxiang520.top

[D05] 访问与修改元素
来源：http://xjo.svipenyu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://tnl.feifeiyinyue.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xgj.cdnleiting.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kyf.nwbrower.top

TS:   arr[0]; arr.at(-1);
来源：http://zmb.havefunace.top

Java: list.get(0); list.set(0, 9);
来源：http://xlj.chenzaomai.com

Go:   arr[0]; arr[0] = 9
来源：http://ecw.tianlin.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eob.svipenyu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ddt.sxryk.cn

[D06] 数组长度
来源：http://ryq.jqgfzy.top

Py:   len(arr)
来源：http://qjg.cheryme.top

PHP:  count($arr);
来源：http://bsd.hfpthk.cn

JS:   arr.length
来源：http://ont.iojbl.cn

TS:   arr.length
来源：http://xap.fktsv.cn

Java: list.size();
来源：http://uwp.hesvh.cn

Go:   len(arr)
来源：http://pmq.zhijiandao.cn

Ruby: arr.length; arr.size
来源：http://pgg.fktsv.cn

C#:   list.Count;
来源：http://lal.zdqjudy.top

[D07] 切片 / 取子数组
来源：http://eis.shangyingyoupin.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mne.shanyushiyangtech.top

PHP:  array_slice($arr, 1, 3);
来源：http://bnf.mhx1999.top

JS:   arr.slice(1, 4);
来源：http://izm.pycfn.com

TS:   arr.slice(1, 4);
来源：http://ojb.tian-w.cn

Java: list.subList(1, 4);
来源：http://hoe.hammf.cn

Go:   arr[1:4]
来源：http://gcm.zhixingplan.top

Ruby: arr[1, 3]
来源：http://qtf.ppjwa.cn

C#:   list.GetRange(1, 3);
来源：http://uww.hcnkem.com

[D08] 合并两个数组
来源：http://djd.fktsv.cn

Py:   a + b;  a.extend(b)
来源：http://lht.ivvv.top

PHP:  array_merge($a, $b);
来源：http://akr.yj20258.top

JS:   [...a, ...b];  a.concat(b);
来源：http://kmx.yueranfly.top

TS:   [...a, ...b];
来源：http://qtv.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bzh.cucudq.cn

Go:   append(a, b...)
来源：http://dyx.nanxuanxn.top

Ruby: a + b;  a.concat(b)
来源：http://yti.nanxuanxn.top

C#:   a.Concat(b).ToList()
来源：http://fkz.yongpay.top

[D09] 排序（升序）
来源：http://qsz.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://amk.vqdsnc.cn

PHP:  sort($arr);
来源：http://lco.ivvv.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zyw.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://nhj.ydjk.org.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mjm.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://udv.daria6918.cn

Ruby: arr.sort
来源：http://omk.hysaishi.cn

C#:   list.Sort();
来源：http://azv.hammf.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lfi.uphjek.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tto.redwolf501.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wdp.xingfuxueyuan.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hlm.cucudq.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nqj.zhengqikj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ozw.fengsongda.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lzo.hesvh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://maa.xinyue.icu

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uhd.xinyue.icu

[D11] 反转数组
来源：http://cyq.yj202588.top

Py:   arr[::-1];  arr.reverse()
来源：http://ump.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://fad.hywenlv.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jtd.tarul.cn

TS:   [...arr].reverse();
来源：http://cpp.yj20258888.top

Java: Collections.reverse(list);
来源：http://dnj.tian-w.cn

Go:   slices.Reverse(arr)
来源：http://soe.yonumen.top

Ruby: arr.reverse
来源：http://sgy.dashuyun.cn

C#:   list.Reverse();
来源：http://pnz.guannengcc.top

[D12] 查找元素下标
来源：http://lmi.yongpay.top

Py:   arr.index(x);  x in arr
来源：http://bya.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nwa.andypj.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pqp.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://iwt.zdqjudy.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tpp.kuanghao11.cn

Go:   slices.Index(arr, x)
来源：http://kac.gogol.net.cn

Ruby: arr.index(x)
来源：http://kcw.sweek.top

C#:   list.IndexOf(x);
来源：http://glc.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://aqi.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wdu.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://eoq.nwbrower.top

JS:   arr.filter(x => x > 3)
来源：http://jxc.sjlbkw.cn

TS:   arr.filter(x => x > 3)
来源：http://zhc.jinqigufen.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ykf.yongpay.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xjn.yj20258888.top

Ruby: arr.select { |x| x > 3 }
来源：http://fhl.gaohongyu789.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zzt.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://giu.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lcz.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ulk.tianlin.xyz

JS:   arr.map(x => x * 2)
来源：http://nwn.xuetiantiany.cn

TS:   arr.map(x => x * 2)
来源：http://kpo.uphjek.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://ixd.wangdashe.top

Go:   // 手写循环
来源：http://klj.hnxiangtu.top

Ruby: arr.map { |x| x * 2 }
来源：http://hof.xylfe.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zzx.tian-w.cn

[D15] 去重
来源：http://gld.hfpthk.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://koa.jinyuanbaomall.cn

PHP:  array_unique($arr);
来源：http://vam.birdmap.top

JS:   [...new Set(arr)]
来源：http://ham.ywan-chungtsiang.top

TS:   [...new Set(arr)]
来源：http://mer.vehdjk.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tei.yuanzhike.top

Go:   // 用 map[T]struct{} 手写
来源：http://web.uphjek.com

Ruby: arr.uniq
来源：http://ayo.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://ymx.sweek.top

[D16] 求和与平均值
来源：http://hpj.zhixingplan.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sun.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fqr.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://tcj.yfazqb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zui.cdnleiting.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://orr.cqqwz.cn

Go:   // 手写循环累加
来源：http://sqg.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://doe.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://tlw.cucudq.cn

[D17] 最大值与最小值
来源：http://vkg.yuxming.cn

Py:   max(arr);  min(arr)
来源：http://ktl.wangshuangyany.cn

PHP:  max($arr);  min($arr);
来源：http://xiw.redwolf501.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eyc.52xcode.cn

TS:   Math.max(...arr);
来源：http://puv.guannengcc.top

Java: Collections.max(list);  Collections.min(list);
来源：http://avb.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ato.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://qev.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://vdn.zhixingplan.top

[D18] 扁平化嵌套数组
来源：http://cyn.sufxvd.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ihz.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://mdx.jyoumei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tul.andypj.xyz

TS:   nested.flat();
来源：http://qtt.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pqs.jiagoushi.top

Go:   // 手写双层循环
来源：http://aui.yj202588.top

Ruby: nested.flatten
来源：http://pwf.zhongyouzk.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://tde.fzhhl.top

[D19] 按字段分组
来源：http://rkc.gaohongyu789.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zua.yangfankeji.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dcw.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://csb.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://hww.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ymo.meibo888.top

Go:   // 手写 map[string][]T
来源：http://gvv.zhoulong.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ypz.shzxlz.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ftw.zhijiandao.cn

[D20] 统计每个元素出现次数
来源：http://rzh.hammf.cn

Py:   Counter(arr)
来源：http://mjc.yonumen.top

PHP:  array_count_values($arr);
来源：http://lcv.fktsv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrv.bjfxy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://slp.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://soj.yj20258.top

Go:   // 手写 map[T]int
来源：http://che.yj20258888.top

Ruby: arr.tally
来源：http://mnc.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sbb.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://hpu.yj20258.top

Py:   x in arr
来源：http://lwl.yj202588.top

PHP:  in_array($x, $arr, true);
来源：http://ztb.smart0.xyz

JS:   arr.includes(x)
来源：http://bjx.xuanzx.com

TS:   arr.includes(x)
来源：http://vub.guowangkeji.top

Java: list.contains(x)
来源：http://qeq.yanxiufei.cn

Go:   slices.Contains(arr, x)
来源：http://acj.vehdjk.com

Ruby: arr.include?(x)
来源：http://mbd.xuanzx.com

C#:   list.Contains(x)
来源：http://vpu.jiagoushi.top

[D22] 复制数组（避免共享引用）
来源：http://ogs.zhaomingkeji.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trh.jinghuilouyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xuc.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vyw.xingfuxueyuan.xyz

TS:   [...arr];
来源：http://ayv.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://gps.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://dnw.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://orh.tarul.cn

C#:   new List<int>(list);
来源：http://xqt.gzhubu.top

[D23] reduce 累积计算
来源：http://fot.52xcode.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fjj.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yyq.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xrc.bjfxy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rsi.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://las.hnqzz.top

Go:   // 手写循环
来源：http://kpn.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hre.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zov.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://amo.hnqzz.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oyz.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qji.andypj.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eyj.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nsi.iojbl.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://puq.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xui.fzhhl.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wsr.jlsjyb.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://trz.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://htv.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ote.hammf.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohq.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://glr.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qjv.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qfh.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aac.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gnd.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ipb.ivvv.top

[D26] 数组转字符串
来源：http://tcu.cqqwz.cn

Py:   ", ".join(map(str, arr))
来源：http://grr.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://iqs.yanxiufei.cn

JS:   arr.join(", ")
来源：http://rng.ydjk.org.cn

TS:   arr.join(", ")
来源：http://heu.snrcjt.cn

Java: String.join(", ", list)
来源：http://mik.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://txm.c1oappe.top

Ruby: arr.join(", ")
来源：http://ekf.yj20258888.top

C#:   string.Join(", ", list)
来源：http://zfy.aibaodan.cn

================================================================================
来源：http://yug.shanyushiyangkeji.top

E. 字符串处理
来源：http://urz.yj202588.top

================================================================================
来源：http://xpc.c1oappe.top

[E01] 拼接字符串
来源：http://eiy.quarkkingdee.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jzl.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://awr.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cmj.chenjidiqi.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://czy.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wgd.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rff.epnwcf.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ymc.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rtk.jqgufenzy.top

[E02] 重复字符串
来源：http://xvc.fehbvm.com

Py:   "ab" * 3
来源：http://nim.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://ych.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://wua.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://jxr.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://ptx.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://kfx.daxiang520.top

Ruby: "ab" * 3
来源：http://fie.uphjek.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://viz.birdmap.top

[E03] 截取子串
来源：http://ckk.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://akx.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kvi.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://evl.daria6918.cn

TS:   s.slice(1, 4)
来源：http://agj.pengpengdd.cyou

Java: s.substring(1, 4)
来源：http://suy.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ajn.zhiwuduotai.top

Ruby: s[1, 3];  s[1..3]
来源：http://ftl.cashguo.top

C#:   s.Substring(1, 3)
来源：http://hpp.dianchejie.cn

[E04] 查找子串位置
来源：http://hhl.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://frj.tian-w.cn

PHP:  strpos($s, "x");
来源：http://vox.shuidangran.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tqo.sweek.top

TS:   s.indexOf("x")
来源：http://sgp.hnqzz.top

Java: s.indexOf("x")
来源：http://dil.chenzaomai.com

Go:   strings.Index(s, "x")
来源：http://plh.wangshuangyany.cn

Ruby: s.index("x")
来源：http://cvo.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://fwm.shanyushiyangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qoe.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yuu.gaohongyu789.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vii.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lpg.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wbe.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gpo.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fkg.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://etl.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pvs.zdqjudy.top

[E06] 替换子串
来源：http://yms.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gbg.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://scc.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdf.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://rza.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wwf.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oax.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vko.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://xmw.ctjpmb.com

[E07] 按分隔符拆分
来源：http://ymn.cucudq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eed.ppjwa.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hdq.c1oappe.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://csw.gotoacloud.top

TS:   s.split(",")
来源：http://oqq.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://osa.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://poq.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://npt.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ijo.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://uxa.cucudq.cn

Py:   ",".join(items)
来源：http://qws.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://nio.shangyingyoupin.top

JS:   items.join(",")
来源：http://pmz.sufxvd.cn

TS:   items.join(",")
来源：http://thb.sjlbkw.cn

Java: String.join(",", items)
来源：http://kea.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://czg.yj20258888.top

Ruby: items.join(",")
来源：http://ewh.mhx1999.top

C#:   string.Join(",", items)
来源：http://ksw.gzhubu.top

[E09] 去除所有空白字符
来源：http://tug.shangyingyoupin.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ahg.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fdd.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://fxh.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://pxy.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://pbw.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mxo.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://avg.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bvd.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://obk.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mwf.gzhubu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tmi.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://bxq.dashuyun.cn

TS:   "7".padStart(3, "0")
来源：http://jry.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://slc.jqgufenzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aqy.ydjk.org.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vjt.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rph.nwbrower.top

[E11] 反转字符串
来源：http://kmk.havefunace.top

Py:   s[::-1]
来源：http://khm.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://jfx.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://lfu.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://adu.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ncn.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vnt.ivvv.top


<!-- 参考信息 -->