代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://bco.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://uge.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zeu.uphjek.com

[D06] 数组长度
来源：http://nwc.hnqzz.top

Py:   len(arr)
来源：http://qca.hongshengwenyu.top

PHP:  count($arr);
来源：http://nsb.tianlin.xyz

JS:   arr.length
来源：http://xxr.guannengcc.top

TS:   arr.length
来源：http://htb.316326.xyz

Java: list.size();
来源：http://pfr.aizwys.cn

Go:   len(arr)
来源：http://vxx.yanxiufei.cn

Ruby: arr.length; arr.size
来源：http://xsf.gzhubu.top

C#:   list.Count;
来源：http://yxz.52xcode.cn

[D07] 切片 / 取子数组
来源：http://sor.chenjidiqi.icu

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://clx.zhaomingkeji.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://iso.fengsongda.top

JS:   arr.slice(1, 4);
来源：http://zqn.jinqigufen.top

TS:   arr.slice(1, 4);
来源：http://hcv.nanxuanxn.top

Java: list.subList(1, 4);
来源：http://flf.hnxiangtu.top

Go:   arr[1:4]
来源：http://prw.0kj1m.cn

Ruby: arr[1, 3]
来源：http://mlf.cdnleiting.top

C#:   list.GetRange(1, 3);
来源：http://hif.zhiwuduotai.top

[D08] 合并两个数组
来源：http://nzf.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://avc.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://tsa.zdqjudy.top

JS:   [...a, ...b];  a.concat(b);
来源：http://fde.sufxvd.cn

TS:   [...a, ...b];
来源：http://pjk.hywenlv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ilm.yj202588.top

Go:   append(a, b...)
来源：http://kvd.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://ipj.kuanghao11.cn

C#:   a.Concat(b).ToList()
来源：http://ust.zhengqikj.top

[D09] 排序（升序）
来源：http://kia.jinqigufen.top

Py:   sorted(arr);  arr.sort()
来源：http://umu.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://quy.guowangkeji.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://esi.xylfe.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vmm.jyoumei.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ziz.zhijiandao.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://txa.yuxming.cn

Ruby: arr.sort
来源：http://juu.birdmap.top

C#:   list.Sort();
来源：http://qhq.yj202588.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gzc.yvedp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nbb.dashuyun.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://btq.316326.xyz

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pls.nanxinkj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nks.hywenlv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xbp.yj20258888.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bjv.shanyushiyangkeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qdy.hnxiangtu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ane.dashuyun.cn

[D11] 反转数组
来源：http://awt.jyoumei.cn

Py:   arr[::-1];  arr.reverse()
来源：http://huv.jiagoushi.top

PHP:  array_reverse($arr);
来源：http://lzp.gaohongyu789.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gmp.dashuyun.cn

TS:   [...arr].reverse();
来源：http://fpl.cdnleiting.top

Java: Collections.reverse(list);
来源：http://sgp.yj20258888.top

Go:   slices.Reverse(arr)
来源：http://eon.hywenlv.cn

Ruby: arr.reverse
来源：http://drn.cheryme.top

C#:   list.Reverse();
来源：http://oua.yueranfly.top

[D12] 查找元素下标
来源：http://ihl.gzhubu.top

Py:   arr.index(x);  x in arr
来源：http://iyy.andypj.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iey.zhiwuduotai.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vtr.chenlongwang.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cqh.jyoumei.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://izg.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://ccd.jlsjyb.cn

Ruby: arr.index(x)
来源：http://upr.gaohongyu789.top

C#:   list.IndexOf(x);
来源：http://wjp.hnxiangtu.top

[D13] 过滤（保留满足条件的）
来源：http://beu.yfazqb.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://isn.sxryk.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vzc.epnwcf.com

JS:   arr.filter(x => x > 3)
来源：http://utb.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://kps.yanxiufei.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://vrq.hywenlv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wwl.gogol.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tke.mhx1999.top

C#:   list.Where(x => x > 3).ToList()
来源：http://hoh.vehdjk.com

[D14] 映射转换（每个元素变形）
来源：http://qjp.tanke756.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://osw.mhx1999.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pji.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://qdx.hfpthk.cn

TS:   arr.map(x => x * 2)
来源：http://fve.shanyushiyangkeji.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://bfo.jinyuanbaomall.cn

Go:   // 手写循环
来源：http://cue.daria6918.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bbk.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gii.yuanzhike.top

[D15] 去重
来源：http://gee.jinyuanbaomall.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://prr.zdbjq.cn

PHP:  array_unique($arr);
来源：http://rub.zhixingplan.top

JS:   [...new Set(arr)]
来源：http://szw.zycfv.cn

TS:   [...new Set(arr)]
来源：http://qty.hfpthk.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qxt.epnwcf.com

Go:   // 用 map[T]struct{} 手写
来源：http://zgt.jinqigfzy.top

Ruby: arr.uniq
来源：http://ocr.smart0.xyz

C#:   list.Distinct().ToList()
来源：http://ufb.smart0.xyz

[D16] 求和与平均值
来源：http://dbr.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ufe.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pjv.tarul.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fzu.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gti.xylfe.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://odo.zhengqikj.top

Go:   // 手写循环累加
来源：http://oyz.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mth.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://zod.zdbjq.cn

[D17] 最大值与最小值
来源：http://azx.yfazqb.com

Py:   max(arr);  min(arr)
来源：http://byg.jqgfzy.top

PHP:  max($arr);  min($arr);
来源：http://zlg.fehbvm.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vmo.jqgufenzy.top

TS:   Math.max(...arr);
来源：http://bqi.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://odd.wangdashe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xgc.pycfn.com

Ruby: arr.max;  arr.min
来源：http://vji.yuxming.cn

C#:   list.Max();  list.Min()
来源：http://hby.gogol.net.cn

[D18] 扁平化嵌套数组
来源：http://pmz.jinghuilouyu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bcu.shangyingyoupin.top

PHP:  array_merge(...$nested);
来源：http://fgx.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://etw.ivvv.top

TS:   nested.flat();
来源：http://vtt.ctjpmb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ute.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://ueg.ywan-chungtsiang.top

Ruby: nested.flatten
来源：http://iwl.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ihm.yj20258888.top

[D19] 按字段分组
来源：http://ayr.chenzaomai.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fco.52xcode.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mcc.cheryme.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dyc.sjlbkw.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uij.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rvm.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://nnn.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cca.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qya.guowangkeji.top

[D20] 统计每个元素出现次数
来源：http://jjm.ppjwa.cn

Py:   Counter(arr)
来源：http://sqz.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://atl.ywan-chungtsiang.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ysj.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tre.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tlm.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://sdd.hongshengwenyu.top

Ruby: arr.tally
来源：http://kob.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eao.yj202588.top

[D21] 判断是否包含某元素
来源：http://hdc.tian-w.cn

Py:   x in arr
来源：http://gkl.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://omb.zhoulong.xyz

JS:   arr.includes(x)
来源：http://hrz.yj202588.top

TS:   arr.includes(x)
来源：http://hrb.quarkkingdee.top

Java: list.contains(x)
来源：http://glg.cdnleiting.top

Go:   slices.Contains(arr, x)
来源：http://gzr.jinqigfzy.top

Ruby: arr.include?(x)
来源：http://cjo.gotoacloud.top

C#:   list.Contains(x)
来源：http://wym.guowangkeji.top

[D22] 复制数组（避免共享引用）
来源：http://sog.yueranfly.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hgw.dianchejie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://trl.zhoulong.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://akn.zhongyouzk.top

TS:   [...arr];
来源：http://fof.sxryk.cn

Java: new ArrayList<>(list);
来源：http://ppw.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://upv.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://jgv.hnxiangtu.top

C#:   new List<int>(list);
来源：http://gxk.yonumen.top

[D23] reduce 累积计算
来源：http://xei.zhijiandao.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fof.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tnt.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://stk.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pas.chenlongwang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gcg.guowangkeji.top

Go:   // 手写循环
来源：http://nfu.xinyue.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://enn.hywenlv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jha.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://bxl.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jdh.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://thg.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://llz.hfpthk.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ifm.vehdjk.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xic.0kj1m.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wyz.jinyuanbaomall.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lem.tian-w.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rcb.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://vvd.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qpi.yueranfly.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lph.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eib.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fkg.yangfankeji.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zxm.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sfu.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wug.smart0.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hxx.sysykeji.top

[D26] 数组转字符串
来源：http://zdz.0kj1m.cn

Py:   ", ".join(map(str, arr))
来源：http://gxs.9152youxi.cn

PHP:  implode(", ", $arr);
来源：http://dzm.tianlin.xyz

JS:   arr.join(", ")
来源：http://ivj.quarkkingdee.top

TS:   arr.join(", ")
来源：http://izw.nwbrower.top

Java: String.join(", ", list)
来源：http://dnr.hesvh.cn

Go:   strings.Join(strs, ", ")
来源：http://nuu.yj20258.top

Ruby: arr.join(", ")
来源：http://gju.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://rux.cheryme.top

================================================================================
来源：http://yun.ydzc1.top

E. 字符串处理
来源：http://aot.ywan-chungtsiang.top

================================================================================
来源：http://sxv.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://ebu.tianlin.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://elc.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xcv.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfk.vehdjk.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vjk.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fpo.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jhd.yuanzhike.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://csn.yvedp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wdm.birdmap.top

[E02] 重复字符串
来源：http://wqg.xylfe.cn

Py:   "ab" * 3
来源：http://rms.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://eng.xuanzx.com

JS:   "ab".repeat(3)
来源：http://ejm.wangdashe.top

TS:   "ab".repeat(3)
来源：http://kwp.yanxiufei.cn

Java: "ab".repeat(3)
来源：http://aqn.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://qrp.bjfxy.top

Ruby: "ab" * 3
来源：http://mev.iojbl.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://eil.guowangkeji.top

[E03] 截取子串
来源：http://jia.mhx1999.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yrx.fehbvm.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sno.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kvh.yj20258.top

TS:   s.slice(1, 4)
来源：http://oxv.jqgfzy.top

Java: s.substring(1, 4)
来源：http://cyn.shangyingyoupin.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rgd.xylfe.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hpd.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://snv.shanyushiyangtech.top

[E04] 查找子串位置
来源：http://ave.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://wod.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://srp.dashuyun.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ybz.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://bex.gaohongyu789.top

Java: s.indexOf("x")
来源：http://vty.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://vvp.ehwqpu.com

Ruby: s.index("x")
来源：http://rty.nwbrower.top

C#:   s.IndexOf("x")
来源：http://yix.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://dmr.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ouh.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://afr.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ene.zhongyouzk.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cji.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dyv.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://txv.9152youxi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://syf.dianchejie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zxy.ivvv.top

[E06] 替换子串
来源：http://mpj.shanyushiyangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aeg.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://hsi.xuanzx.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vtq.ydzc1.top

TS:   s.replaceAll("a", "b")
来源：http://gmn.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kda.shzxlz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kzf.yj202588.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://svd.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://arx.cqqwz.cn

[E07] 按分隔符拆分
来源：http://pgg.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sag.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vsh.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wwe.xylfe.cn

TS:   s.split(",")
来源：http://pil.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://aij.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jxk.nanxuanxn.top

Ruby: s.split(",");  s.split
来源：http://vlz.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gom.ivvv.top

[E08] 数组按分隔符合并
来源：http://inl.ehwqpu.com

Py:   ",".join(items)
来源：http://fyc.hnqzz.top

PHP:  implode(",", $items);
来源：http://rng.hnqzz.top

JS:   items.join(",")
来源：http://nlt.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://frl.ctjpmb.com

Java: String.join(",", items)
来源：http://ouj.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://epi.chenjidiqi.icu

Ruby: items.join(",")
来源：http://asn.hnqzz.top

C#:   string.Join(",", items)
来源：http://csd.guowangkeji.top

[E09] 去除所有空白字符
来源：http://hif.chenlongwang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tio.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nli.ehwqpu.com

JS:   s.replace(/\s+/g, "")
来源：http://ymd.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://bxz.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://gpy.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ujr.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://tfw.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jsp.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://coi.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zso.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pkk.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://ami.daria6918.cn

TS:   "7".padStart(3, "0")
来源：http://sph.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://ouj.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zxr.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qko.zhongyouzk.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qas.fktsv.cn

[E11] 反转字符串
来源：http://ojg.vqdsnc.cn

Py:   s[::-1]
来源：http://umd.hesvh.cn

PHP:  strrev($s);
来源：http://use.jinyuanbaomall.cn

JS:   [...s].reverse().join("")
来源：http://afa.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://dav.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://hlq.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xjd.jinghuilouyu.cn

Ruby: s.reverse
来源：http://fge.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hba.birdmap.top

[E12] 统计某字符出现次数
来源：http://saq.yj20258.top

Py:   s.count("a")
来源：http://kfq.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://bdz.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://wtv.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://utu.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ehi.cheryme.top


<!-- 参考信息 -->