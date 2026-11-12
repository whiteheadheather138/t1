代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lkn.zhongyouzk.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://llu.shanyushiyangkeji.top

[D05] 访问与修改元素
来源：http://rqo.ydjk.org.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kxy.ydjk.org.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bgb.sjlbkw.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://nkf.quarkkingdee.top

TS:   arr[0]; arr.at(-1);
来源：http://ool.gogol.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://uus.jinqigufen.top

Go:   arr[0]; arr[0] = 9
来源：http://bkw.yueranfly.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://vrn.mhx1999.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eyk.nanxuanxn.top

[D06] 数组长度
来源：http://tfl.ydjk.org.cn

Py:   len(arr)
来源：http://gbz.redwolf501.top

PHP:  count($arr);
来源：http://lrt.xinyue.icu

JS:   arr.length
来源：http://myg.epnwcf.com

TS:   arr.length
来源：http://mwq.xinyue.icu

Java: list.size();
来源：http://imh.yvedp.cn

Go:   len(arr)
来源：http://qmq.shzxlz.cn

Ruby: arr.length; arr.size
来源：http://ztl.dashuyun.cn

C#:   list.Count;
来源：http://kuv.jiagoushi.top

[D07] 切片 / 取子数组
来源：http://yjw.fengsongda.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://daz.xziqi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kie.hcnkem.com

JS:   arr.slice(1, 4);
来源：http://urx.vqdsnc.cn

TS:   arr.slice(1, 4);
来源：http://gdm.sjlbkw.cn

Java: list.subList(1, 4);
来源：http://fdr.vqdsnc.cn

Go:   arr[1:4]
来源：http://fbd.jinqigufen.top

Ruby: arr[1, 3]
来源：http://nsx.tanke756.top

C#:   list.GetRange(1, 3);
来源：http://tmv.jinqigfzy.top

[D08] 合并两个数组
来源：http://dsc.jiagoushi.top

Py:   a + b;  a.extend(b)
来源：http://kzw.hongshengwenyu.top

PHP:  array_merge($a, $b);
来源：http://pwh.bjfxy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://erm.zhoulong.xyz

TS:   [...a, ...b];
来源：http://tiu.yonumen.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kwl.hnqzz.top

Go:   append(a, b...)
来源：http://bue.bjfxy.top

Ruby: a + b;  a.concat(b)
来源：http://gmq.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://jxx.ehwqpu.com

[D09] 排序（升序）
来源：http://cja.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://ano.tarul.cn

PHP:  sort($arr);
来源：http://qvn.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rqg.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://wal.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wyf.ctjpmb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tei.fengsongda.top

Ruby: arr.sort
来源：http://ecl.ppjwa.cn

C#:   list.Sort();
来源：http://hrb.hfpthk.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://gyf.ywan-chungtsiang.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mue.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qij.zhiwuduotai.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xpg.zhaomingkeji.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://tnx.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nvq.haohaochexian.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sxq.hfpthk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dpt.chenlongwang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bor.zhongyouzk.top

[D11] 反转数组
来源：http://snd.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://iev.zycfv.cn

PHP:  array_reverse($arr);
来源：http://ypi.yvedp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://efz.shzxlz.cn

TS:   [...arr].reverse();
来源：http://zmv.fzhhl.top

Java: Collections.reverse(list);
来源：http://ywv.hfpthk.cn

Go:   slices.Reverse(arr)
来源：http://lcb.yuanzhike.top

Ruby: arr.reverse
来源：http://vpv.iojbl.cn

C#:   list.Reverse();
来源：http://pbs.aizwys.cn

[D12] 查找元素下标
来源：http://kyp.jqgufenzy.top

Py:   arr.index(x);  x in arr
来源：http://qes.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tgw.gotoacloud.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vjg.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xnq.sxryk.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jsn.jqgfzy.top

Go:   slices.Index(arr, x)
来源：http://nyv.jinyuanbaomall.cn

Ruby: arr.index(x)
来源：http://ydi.jinqigfzy.top

C#:   list.IndexOf(x);
来源：http://bxg.yuanzhike.top

[D13] 过滤（保留满足条件的）
来源：http://pml.hesvh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qzo.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://woh.ydzc1.top

JS:   arr.filter(x => x > 3)
来源：http://ceq.pengpengdd.cyou

TS:   arr.filter(x => x > 3)
来源：http://usu.iojbl.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tau.guowangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xrx.chenzaomai.com

Ruby: arr.select { |x| x > 3 }
来源：http://quh.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ojb.ivvv.top

[D14] 映射转换（每个元素变形）
来源：http://fby.zhiwuduotai.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://szy.ehwqpu.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://etu.zhixingplan.top

JS:   arr.map(x => x * 2)
来源：http://awb.shanyushiyangkeji.top

TS:   arr.map(x => x * 2)
来源：http://jnq.nanxinkj.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvw.tian-w.cn

Go:   // 手写循环
来源：http://obo.smart0.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://uot.0kj1m.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fmg.fehbvm.com

[D15] 去重
来源：http://wsl.yongpay.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://omc.zhiwuduotai.top

PHP:  array_unique($arr);
来源：http://psi.cheryme.top

JS:   [...new Set(arr)]
来源：http://hbn.aibaodan.cn

TS:   [...new Set(arr)]
来源：http://kyr.xuetiantiany.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://npn.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://oxi.zhoulong.xyz

Ruby: arr.uniq
来源：http://jrl.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://sfb.fengsongda.top

[D16] 求和与平均值
来源：http://iri.ehwqpu.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iny.fanxiaobao.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vts.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://std.kuanghao11.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wdp.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fip.hammf.cn

Go:   // 手写循环累加
来源：http://kmp.pycfn.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qzi.fzhhl.top

C#:   list.Sum();  list.Average()
来源：http://ruf.ydzc1.top

[D17] 最大值与最小值
来源：http://iqx.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://dfk.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://ood.sweek.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sed.aizwys.cn

TS:   Math.max(...arr);
来源：http://ros.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ted.jiagoushi.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ilw.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://tvi.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://agj.zhaomingkeji.xyz

[D18] 扁平化嵌套数组
来源：http://kty.zhongyouzk.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://imv.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://lru.ctjpmb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ani.guannengcc.top

TS:   nested.flat();
来源：http://sas.yj20258888.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zph.yj202588.top

Go:   // 手写双层循环
来源：http://oxp.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://uhx.ydzc1.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vun.jiagoushi.top

[D19] 按字段分组
来源：http://kzz.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kch.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://gsf.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wfn.sysykeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://iom.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://spb.tian-w.cn

Go:   // 手写 map[string][]T
来源：http://jyd.xingfuxueyuan.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://vyf.hfpthk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://khx.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://mvi.yfazqb.com

Py:   Counter(arr)
来源：http://dvn.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://ofp.yangfankeji.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dxo.ydjk.org.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skb.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rub.shzxlz.cn

Go:   // 手写 map[T]int
来源：http://oog.fktsv.cn

Ruby: arr.tally
来源：http://tyx.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fwt.xinyue.icu

[D21] 判断是否包含某元素
来源：http://vvz.fehbvm.com

Py:   x in arr
来源：http://qhl.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://iuo.yuxming.cn

JS:   arr.includes(x)
来源：http://fiq.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://joo.feifeiyinyue.top

Java: list.contains(x)
来源：http://zzd.daxiang520.top

Go:   slices.Contains(arr, x)
来源：http://aqz.gotoacloud.top

Ruby: arr.include?(x)
来源：http://fmq.shuidangran.top

C#:   list.Contains(x)
来源：http://arz.xuetiantiany.cn

[D22] 复制数组（避免共享引用）
来源：http://rsr.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ikd.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hae.yongpay.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rre.gotoacloud.top

TS:   [...arr];
来源：http://uqf.yj20258888.top

Java: new ArrayList<>(list);
来源：http://kab.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jwh.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://iwf.hysaishi.cn

C#:   new List<int>(list);
来源：http://cwr.tian-w.cn

[D23] reduce 累积计算
来源：http://ffe.zhongyouzk.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gji.daria6918.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qfo.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mek.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xyw.hammf.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxx.dianchejie.cn

Go:   // 手写循环
来源：http://qjw.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nzf.redwolf501.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://urg.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://ijm.jlsjyb.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jqw.jianghu66.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kwo.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jkx.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cjz.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bag.epnwcf.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://phl.jiagoushi.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wdt.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qug.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://cpi.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uss.nanxuanxn.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wvx.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uzy.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://umr.zdbjq.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://iqw.xinyue.icu

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zzu.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wdh.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://scr.smart0.xyz

[D26] 数组转字符串
来源：http://zjr.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://zsl.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://wen.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://ifb.gaohongyu789.top

TS:   arr.join(", ")
来源：http://iqx.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://nkz.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://nxr.fzhhl.top

Ruby: arr.join(", ")
来源：http://qov.hcnkem.com

C#:   string.Join(", ", list)
来源：http://sja.snrcjt.cn

================================================================================
来源：http://ljl.haohaochexian.top

E. 字符串处理
来源：http://nls.316326.xyz

================================================================================
来源：http://hba.hysaishi.cn

[E01] 拼接字符串
来源：http://mwc.ydjk.org.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pej.hongshengwenyu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jvf.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nlv.jlsjyb.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tqx.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rqd.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yhb.fengsongda.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cko.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fvc.gaohongyu789.top

[E02] 重复字符串
来源：http://luq.dianchejie.cn

Py:   "ab" * 3
来源：http://bbv.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://thq.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://efw.redwolf501.top

TS:   "ab".repeat(3)
来源：http://uep.gzhubu.top

Java: "ab".repeat(3)
来源：http://cvf.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://hmg.shzxlz.cn

Ruby: "ab" * 3
来源：http://eyu.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://apu.ehwqpu.com

[E03] 截取子串
来源：http://fmd.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qum.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hgy.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tby.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://zmn.316326.xyz

Java: s.substring(1, 4)
来源：http://jaj.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sne.tianlin.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://ygp.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://qtt.pengpengdd.cyou

[E04] 查找子串位置
来源：http://pcr.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://eex.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://tuf.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lvf.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://beh.uphjek.com

Java: s.indexOf("x")
来源：http://utr.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://ojn.vqdsnc.cn

Ruby: s.index("x")
来源：http://wpe.haohaochexian.top

C#:   s.IndexOf("x")
来源：http://iwt.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://efs.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zob.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oui.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iel.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tqs.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wzz.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://odb.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vcg.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hko.0kj1m.cn

[E06] 替换子串
来源：http://nbc.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gdq.hammf.cn

PHP:  str_replace("a", "b", $s);
来源：http://ojl.yuxming.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://brh.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://sss.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://det.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dxq.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://egp.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://wqn.9152youxi.cn

[E07] 按分隔符拆分
来源：http://esj.jiagoushi.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qct.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ikd.gaohongyu789.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xmb.sufxvd.cn

TS:   s.split(",")
来源：http://maf.fzhhl.top

Java: s.split(",");  s.split("\\s+")
来源：http://tgj.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://psf.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://kas.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pko.yj20258.top

[E08] 数组按分隔符合并
来源：http://pdl.birdmap.top

Py:   ",".join(items)
来源：http://jvu.tarul.cn

PHP:  implode(",", $items);
来源：http://hou.hnxiangtu.top

JS:   items.join(",")
来源：http://fwv.yj20258888.top

TS:   items.join(",")
来源：http://vrj.yj20258888.top

Java: String.join(",", items)
来源：http://bqb.yj202588.top

Go:   strings.Join(items, ",")
来源：http://crn.zhongyouzk.top

Ruby: items.join(",")
来源：http://lzo.ppjwa.cn

C#:   string.Join(",", items)
来源：http://efs.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://leb.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://niy.jyoumei.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tdc.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://vvq.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://xto.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://xiw.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zrb.shanyushiyangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://tjk.ppjwa.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nqj.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://mkd.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gdi.andypj.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://any.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://fee.mhx1999.top

TS:   "7".padStart(3, "0")
来源：http://ite.cucudq.cn

Java: String.format("%03d", 7)
来源：http://xzi.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pme.ydzc1.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yxz.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bbi.316326.xyz

[E11] 反转字符串
来源：http://nrx.zhaomingkeji.xyz

Py:   s[::-1]
来源：http://spj.zhiwuduotai.top

PHP:  strrev($s);
来源：http://use.feifeiyinyue.top

JS:   [...s].reverse().join("")
来源：http://wzs.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://yjx.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xdh.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://trc.xinyue.icu


<!-- 参考信息 -->