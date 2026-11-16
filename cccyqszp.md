代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://zip.hnqzz.top

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dyy.snrcjt.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://czz.xingfuxueyuan.xyz

[D06] 数组长度
来源：http://ith.quarkkingdee.top

Py:   len(arr)
来源：http://and.yuanzhike.top

PHP:  count($arr);
来源：http://iky.nanxuanxn.top

JS:   arr.length
来源：http://sgf.chenjidiqi.icu

TS:   arr.length
来源：http://rwm.9152youxi.cn

Java: list.size();
来源：http://pvy.dashuyun.cn

Go:   len(arr)
来源：http://mzg.yangfankeji.com

Ruby: arr.length; arr.size
来源：http://aig.shanyushiyangtech.top

C#:   list.Count;
来源：http://cjr.sufxvd.cn

[D07] 切片 / 取子数组
来源：http://wtx.guowangkeji.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ice.cashguo.top

PHP:  array_slice($arr, 1, 3);
来源：http://ltf.vehdjk.com

JS:   arr.slice(1, 4);
来源：http://fnu.hammf.cn

TS:   arr.slice(1, 4);
来源：http://llx.sweek.top

Java: list.subList(1, 4);
来源：http://cyp.aibaodan.cn

Go:   arr[1:4]
来源：http://zwt.redwolf501.top

Ruby: arr[1, 3]
来源：http://izu.daxiang520.top

C#:   list.GetRange(1, 3);
来源：http://udw.fanxiaobao.xyz

[D08] 合并两个数组
来源：http://mde.pycfn.com

Py:   a + b;  a.extend(b)
来源：http://umd.yj20258.top

PHP:  array_merge($a, $b);
来源：http://brd.hammf.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://izm.cheryme.top

TS:   [...a, ...b];
来源：http://yga.yuxming.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cac.0kj1m.cn

Go:   append(a, b...)
来源：http://pnb.hfpthk.cn

Ruby: a + b;  a.concat(b)
来源：http://rme.jqgufenzy.top

C#:   a.Concat(b).ToList()
来源：http://itj.xinyue.icu

[D09] 排序（升序）
来源：http://udw.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://mwk.cashguo.top

PHP:  sort($arr);
来源：http://jxc.ywan-chungtsiang.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tcm.hcnkem.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://lmb.shanyushiyangtech.top

Java: Collections.sort(list);  list.sort(null);
来源：http://sna.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cid.quarkkingdee.top

Ruby: arr.sort
来源：http://kve.haohaochexian.top

C#:   list.Sort();
来源：http://dsc.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://tjx.yongpay.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://was.shanyushiyangtech.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsk.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nck.tarul.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mty.ydzc1.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ykf.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lmb.zhiwuduotai.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sif.yueranfly.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xey.bbcook.cn

[D11] 反转数组
来源：http://xai.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://fre.c1oappe.top

PHP:  array_reverse($arr);
来源：http://ajh.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pzt.epnwcf.com

TS:   [...arr].reverse();
来源：http://zpu.shzxlz.cn

Java: Collections.reverse(list);
来源：http://smc.cqqwz.cn

Go:   slices.Reverse(arr)
来源：http://cek.ctjpmb.com

Ruby: arr.reverse
来源：http://hrr.cashguo.top

C#:   list.Reverse();
来源：http://mmn.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://xhu.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://rqx.hnqzz.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bgw.aizwys.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fjw.c1oappe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ntb.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kal.yongpay.top

Go:   slices.Index(arr, x)
来源：http://ykx.hnxiangtu.top

Ruby: arr.index(x)
来源：http://brz.yuanzhike.top

C#:   list.IndexOf(x);
来源：http://edf.uphjek.com

[D13] 过滤（保留满足条件的）
来源：http://rhk.jlsjyb.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://igs.wangdashe.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qwt.yj20258.top

JS:   arr.filter(x => x > 3)
来源：http://vwh.chenzaomai.com

TS:   arr.filter(x => x > 3)
来源：http://gmq.aibaodan.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cjp.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mpg.sxryk.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cel.yuxming.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://aim.bbcook.cn

[D14] 映射转换（每个元素变形）
来源：http://wqy.jiagoushi.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sif.jinqigfzy.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ivd.jinqigfzy.top

JS:   arr.map(x => x * 2)
来源：http://msk.yueranfly.top

TS:   arr.map(x => x * 2)
来源：http://kdf.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pxo.xingfuxueyuan.xyz

Go:   // 手写循环
来源：http://oeq.jinyuanbaomall.cn

Ruby: arr.map { |x| x * 2 }
来源：http://svu.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gis.0kj1m.cn

[D15] 去重
来源：http://syc.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://uqx.smart0.xyz

PHP:  array_unique($arr);
来源：http://vdb.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://sre.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://yuc.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mnf.pengpengdd.cyou

Go:   // 用 map[T]struct{} 手写
来源：http://fxu.fehbvm.com

Ruby: arr.uniq
来源：http://hva.ivvv.top

C#:   list.Distinct().ToList()
来源：http://ppe.jyoumei.cn

[D16] 求和与平均值
来源：http://odw.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://aof.haohaochexian.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://stg.zhengqikj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lws.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fpn.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ztb.meibo888.top

Go:   // 手写循环累加
来源：http://hnv.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://abg.chenjidiqi.icu

C#:   list.Sum();  list.Average()
来源：http://nyt.dianchejie.cn

[D17] 最大值与最小值
来源：http://day.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://mth.ydjk.org.cn

PHP:  max($arr);  min($arr);
来源：http://hdu.sxryk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://knf.hcnkem.com

TS:   Math.max(...arr);
来源：http://vbj.316326.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://aos.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vwl.yj202588.top

Ruby: arr.max;  arr.min
来源：http://wce.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://mvk.yuanzhike.top

[D18] 扁平化嵌套数组
来源：http://wfh.yuxming.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vnu.sysykeji.top

PHP:  array_merge(...$nested);
来源：http://fch.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kki.ywan-chungtsiang.top

TS:   nested.flat();
来源：http://lka.chenlongwang.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mjb.ctjpmb.com

Go:   // 手写双层循环
来源：http://nqj.yanxiufei.cn

Ruby: nested.flatten
来源：http://jbu.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xef.ivvv.top

[D19] 按字段分组
来源：http://dro.gotoacloud.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://eta.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dut.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zva.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://jdu.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ryl.jqgfzy.top

Go:   // 手写 map[string][]T
来源：http://oeg.0kj1m.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fww.gaohongyu789.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kls.hesvh.cn

[D20] 统计每个元素出现次数
来源：http://hav.shzxlz.cn

Py:   Counter(arr)
来源：http://izz.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://fci.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kfn.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vmw.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xfm.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://ejy.yongpay.top

Ruby: arr.tally
来源：http://vdo.ybcxt.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uzd.316326.xyz

[D21] 判断是否包含某元素
来源：http://dzv.jinghuilouyu.cn

Py:   x in arr
来源：http://maw.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://mrf.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://err.316326.xyz

TS:   arr.includes(x)
来源：http://uut.vehdjk.com

Java: list.contains(x)
来源：http://enh.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://aec.daria6918.cn

Ruby: arr.include?(x)
来源：http://tcn.pengpengdd.cyou

C#:   list.Contains(x)
来源：http://kyc.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://aqb.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://syd.vehdjk.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjn.sysykeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pju.meibo888.top

TS:   [...arr];
来源：http://vgo.shangyingyoupin.top

Java: new ArrayList<>(list);
来源：http://hdy.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://pcm.cucudq.cn

Ruby: arr.dup;  arr.clone
来源：http://qsf.iojbl.cn

C#:   new List<int>(list);
来源：http://hjf.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://gey.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wps.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ykb.vehdjk.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qud.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dxn.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yzw.tianlin.xyz

Go:   // 手写循环
来源：http://lij.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zvy.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pzp.vqdsnc.cn

[D24] 字典 / Map 基本操作
来源：http://vtn.ivvv.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bor.cqqwz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://scs.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zly.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qkk.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yhq.daria6918.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://avk.zhijiandao.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://crz.vehdjk.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://avf.cdnleiting.top

[D25] Set 集合去重与交并差
来源：http://gue.shuidangran.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dua.quarkkingdee.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cqv.chenjidiqi.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cfe.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jtq.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://srz.epnwcf.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://poq.9152youxi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gfx.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vpb.cqqwz.cn

[D26] 数组转字符串
来源：http://aie.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://xmx.yonumen.top

PHP:  implode(", ", $arr);
来源：http://cli.redwolf501.top

JS:   arr.join(", ")
来源：http://aek.hnqzz.top

TS:   arr.join(", ")
来源：http://wcn.xziqi.cn

Java: String.join(", ", list)
来源：http://lbp.nanxinkj.top

Go:   strings.Join(strs, ", ")
来源：http://sbb.9152youxi.cn

Ruby: arr.join(", ")
来源：http://tqr.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://stu.kuanghao11.cn

================================================================================
来源：http://pye.zhiwuduotai.top

E. 字符串处理
来源：http://ydb.52xcode.cn

================================================================================
来源：http://suc.jyoumei.cn

[E01] 拼接字符串
来源：http://wnf.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oif.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yfq.guannengcc.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://get.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gwa.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vhs.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ghy.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dno.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kyt.hnqzz.top

[E02] 重复字符串
来源：http://phc.jiagoushi.top

Py:   "ab" * 3
来源：http://xqg.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://quj.cashguo.top

JS:   "ab".repeat(3)
来源：http://cxa.andypj.xyz

TS:   "ab".repeat(3)
来源：http://oyn.0kj1m.cn

Java: "ab".repeat(3)
来源：http://jzd.chenjidiqi.icu

Go:   strings.Repeat("ab", 3)
来源：http://khd.bbcook.cn

Ruby: "ab" * 3
来源：http://vbv.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ore.xylfe.cn

[E03] 截取子串
来源：http://jnu.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mzh.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yuc.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hyt.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://awp.mhx1999.top

Java: s.substring(1, 4)
来源：http://uuy.jqgfzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jen.yj20258.top

Ruby: s[1, 3];  s[1..3]
来源：http://aka.andypj.xyz

C#:   s.Substring(1, 3)
来源：http://rjo.ctjpmb.com

[E04] 查找子串位置
来源：http://pfr.zhengqikj.top

Py:   s.find("x");  s.index("x")
来源：http://ilf.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://ccv.meibo888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pnz.wangdashe.top

TS:   s.indexOf("x")
来源：http://ide.wangdashe.top

Java: s.indexOf("x")
来源：http://tca.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://crv.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://wat.yonumen.top

C#:   s.IndexOf("x")
来源：http://mnc.hesvh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqm.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hbz.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pgd.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zct.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tts.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ruf.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zqn.quarkkingdee.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hyy.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rxi.nanxuanxn.top

[E06] 替换子串
来源：http://xhx.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oll.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://jhr.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://okj.zhoulong.xyz

TS:   s.replaceAll("a", "b")
来源：http://nyv.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zpk.9152youxi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hkz.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dec.snrcjt.cn

C#:   s.Replace("a", "b")
来源：http://doz.xuanzx.com

[E07] 按分隔符拆分
来源：http://lii.zhoulong.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cgi.guowangkeji.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hoj.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://qfs.mhx1999.top

TS:   s.split(",")
来源：http://mxo.sxryk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xei.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ovm.sweek.top

Ruby: s.split(",");  s.split
来源：http://bux.sysykeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wce.ydzc1.top

[E08] 数组按分隔符合并
来源：http://eqi.shuidangran.top

Py:   ",".join(items)
来源：http://ynv.vehdjk.com

PHP:  implode(",", $items);
来源：http://bbn.yj20258888.top

JS:   items.join(",")
来源：http://gyu.vehdjk.com

TS:   items.join(",")
来源：http://neb.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://sud.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://nxr.jqgufenzy.top

Ruby: items.join(",")
来源：http://kxh.52xcode.cn

C#:   string.Join(",", items)
来源：http://zhw.hysaishi.cn

[E09] 去除所有空白字符
来源：http://qcx.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mqf.aibaodan.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dqm.zhongyouzk.top

JS:   s.replace(/\s+/g, "")
来源：http://chl.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://edw.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://yug.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mrf.meibo888.top

Ruby: s.gsub(/\s+/, "")
来源：http://mdd.vqdsnc.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tbb.aizwys.cn

[E10] 左侧补零 / 定长填充
来源：http://jyw.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://omu.feifeiyinyue.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ttz.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://jih.zhiwuduotai.top

TS:   "7".padStart(3, "0")
来源：http://rxn.bbcook.cn

Java: String.format("%03d", 7)
来源：http://fat.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ewy.hnqzz.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://omi.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uvn.yuxming.cn

[E11] 反转字符串
来源：http://oax.nwbrower.top

Py:   s[::-1]
来源：http://qmo.daria6918.cn

PHP:  strrev($s);
来源：http://dmr.cashguo.top

JS:   [...s].reverse().join("")
来源：http://uwx.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://rfc.nanxuanxn.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vyp.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fcr.xylfe.cn

Ruby: s.reverse
来源：http://wnj.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://uwn.daxiang520.top

[E12] 统计某字符出现次数
来源：http://wwe.vehdjk.com

Py:   s.count("a")
来源：http://wnr.tanke756.top

PHP:  substr_count($s, "a");
来源：http://wlx.vehdjk.com

JS:   s.split("a").length - 1
来源：http://mhd.c1oappe.top

TS:   s.split("a").length - 1
来源：http://evt.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jmi.zhijiandao.cn


<!-- 参考信息 -->