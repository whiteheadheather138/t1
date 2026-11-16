代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xpl.wangdashe.top

TS:   arr.splice(0, 1);
来源：http://wbo.jyoumei.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qgy.smart0.xyz

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://edf.xziqi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jha.nanxuanxn.top

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://krg.jqgufenzy.top

[D05] 访问与修改元素
来源：http://ngp.jlsjyb.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://aoc.hysaishi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bzv.cashguo.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://jcd.zhiwuduotai.top

TS:   arr[0]; arr.at(-1);
来源：http://ovk.yanxiufei.cn

Java: list.get(0); list.set(0, 9);
来源：http://sjn.hnxiangtu.top

Go:   arr[0]; arr[0] = 9
来源：http://wjx.ydjk.org.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ltk.ctjpmb.com

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://zsz.dianchejie.cn

[D06] 数组长度
来源：http://dpk.hfpthk.cn

Py:   len(arr)
来源：http://ebq.chenzaomai.com

PHP:  count($arr);
来源：http://ujp.hesvh.cn

JS:   arr.length
来源：http://jbq.feifeiyinyue.top

TS:   arr.length
来源：http://jbb.jyoumei.cn

Java: list.size();
来源：http://ofg.jinqigfzy.top

Go:   len(arr)
来源：http://jqo.zycfv.cn

Ruby: arr.length; arr.size
来源：http://bvo.tarul.cn

C#:   list.Count;
来源：http://azt.birdmap.top

[D07] 切片 / 取子数组
来源：http://ums.c1oappe.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fxb.meibo888.top

PHP:  array_slice($arr, 1, 3);
来源：http://fjh.gzhubu.top

JS:   arr.slice(1, 4);
来源：http://cyq.daria6918.cn

TS:   arr.slice(1, 4);
来源：http://kwr.gogol.net.cn

Java: list.subList(1, 4);
来源：http://zjy.hammf.cn

Go:   arr[1:4]
来源：http://hll.iojbl.cn

Ruby: arr[1, 3]
来源：http://oze.jinqigufen.top

C#:   list.GetRange(1, 3);
来源：http://sdi.bjfxy.top

[D08] 合并两个数组
来源：http://wal.zhengqikj.top

Py:   a + b;  a.extend(b)
来源：http://yeb.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://knw.mhx1999.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rkz.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://cmw.zdqjudy.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qac.sjlbkw.cn

Go:   append(a, b...)
来源：http://lmp.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://evp.ppjwa.cn

C#:   a.Concat(b).ToList()
来源：http://pqz.ppjwa.cn

[D09] 排序（升序）
来源：http://wiy.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://yww.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://adk.xinyue.icu

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yxv.yonumen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://bnp.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://xyk.nanxinkj.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gvu.tanke756.top

Ruby: arr.sort
来源：http://aod.hammf.cn

C#:   list.Sort();
来源：http://res.guannengcc.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://njg.fktsv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cta.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cxk.tian-w.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://maz.xingfuxueyuan.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dwf.zycfv.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vfe.svipenyu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dfi.316326.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kew.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tia.gaohongyu789.top

[D11] 反转数组
来源：http://mpy.pengpengdd.cyou

Py:   arr[::-1];  arr.reverse()
来源：http://was.hnxiangtu.top

PHP:  array_reverse($arr);
来源：http://sdt.xziqi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://oss.zhongyouzk.top

TS:   [...arr].reverse();
来源：http://tpy.0kj1m.cn

Java: Collections.reverse(list);
来源：http://til.zhixingplan.top

Go:   slices.Reverse(arr)
来源：http://cpv.hfpthk.cn

Ruby: arr.reverse
来源：http://anb.nanxuanxn.top

C#:   list.Reverse();
来源：http://zki.xinyue.icu

[D12] 查找元素下标
来源：http://hrn.shanyushiyangkeji.top

Py:   arr.index(x);  x in arr
来源：http://adt.nanxuanxn.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wme.smart0.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ysn.52xcode.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ama.yongpay.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ayn.wangshuangyany.cn

Go:   slices.Index(arr, x)
来源：http://mhr.52xcode.cn

Ruby: arr.index(x)
来源：http://yag.epnwcf.com

C#:   list.IndexOf(x);
来源：http://lnf.shuidangran.top

[D13] 过滤（保留满足条件的）
来源：http://xpo.gogol.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qqh.hcnkem.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xns.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://dcr.tanke756.top

TS:   arr.filter(x => x > 3)
来源：http://aga.ywan-chungtsiang.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xuw.pengpengdd.cyou

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://psd.feifeiyinyue.top

Ruby: arr.select { |x| x > 3 }
来源：http://bgb.gotoacloud.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ukf.cucudq.cn

[D14] 映射转换（每个元素变形）
来源：http://fuj.wangshuangyany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wfa.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rxv.smart0.xyz

JS:   arr.map(x => x * 2)
来源：http://mkq.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://wme.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://myu.gzhubu.top

Go:   // 手写循环
来源：http://qvw.dashuyun.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sex.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://boo.ppjwa.cn

[D15] 去重
来源：http://rdv.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fxt.ydzc1.top

PHP:  array_unique($arr);
来源：http://qvf.sufxvd.cn

JS:   [...new Set(arr)]
来源：http://iae.dashuyun.cn

TS:   [...new Set(arr)]
来源：http://vbu.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tbk.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xko.hnxiangtu.top

Ruby: arr.uniq
来源：http://lzj.guowangkeji.top

C#:   list.Distinct().ToList()
来源：http://gmx.yongpay.top

[D16] 求和与平均值
来源：http://jge.zhengqikj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jjd.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cmt.zdqjudy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ptv.tian-w.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dwm.yj20258.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qez.yueranfly.top

Go:   // 手写循环累加
来源：http://omn.zhaomingkeji.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eet.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://mnb.ydzc1.top

[D17] 最大值与最小值
来源：http://esf.yj202588.top

Py:   max(arr);  min(arr)
来源：http://tjo.vqdsnc.cn

PHP:  max($arr);  min($arr);
来源：http://msg.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wrm.iojbl.cn

TS:   Math.max(...arr);
来源：http://giy.nwbrower.top

Java: Collections.max(list);  Collections.min(list);
来源：http://tta.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cxe.zdqjudy.top

Ruby: arr.max;  arr.min
来源：http://hwr.hesvh.cn

C#:   list.Max();  list.Min()
来源：http://xxa.feifeiyinyue.top

[D18] 扁平化嵌套数组
来源：http://ntl.316326.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wlh.zdqjudy.top

PHP:  array_merge(...$nested);
来源：http://sov.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rob.vqdsnc.cn

TS:   nested.flat();
来源：http://jex.yangfankeji.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oml.epnwcf.com

Go:   // 手写双层循环
来源：http://bec.yj202588.top

Ruby: nested.flatten
来源：http://xan.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rsj.mhx1999.top

[D19] 按字段分组
来源：http://hut.cqqwz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dzy.zhiwuduotai.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ggm.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://oyc.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fcl.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yvx.hywenlv.cn

Go:   // 手写 map[string][]T
来源：http://nhv.fanxiaobao.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://oru.hammf.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pqf.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://tby.ybcxt.top

Py:   Counter(arr)
来源：http://dzp.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://lzx.316326.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nqe.xuanzx.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lbl.jianghu66.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://arz.fanxiaobao.xyz

Go:   // 手写 map[T]int
来源：http://kga.chenzaomai.com

Ruby: arr.tally
来源：http://kgn.cqqwz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yzj.chenzaomai.com

[D21] 判断是否包含某元素
来源：http://ntn.yj202588.top

Py:   x in arr
来源：http://tmu.cucudq.cn

PHP:  in_array($x, $arr, true);
来源：http://gli.sxryk.cn

JS:   arr.includes(x)
来源：http://gpf.hfpthk.cn

TS:   arr.includes(x)
来源：http://fiw.uphjek.com

Java: list.contains(x)
来源：http://jgm.fengsongda.top

Go:   slices.Contains(arr, x)
来源：http://xgt.cqqwz.cn

Ruby: arr.include?(x)
来源：http://vax.cashguo.top

C#:   list.Contains(x)
来源：http://ang.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://nav.fktsv.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vah.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xxy.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jms.jinqigfzy.top

TS:   [...arr];
来源：http://dck.mhx1999.top

Java: new ArrayList<>(list);
来源：http://wuy.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vee.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://xyl.dianchejie.cn

C#:   new List<int>(list);
来源：http://hhr.hywenlv.cn

[D23] reduce 累积计算
来源：http://ahn.guowangkeji.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wqk.jinyuanbaomall.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kbp.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ihf.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gxq.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oza.yvedp.cn

Go:   // 手写循环
来源：http://pgf.hywenlv.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wyi.uphjek.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nqf.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://eum.feifeiyinyue.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://shk.cucudq.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://izt.ppjwa.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jud.bjfxy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kag.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zoh.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ezo.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hwa.daria6918.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xfn.aibaodan.cn

[D25] Set 集合去重与交并差
来源：http://pjv.dianchejie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jqo.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://arj.xinyue.icu

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cmj.xziqi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ajr.yongpay.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://szk.zhaomingkeji.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://txo.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hve.yongpay.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baa.sysykeji.top

[D26] 数组转字符串
来源：http://ywf.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://vfm.sxryk.cn

PHP:  implode(", ", $arr);
来源：http://bzf.wangdashe.top

JS:   arr.join(", ")
来源：http://fuj.cdnleiting.top

TS:   arr.join(", ")
来源：http://gum.xuanzx.com

Java: String.join(", ", list)
来源：http://tas.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://rxo.sysykeji.top

Ruby: arr.join(", ")
来源：http://dqa.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://usf.shzxlz.cn

================================================================================
来源：http://skc.0kj1m.cn

E. 字符串处理
来源：http://zav.jianghu66.top

================================================================================
来源：http://zca.yangfankeji.com

[E01] 拼接字符串
来源：http://ooj.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bqq.yonumen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wde.yfazqb.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mqw.tian-w.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://otz.yangfankeji.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fmo.meibo888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ecq.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xzt.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bwj.hfpthk.cn

[E02] 重复字符串
来源：http://ryk.jiagoushi.top

Py:   "ab" * 3
来源：http://obu.snrcjt.cn

PHP:  str_repeat("ab", 3);
来源：http://alh.fktsv.cn

JS:   "ab".repeat(3)
来源：http://eiv.ydzc1.top

TS:   "ab".repeat(3)
来源：http://ztr.yvedp.cn

Java: "ab".repeat(3)
来源：http://wvy.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://cgy.xinyue.icu

Ruby: "ab" * 3
来源：http://ixi.ivvv.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cwh.jlsjyb.cn

[E03] 截取子串
来源：http://hqk.hcnkem.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://row.redwolf501.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ial.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zhq.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://uej.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://ugg.dashuyun.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dok.gotoacloud.top

Ruby: s[1, 3];  s[1..3]
来源：http://mga.jinqigfzy.top

C#:   s.Substring(1, 3)
来源：http://iak.hcnkem.com

[E04] 查找子串位置
来源：http://qwf.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://lqc.mhx1999.top

PHP:  strpos($s, "x");
来源：http://jqe.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vdo.cucudq.cn

TS:   s.indexOf("x")
来源：http://ska.dianchejie.cn

Java: s.indexOf("x")
来源：http://iul.nwbrower.top

Go:   strings.Index(s, "x")
来源：http://avh.yvedp.cn

Ruby: s.index("x")
来源：http://vsk.jianghu66.top

C#:   s.IndexOf("x")
来源：http://fft.zdqjudy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lyi.yueranfly.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hvl.ppjwa.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://udv.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjr.pengpengdd.cyou

TS:   s.includes("x");  s.startsWith("a")
来源：http://axg.iojbl.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpo.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tbi.ppjwa.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qxe.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sgx.wangshuangyany.cn

[E06] 替换子串
来源：http://dca.yueranfly.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://grr.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://bja.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://onr.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://oiy.hfpthk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://teg.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kic.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ryu.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://knk.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://gyx.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rmn.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hxn.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ink.yuxming.cn

TS:   s.split(",")
来源：http://quv.xziqi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://guv.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://slo.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://gzz.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yih.andypj.xyz

[E08] 数组按分隔符合并
来源：http://dpb.ydzc1.top

Py:   ",".join(items)
来源：http://kbz.uphjek.com

PHP:  implode(",", $items);
来源：http://ulv.yfazqb.com

JS:   items.join(",")
来源：http://srn.jianghu66.top

TS:   items.join(",")
来源：http://ptk.xuanzx.com

Java: String.join(",", items)
来源：http://fbp.uphjek.com

Go:   strings.Join(items, ",")
来源：http://jsb.hywenlv.cn

Ruby: items.join(",")
来源：http://fpg.daxiang520.top

C#:   string.Join(",", items)
来源：http://rxm.sufxvd.cn

[E09] 去除所有空白字符
来源：http://hpy.smart0.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qcw.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nzi.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://qbu.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://hrr.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://yhq.hesvh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qyx.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ual.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dfw.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://chw.hongshengwenyu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zjs.nanxuanxn.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fbo.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://mga.tianlin.xyz

TS:   "7".padStart(3, "0")
来源：http://pce.316326.xyz

Java: String.format("%03d", 7)
来源：http://ywr.sufxvd.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wdd.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://esf.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ocy.kuanghao11.cn

[E11] 反转字符串
来源：http://hga.0kj1m.cn

Py:   s[::-1]
来源：http://bgk.hnxiangtu.top

PHP:  strrev($s);
来源：http://ish.jiagoushi.top


<!-- 参考信息 -->