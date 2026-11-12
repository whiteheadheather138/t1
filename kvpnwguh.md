代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wcn.jyoumei.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://suq.ctjpmb.com

[D05] 访问与修改元素
来源：http://yot.yangfankeji.com

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hsl.svipenyu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yse.yangfankeji.com

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aus.ehwqpu.com

TS:   arr[0]; arr.at(-1);
来源：http://tpl.yfazqb.com

Java: list.get(0); list.set(0, 9);
来源：http://jdp.yangfankeji.com

Go:   arr[0]; arr[0] = 9
来源：http://kwe.fanxiaobao.xyz

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qfy.yanxiufei.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mvh.mhx1999.top

[D06] 数组长度
来源：http://otv.wangdashe.top

Py:   len(arr)
来源：http://zte.jlsjyb.cn

PHP:  count($arr);
来源：http://wff.chenlongwang.top

JS:   arr.length
来源：http://awm.quarkkingdee.top

TS:   arr.length
来源：http://slq.yuxming.cn

Java: list.size();
来源：http://pap.chenlongwang.top

Go:   len(arr)
来源：http://eko.xziqi.cn

Ruby: arr.length; arr.size
来源：http://rnb.dianchejie.cn

C#:   list.Count;
来源：http://nci.hammf.cn

[D07] 切片 / 取子数组
来源：http://mfh.jinqigfzy.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fyj.chenlongwang.top

PHP:  array_slice($arr, 1, 3);
来源：http://csg.zhongyouzk.top

JS:   arr.slice(1, 4);
来源：http://lui.feifeiyinyue.top

TS:   arr.slice(1, 4);
来源：http://pxs.nanxinkj.top

Java: list.subList(1, 4);
来源：http://ttw.ehwqpu.com

Go:   arr[1:4]
来源：http://iik.bjfxy.top

Ruby: arr[1, 3]
来源：http://fgz.vehdjk.com

C#:   list.GetRange(1, 3);
来源：http://caf.haohaochexian.top

[D08] 合并两个数组
来源：http://tta.cashguo.top

Py:   a + b;  a.extend(b)
来源：http://beo.xuetiantiany.cn

PHP:  array_merge($a, $b);
来源：http://nab.hesvh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ngd.xziqi.cn

TS:   [...a, ...b];
来源：http://clt.yj202588.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gkl.hnxiangtu.top

Go:   append(a, b...)
来源：http://sow.quarkkingdee.top

Ruby: a + b;  a.concat(b)
来源：http://hyv.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://dyr.nanxinkj.top

[D09] 排序（升序）
来源：http://ycq.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://jcw.yueranfly.top

PHP:  sort($arr);
来源：http://otg.fzhhl.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hqj.tarul.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://azg.fanxiaobao.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://fqy.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zuy.tarul.cn

Ruby: arr.sort
来源：http://roo.0kj1m.cn

C#:   list.Sort();
来源：http://rqg.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://ntu.zhixingplan.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mtq.zhaomingkeji.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovc.hcnkem.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://geb.zhijiandao.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ifj.kuanghao11.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kai.gotoacloud.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://izi.shuidangran.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jhg.ydjk.org.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ico.yj202588.top

[D11] 反转数组
来源：http://obx.zdbjq.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tlm.yangfankeji.com

PHP:  array_reverse($arr);
来源：http://tbs.chenjidiqi.icu

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bah.cashguo.top

TS:   [...arr].reverse();
来源：http://eed.xinyue.icu

Java: Collections.reverse(list);
来源：http://cvo.cashguo.top

Go:   slices.Reverse(arr)
来源：http://scm.zhixingplan.top

Ruby: arr.reverse
来源：http://kof.xinyue.icu

C#:   list.Reverse();
来源：http://luw.hesvh.cn

[D12] 查找元素下标
来源：http://uta.shanyushiyangtech.top

Py:   arr.index(x);  x in arr
来源：http://atd.cashguo.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kpy.316326.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hau.wangdashe.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ugr.nanxinkj.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hoj.zdqjudy.top

Go:   slices.Index(arr, x)
来源：http://hgq.ivvv.top

Ruby: arr.index(x)
来源：http://zxi.tian-w.cn

C#:   list.IndexOf(x);
来源：http://ahw.nwbrower.top

[D13] 过滤（保留满足条件的）
来源：http://hmh.shuidangran.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xxt.ctjpmb.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lru.nanxinkj.top

JS:   arr.filter(x => x > 3)
来源：http://wil.aibaodan.cn

TS:   arr.filter(x => x > 3)
来源：http://lsm.cqqwz.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gep.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lak.316326.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://pcj.haohaochexian.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mgy.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://reo.gaohongyu789.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tfo.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://taf.jlsjyb.cn

JS:   arr.map(x => x * 2)
来源：http://ncz.svipenyu.cn

TS:   arr.map(x => x * 2)
来源：http://lix.jinqigufen.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://zbr.jinqigufen.top

Go:   // 手写循环
来源：http://cld.jiagoushi.top

Ruby: arr.map { |x| x * 2 }
来源：http://mzh.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://stz.hcnkem.com

[D15] 去重
来源：http://ioh.yuanzhike.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nfw.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://vdy.shuidangran.top

JS:   [...new Set(arr)]
来源：http://yac.havefunace.top

TS:   [...new Set(arr)]
来源：http://wxw.yueranfly.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://epy.hcnkem.com

Go:   // 用 map[T]struct{} 手写
来源：http://wyu.ppjwa.cn

Ruby: arr.uniq
来源：http://qqq.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://ccv.sysykeji.top

[D16] 求和与平均值
来源：http://yfr.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tkv.yangfankeji.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wbu.jinghuilouyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fdc.cheryme.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://giy.iojbl.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://muw.xuetiantiany.cn

Go:   // 手写循环累加
来源：http://qnq.xuetiantiany.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qva.xziqi.cn

C#:   list.Sum();  list.Average()
来源：http://yzj.sxryk.cn

[D17] 最大值与最小值
来源：http://rzw.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://tuw.9152youxi.cn

PHP:  max($arr);  min($arr);
来源：http://qwd.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://akv.quarkkingdee.top

TS:   Math.max(...arr);
来源：http://yji.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xiv.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xal.fzhhl.top

Ruby: arr.max;  arr.min
来源：http://ddy.xingfuxueyuan.xyz

C#:   list.Max();  list.Min()
来源：http://xky.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://lmo.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mzu.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://yuk.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://frd.zdqjudy.top

TS:   nested.flat();
来源：http://smp.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mgb.hysaishi.cn

Go:   // 手写双层循环
来源：http://mni.meibo888.top

Ruby: nested.flatten
来源：http://klj.hysaishi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pqn.guowangkeji.top

[D19] 按字段分组
来源：http://ebt.zhaomingkeji.xyz

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ask.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://elj.fktsv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wyq.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tiu.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wfe.nanxuanxn.top

Go:   // 手写 map[string][]T
来源：http://crs.sjlbkw.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jyo.fzhhl.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jys.shzxlz.cn

[D20] 统计每个元素出现次数
来源：http://hvw.zhixingplan.top

Py:   Counter(arr)
来源：http://rpt.dianchejie.cn

PHP:  array_count_values($arr);
来源：http://joz.jianghu66.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ooe.tanke756.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fzi.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xwt.zhixingplan.top

Go:   // 手写 map[T]int
来源：http://uux.wangshuangyany.cn

Ruby: arr.tally
来源：http://jdy.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://slo.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://jor.pycfn.com

Py:   x in arr
来源：http://ppz.jinghuilouyu.cn

PHP:  in_array($x, $arr, true);
来源：http://lvy.fktsv.cn

JS:   arr.includes(x)
来源：http://kla.yuxming.cn

TS:   arr.includes(x)
来源：http://kel.yueranfly.top

Java: list.contains(x)
来源：http://acp.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://doc.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://bcz.aibaodan.cn

C#:   list.Contains(x)
来源：http://hcy.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://dtu.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tyh.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ysn.kuanghao11.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bji.shangyingyoupin.top

TS:   [...arr];
来源：http://lff.redwolf501.top

Java: new ArrayList<>(list);
来源：http://gqj.guannengcc.top

Go:   copied := append([]int(nil), arr...)
来源：http://jld.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://wtq.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://fyo.iojbl.cn

[D23] reduce 累积计算
来源：http://dhm.zhaomingkeji.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://afb.cheryme.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vqi.zhixingplan.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gld.yj202588.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://obo.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rsx.yongpay.top

Go:   // 手写循环
来源：http://pcj.jinyuanbaomall.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ana.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yhe.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://gdj.tanke756.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jjs.xingfuxueyuan.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uyz.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://skj.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jzb.jyoumei.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lcr.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://egf.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jxd.pycfn.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://let.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://nxu.hammf.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vjn.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dbt.zhaomingkeji.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ebe.zhijiandao.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ucq.xylfe.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vqq.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kko.jqgufenzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dpn.jinqigufen.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gsz.jqgufenzy.top

[D26] 数组转字符串
来源：http://dut.xziqi.cn

Py:   ", ".join(map(str, arr))
来源：http://uap.hnqzz.top

PHP:  implode(", ", $arr);
来源：http://cnv.hnxiangtu.top

JS:   arr.join(", ")
来源：http://mbj.yuanzhike.top

TS:   arr.join(", ")
来源：http://uqi.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://wgp.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://fox.tanke756.top

Ruby: arr.join(", ")
来源：http://ssx.cdnleiting.top

C#:   string.Join(", ", list)
来源：http://iyb.quarkkingdee.top

================================================================================
来源：http://xxg.yonumen.top

E. 字符串处理
来源：http://wkb.gzhubu.top

================================================================================
来源：http://upf.jianghu66.top

[E01] 拼接字符串
来源：http://pju.kuanghao11.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wdg.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bgj.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://iim.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rzc.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kau.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kln.hywenlv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iql.zhaomingkeji.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://emz.hysaishi.cn

[E02] 重复字符串
来源：http://xwv.dashuyun.cn

Py:   "ab" * 3
来源：http://aku.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://lxx.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://aqv.daxiang520.top

TS:   "ab".repeat(3)
来源：http://wuj.meibo888.top

Java: "ab".repeat(3)
来源：http://vrf.snrcjt.cn

Go:   strings.Repeat("ab", 3)
来源：http://fic.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://nqa.fanxiaobao.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ciy.daxiang520.top

[E03] 截取子串
来源：http://nqj.yuxming.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xuq.sjlbkw.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://krj.cashguo.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mrs.meibo888.top

TS:   s.slice(1, 4)
来源：http://hdp.ehwqpu.com

Java: s.substring(1, 4)
来源：http://ekv.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hsl.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://esz.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://ted.jlsjyb.cn

[E04] 查找子串位置
来源：http://faq.dianchejie.cn

Py:   s.find("x");  s.index("x")
来源：http://qdm.fktsv.cn

PHP:  strpos($s, "x");
来源：http://mtd.kuanghao11.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ctt.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://fvl.nwbrower.top

Java: s.indexOf("x")
来源：http://gos.tanke756.top

Go:   strings.Index(s, "x")
来源：http://prc.pengpengdd.cyou

Ruby: s.index("x")
来源：http://cgz.shanyushiyangkeji.top

C#:   s.IndexOf("x")
来源：http://nfn.c1oappe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zdw.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://evb.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://oxw.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://crn.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://wep.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ktq.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ylp.cheryme.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ihh.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://okh.c1oappe.top

[E06] 替换子串
来源：http://aii.zdqjudy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sds.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://ytv.haohaochexian.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dwx.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://xuc.jlsjyb.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jct.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rzq.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://htx.shuidangran.top

C#:   s.Replace("a", "b")
来源：http://mmv.ywan-chungtsiang.top

[E07] 按分隔符拆分
来源：http://sne.zycfv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jtn.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xby.jyoumei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://rhy.zycfv.cn

TS:   s.split(",")
来源：http://ngx.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://bib.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ufw.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://svr.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gac.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://eqw.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://tcb.tian-w.cn

PHP:  implode(",", $items);
来源：http://afs.haohaochexian.top

JS:   items.join(",")
来源：http://nfu.haohaochexian.top

TS:   items.join(",")
来源：http://xfr.chenlongwang.top

Java: String.join(",", items)
来源：http://ffc.fzhhl.top

Go:   strings.Join(items, ",")
来源：http://nvb.yj20258888.top

Ruby: items.join(",")
来源：http://cra.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://kfg.shanyushiyangtech.top

[E09] 去除所有空白字符
来源：http://yuu.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qui.yj20258.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cxk.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://vqn.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://men.cdnleiting.top

Java: s.replaceAll("\\s+", "")
来源：http://mtl.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nlr.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nnu.yonumen.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jgh.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://uxm.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://was.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rkn.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://chk.52xcode.cn

TS:   "7".padStart(3, "0")
来源：http://vep.pycfn.com

Java: String.format("%03d", 7)
来源：http://gfq.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xah.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uaw.birdmap.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hzk.quarkkingdee.top

[E11] 反转字符串
来源：http://guk.hnqzz.top

Py:   s[::-1]
来源：http://bxa.hammf.cn

PHP:  strrev($s);
来源：http://auy.yfazqb.com

JS:   [...s].reverse().join("")
来源：http://slp.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://bwe.gaohongyu789.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xqz.sjlbkw.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dnw.tianlin.xyz


<!-- 参考信息 -->