代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aky.andypj.xyz

TS:   arr.splice(0, 1);
来源：http://sxg.hnxiangtu.top

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nid.cqqwz.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mgl.bbcook.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mjz.tarul.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zlt.nanxuanxn.top

[D05] 访问与修改元素
来源：http://ffn.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cnu.sysykeji.top

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hbt.gotoacloud.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://osf.gotoacloud.top

TS:   arr[0]; arr.at(-1);
来源：http://nai.iojbl.cn

Java: list.get(0); list.set(0, 9);
来源：http://paw.xuetiantiany.cn

Go:   arr[0]; arr[0] = 9
来源：http://mva.jyoumei.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ots.zhijiandao.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ioh.yangfankeji.com

[D06] 数组长度
来源：http://kqr.dashuyun.cn

Py:   len(arr)
来源：http://efk.havefunace.top

PHP:  count($arr);
来源：http://nnc.uphjek.com

JS:   arr.length
来源：http://iaa.dianchejie.cn

TS:   arr.length
来源：http://euy.ctjpmb.com

Java: list.size();
来源：http://imi.svipenyu.cn

Go:   len(arr)
来源：http://qoo.cqqwz.cn

Ruby: arr.length; arr.size
来源：http://oqk.xuetiantiany.cn

C#:   list.Count;
来源：http://zyb.nanxinkj.top

[D07] 切片 / 取子数组
来源：http://yrz.ydzc1.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ivj.smart0.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://zfn.ydzc1.top

JS:   arr.slice(1, 4);
来源：http://bcd.wangshuangyany.cn

TS:   arr.slice(1, 4);
来源：http://cmu.guowangkeji.top

Java: list.subList(1, 4);
来源：http://jyp.9152youxi.cn

Go:   arr[1:4]
来源：http://ssh.nanxuanxn.top

Ruby: arr[1, 3]
来源：http://lpd.sjlbkw.cn

C#:   list.GetRange(1, 3);
来源：http://dzx.hnqzz.top

[D08] 合并两个数组
来源：http://hjo.zycfv.cn

Py:   a + b;  a.extend(b)
来源：http://goq.tian-w.cn

PHP:  array_merge($a, $b);
来源：http://fpl.ivvv.top

JS:   [...a, ...b];  a.concat(b);
来源：http://sxi.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://ipt.yfazqb.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://juf.bbcook.cn

Go:   append(a, b...)
来源：http://btw.haohaochexian.top

Ruby: a + b;  a.concat(b)
来源：http://jaf.yuxming.cn

C#:   a.Concat(b).ToList()
来源：http://jwy.iojbl.cn

[D09] 排序（升序）
来源：http://gbd.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://xvp.0kj1m.cn

PHP:  sort($arr);
来源：http://ysi.gaohongyu789.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xgb.gzhubu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://sjp.jqgfzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ekf.52xcode.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lwt.jlsjyb.cn

Ruby: arr.sort
来源：http://ipr.jinyuanbaomall.cn

C#:   list.Sort();
来源：http://xqv.vehdjk.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyv.cheryme.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fsa.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vqm.0kj1m.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://fcn.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://muh.zhixingplan.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zqx.fktsv.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://clw.cucudq.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bok.c1oappe.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gvu.hnxiangtu.top

[D11] 反转数组
来源：http://wdj.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qhn.nanxinkj.top

PHP:  array_reverse($arr);
来源：http://ibu.aibaodan.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gdv.ctjpmb.com

TS:   [...arr].reverse();
来源：http://che.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://kps.yuxming.cn

Go:   slices.Reverse(arr)
来源：http://jai.sysykeji.top

Ruby: arr.reverse
来源：http://nuj.jlsjyb.cn

C#:   list.Reverse();
来源：http://hip.chenjidiqi.icu

[D12] 查找元素下标
来源：http://tie.fzhhl.top

Py:   arr.index(x);  x in arr
来源：http://xnm.jyoumei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wkr.hfpthk.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://exi.wangshuangyany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zil.zhoulong.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sdu.iojbl.cn

Go:   slices.Index(arr, x)
来源：http://xlb.jqgufenzy.top

Ruby: arr.index(x)
来源：http://sgx.zhixingplan.top

C#:   list.IndexOf(x);
来源：http://ocd.ctjpmb.com

[D13] 过滤（保留满足条件的）
来源：http://bov.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zvg.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pze.zhixingplan.top

JS:   arr.filter(x => x > 3)
来源：http://kcx.cashguo.top

TS:   arr.filter(x => x > 3)
来源：http://spn.hfpthk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aqr.nanxuanxn.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hlc.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://fhe.wangdashe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ele.tanke756.top

[D14] 映射转换（每个元素变形）
来源：http://nlp.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xkb.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zks.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://mjk.ydzc1.top

TS:   arr.map(x => x * 2)
来源：http://lpj.hesvh.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ggy.yuxming.cn

Go:   // 手写循环
来源：http://fpi.chenlongwang.top

Ruby: arr.map { |x| x * 2 }
来源：http://krf.hysaishi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xpt.cheryme.top

[D15] 去重
来源：http://xpj.wangdashe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vmg.nwbrower.top

PHP:  array_unique($arr);
来源：http://rrl.guowangkeji.top

JS:   [...new Set(arr)]
来源：http://zny.sjlbkw.cn

TS:   [...new Set(arr)]
来源：http://ifa.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ybl.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://ewn.tanke756.top

Ruby: arr.uniq
来源：http://obq.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://tmj.daxiang520.top

[D16] 求和与平均值
来源：http://xcz.guannengcc.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dls.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://evv.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsw.bbcook.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://omz.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uqb.cdnleiting.top

Go:   // 手写循环累加
来源：http://cht.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://znm.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://hdg.yj20258.top

[D17] 最大值与最小值
来源：http://efd.shuidangran.top

Py:   max(arr);  min(arr)
来源：http://hnt.yangfankeji.com

PHP:  max($arr);  min($arr);
来源：http://xdc.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ayz.ydjk.org.cn

TS:   Math.max(...arr);
来源：http://nlj.ybcxt.top

Java: Collections.max(list);  Collections.min(list);
来源：http://iuy.feifeiyinyue.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gor.nwbrower.top

Ruby: arr.max;  arr.min
来源：http://wsp.meibo888.top

C#:   list.Max();  list.Min()
来源：http://ymi.ppjwa.cn

[D18] 扁平化嵌套数组
来源：http://lfq.dianchejie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rsj.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://qgw.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://aia.yonumen.top

TS:   nested.flat();
来源：http://ifw.yfazqb.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://duw.zdbjq.cn

Go:   // 手写双层循环
来源：http://rtc.ctjpmb.com

Ruby: nested.flatten
来源：http://ovv.chenjidiqi.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://pzz.fanxiaobao.xyz

[D19] 按字段分组
来源：http://ffo.xuetiantiany.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://spu.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://uyx.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tii.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://lys.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ago.jqgufenzy.top

Go:   // 手写 map[string][]T
来源：http://jmb.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://rtd.meibo888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gsa.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://ugq.haohaochexian.top

Py:   Counter(arr)
来源：http://ubx.ywan-chungtsiang.top

PHP:  array_count_values($arr);
来源：http://xff.xuanzx.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tld.wangshuangyany.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://veo.cashguo.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://njy.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://dul.zdbjq.cn

Ruby: arr.tally
来源：http://utr.cucudq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lom.yuanzhike.top

[D21] 判断是否包含某元素
来源：http://jhl.dianchejie.cn

Py:   x in arr
来源：http://npi.zdbjq.cn

PHP:  in_array($x, $arr, true);
来源：http://rma.meibo888.top

JS:   arr.includes(x)
来源：http://auh.xziqi.cn

TS:   arr.includes(x)
来源：http://plq.feifeiyinyue.top

Java: list.contains(x)
来源：http://vdv.fehbvm.com

Go:   slices.Contains(arr, x)
来源：http://yxf.jlsjyb.cn

Ruby: arr.include?(x)
来源：http://rvm.chenjidiqi.icu

C#:   list.Contains(x)
来源：http://tgs.meibo888.top

[D22] 复制数组（避免共享引用）
来源：http://ecu.hywenlv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lny.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wtt.zdqjudy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rzq.jinghuilouyu.cn

TS:   [...arr];
来源：http://mch.0kj1m.cn

Java: new ArrayList<>(list);
来源：http://cxj.jinqigfzy.top

Go:   copied := append([]int(nil), arr...)
来源：http://kod.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://vtm.daria6918.cn

C#:   new List<int>(list);
来源：http://ujx.jinqigufen.top

[D23] reduce 累积计算
来源：http://wig.yfazqb.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qao.ppjwa.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cbr.shangyingyoupin.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qwd.chenjidiqi.icu

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sfq.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wmw.guowangkeji.top

Go:   // 手写循环
来源：http://tiv.nanxinkj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qlv.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://elx.shanyushiyangtech.top

[D24] 字典 / Map 基本操作
来源：http://xrh.quarkkingdee.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pyl.fzhhl.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jyi.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xgm.cdnleiting.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://laz.ivvv.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wlm.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rgc.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yja.fktsv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ueh.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://pex.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://giz.gotoacloud.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vda.fengsongda.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ltj.tian-w.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kfk.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jhv.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wih.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://nsl.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hiz.guannengcc.top

[D26] 数组转字符串
来源：http://odb.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://zeg.fktsv.cn

PHP:  implode(", ", $arr);
来源：http://xnt.yanxiufei.cn

JS:   arr.join(", ")
来源：http://tmk.tian-w.cn

TS:   arr.join(", ")
来源：http://rxb.shzxlz.cn

Java: String.join(", ", list)
来源：http://tay.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://doj.gzhubu.top

Ruby: arr.join(", ")
来源：http://czt.fehbvm.com

C#:   string.Join(", ", list)
来源：http://gjq.yongpay.top

================================================================================
来源：http://tgh.gotoacloud.top

E. 字符串处理
来源：http://ckq.kuanghao11.cn

================================================================================
来源：http://jmo.jlsjyb.cn

[E01] 拼接字符串
来源：http://atk.cucudq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ist.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fkd.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jkx.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://thl.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aqm.hongshengwenyu.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xcy.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ijw.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://liq.zhoulong.xyz

[E02] 重复字符串
来源：http://pwj.pycfn.com

Py:   "ab" * 3
来源：http://agl.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://uux.shuidangran.top

JS:   "ab".repeat(3)
来源：http://qbx.pycfn.com

TS:   "ab".repeat(3)
来源：http://mgr.ppjwa.cn

Java: "ab".repeat(3)
来源：http://xaq.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://iym.yj202588.top

Ruby: "ab" * 3
来源：http://swh.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pja.hammf.cn

[E03] 截取子串
来源：http://nvi.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dxh.zdbjq.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hfy.daria6918.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rni.nanxuanxn.top

TS:   s.slice(1, 4)
来源：http://rpx.gotoacloud.top

Java: s.substring(1, 4)
来源：http://okw.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xlw.jianghu66.top

Ruby: s[1, 3];  s[1..3]
来源：http://qpo.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://vyk.zhixingplan.top

[E04] 查找子串位置
来源：http://ksj.hfpthk.cn

Py:   s.find("x");  s.index("x")
来源：http://iyx.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://qcy.zhijiandao.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtc.cashguo.top

TS:   s.indexOf("x")
来源：http://pyg.zycfv.cn

Java: s.indexOf("x")
来源：http://skr.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://jdg.fehbvm.com

Ruby: s.index("x")
来源：http://ksm.tian-w.cn

C#:   s.IndexOf("x")
来源：http://skj.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kow.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mpj.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://huj.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://crn.dianchejie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gmu.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ebu.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ckh.zycfv.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yzj.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mnz.smart0.xyz

[E06] 替换子串
来源：http://xul.tianlin.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://huh.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://pll.hnqzz.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aws.xingfuxueyuan.xyz

TS:   s.replaceAll("a", "b")
来源：http://onz.zhengqikj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zbp.c1oappe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wye.ivvv.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mre.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://iae.yfazqb.com

[E07] 按分隔符拆分
来源：http://zzj.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mcb.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://llu.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bbc.cdnleiting.top

TS:   s.split(",")
来源：http://btb.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://ivz.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://feb.fktsv.cn

Ruby: s.split(",");  s.split
来源：http://ofl.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cro.cucudq.cn

[E08] 数组按分隔符合并
来源：http://kgw.mhx1999.top

Py:   ",".join(items)
来源：http://fio.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://hyn.tanke756.top

JS:   items.join(",")
来源：http://gsl.guannengcc.top

TS:   items.join(",")
来源：http://xif.feifeiyinyue.top

Java: String.join(",", items)
来源：http://gxa.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://gue.cqqwz.cn

Ruby: items.join(",")
来源：http://qdi.uphjek.com

C#:   string.Join(",", items)
来源：http://upa.pycfn.com

[E09] 去除所有空白字符
来源：http://aou.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rkd.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lew.tian-w.cn

JS:   s.replace(/\s+/g, "")
来源：http://jlv.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://ads.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://fee.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jxh.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://cap.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dew.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://mmk.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fbn.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://woh.zdqjudy.top

JS:   "7".padStart(3, "0")
来源：http://deq.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://mty.yvedp.cn

Java: String.format("%03d", 7)
来源：http://qnt.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://yiw.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pnp.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xti.xziqi.cn

[E11] 反转字符串
来源：http://txh.aizwys.cn

Py:   s[::-1]
来源：http://cnx.wangshuangyany.cn

PHP:  strrev($s);
来源：http://pap.0kj1m.cn


<!-- 参考信息 -->