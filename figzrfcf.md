代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://nau.vqdsnc.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xrr.andypj.xyz

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pfb.snrcjt.cn

[D06] 数组长度
来源：http://zec.ivvv.top

Py:   len(arr)
来源：http://pyb.jianghu66.top

PHP:  count($arr);
来源：http://zbw.0kj1m.cn

JS:   arr.length
来源：http://nwa.jinyuanbaomall.cn

TS:   arr.length
来源：http://vxd.tianlin.xyz

Java: list.size();
来源：http://qqt.dianchejie.cn

Go:   len(arr)
来源：http://hdj.52xcode.cn

Ruby: arr.length; arr.size
来源：http://ayd.xinyue.icu

C#:   list.Count;
来源：http://bul.zhijiandao.cn

[D07] 切片 / 取子数组
来源：http://voq.iojbl.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://evq.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://tou.cheryme.top

JS:   arr.slice(1, 4);
来源：http://gep.9152youxi.cn

TS:   arr.slice(1, 4);
来源：http://wph.hesvh.cn

Java: list.subList(1, 4);
来源：http://ukl.aibaodan.cn

Go:   arr[1:4]
来源：http://nlv.hammf.cn

Ruby: arr[1, 3]
来源：http://mgw.yonumen.top

C#:   list.GetRange(1, 3);
来源：http://xwl.nanxuanxn.top

[D08] 合并两个数组
来源：http://mpv.yj202588.top

Py:   a + b;  a.extend(b)
来源：http://ltx.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://elk.zhixingplan.top

JS:   [...a, ...b];  a.concat(b);
来源：http://ult.shuidangran.top

TS:   [...a, ...b];
来源：http://rqz.pycfn.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mcu.shzxlz.cn

Go:   append(a, b...)
来源：http://uak.cucudq.cn

Ruby: a + b;  a.concat(b)
来源：http://tdm.yj20258888.top

C#:   a.Concat(b).ToList()
来源：http://wfy.ivvv.top

[D09] 排序（升序）
来源：http://rga.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://vfa.hysaishi.cn

PHP:  sort($arr);
来源：http://zzo.gotoacloud.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yur.guannengcc.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://esd.yangfankeji.com

Java: Collections.sort(list);  list.sort(null);
来源：http://eak.guowangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yda.zdbjq.cn

Ruby: arr.sort
来源：http://otv.uphjek.com

C#:   list.Sort();
来源：http://quq.gaohongyu789.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://fhb.mhx1999.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wjg.jlsjyb.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cda.sufxvd.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hde.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dps.jinqigfzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://roq.daxiang520.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qve.cdnleiting.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tax.xingfuxueyuan.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://arn.yuanzhike.top

[D11] 反转数组
来源：http://sxi.hnqzz.top

Py:   arr[::-1];  arr.reverse()
来源：http://rcy.aibaodan.cn

PHP:  array_reverse($arr);
来源：http://ayd.smart0.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ntt.wangdashe.top

TS:   [...arr].reverse();
来源：http://nle.pengpengdd.cyou

Java: Collections.reverse(list);
来源：http://kvg.quarkkingdee.top

Go:   slices.Reverse(arr)
来源：http://wup.yanxiufei.cn

Ruby: arr.reverse
来源：http://smn.hysaishi.cn

C#:   list.Reverse();
来源：http://nff.jqgufenzy.top

[D12] 查找元素下标
来源：http://eux.jinyuanbaomall.cn

Py:   arr.index(x);  x in arr
来源：http://flp.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fda.birdmap.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zgb.ctjpmb.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vvb.yueranfly.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://swj.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://wlh.yvedp.cn

Ruby: arr.index(x)
来源：http://hbp.yvedp.cn

C#:   list.IndexOf(x);
来源：http://hrj.yanxiufei.cn

[D13] 过滤（保留满足条件的）
来源：http://eqb.svipenyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yeq.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ppj.cashguo.top

JS:   arr.filter(x => x > 3)
来源：http://afg.nanxuanxn.top

TS:   arr.filter(x => x > 3)
来源：http://zgp.cucudq.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pra.fanxiaobao.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uaw.jlsjyb.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uwa.snrcjt.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kng.pengpengdd.cyou

[D14] 映射转换（每个元素变形）
来源：http://igy.vqdsnc.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jkb.vqdsnc.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://atr.feifeiyinyue.top

JS:   arr.map(x => x * 2)
来源：http://rwq.zhiwuduotai.top

TS:   arr.map(x => x * 2)
来源：http://bub.jiagoushi.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://sfd.yueranfly.top

Go:   // 手写循环
来源：http://cxm.xuetiantiany.cn

Ruby: arr.map { |x| x * 2 }
来源：http://giq.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oky.sysykeji.top

[D15] 去重
来源：http://mkr.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dyx.zdbjq.cn

PHP:  array_unique($arr);
来源：http://kjp.redwolf501.top

JS:   [...new Set(arr)]
来源：http://hgj.tian-w.cn

TS:   [...new Set(arr)]
来源：http://wzg.yuxming.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ryf.fktsv.cn

Go:   // 用 map[T]struct{} 手写
来源：http://glq.yuanzhike.top

Ruby: arr.uniq
来源：http://xlb.wangshuangyany.cn

C#:   list.Distinct().ToList()
来源：http://seh.yj20258888.top

[D16] 求和与平均值
来源：http://gng.9152youxi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vcg.tanke756.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cjd.yj20258.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qgl.svipenyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hnx.gaohongyu789.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sia.daria6918.cn

Go:   // 手写循环累加
来源：http://irr.ywan-chungtsiang.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ltr.hnqzz.top

C#:   list.Sum();  list.Average()
来源：http://xuv.jqgfzy.top

[D17] 最大值与最小值
来源：http://tad.havefunace.top

Py:   max(arr);  min(arr)
来源：http://hhx.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://wjo.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ekg.cashguo.top

TS:   Math.max(...arr);
来源：http://gzj.zhongyouzk.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gdj.sufxvd.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ueo.shzxlz.cn

Ruby: arr.max;  arr.min
来源：http://lfk.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://emp.guannengcc.top

[D18] 扁平化嵌套数组
来源：http://ejh.fanxiaobao.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vql.meibo888.top

PHP:  array_merge(...$nested);
来源：http://iqi.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iox.aizwys.cn

TS:   nested.flat();
来源：http://naz.jyoumei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ohz.chenzaomai.com

Go:   // 手写双层循环
来源：http://jox.yangfankeji.com

Ruby: nested.flatten
来源：http://ufr.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://anq.hongshengwenyu.top

[D19] 按字段分组
来源：http://vux.ctjpmb.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fxr.hongshengwenyu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hxo.jlsjyb.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tdp.smart0.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://soc.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cbb.ywan-chungtsiang.top

Go:   // 手写 map[string][]T
来源：http://liy.yanxiufei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zyp.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rjh.yanxiufei.cn

[D20] 统计每个元素出现次数
来源：http://sgj.cucudq.cn

Py:   Counter(arr)
来源：http://hvl.yanxiufei.cn

PHP:  array_count_values($arr);
来源：http://soh.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rdt.shuidangran.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://axl.xinyue.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ecs.yvedp.cn

Go:   // 手写 map[T]int
来源：http://fah.vqdsnc.cn

Ruby: arr.tally
来源：http://bqe.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wal.zhongyouzk.top

[D21] 判断是否包含某元素
来源：http://xgv.yuxming.cn

Py:   x in arr
来源：http://sbm.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://vro.sysykeji.top

JS:   arr.includes(x)
来源：http://wcs.xylfe.cn

TS:   arr.includes(x)
来源：http://uez.feifeiyinyue.top

Java: list.contains(x)
来源：http://oky.wangdashe.top

Go:   slices.Contains(arr, x)
来源：http://pmb.cdnleiting.top

Ruby: arr.include?(x)
来源：http://bmi.shanyushiyangtech.top

C#:   list.Contains(x)
来源：http://tkd.hongshengwenyu.top

[D22] 复制数组（避免共享引用）
来源：http://vnl.ywan-chungtsiang.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nth.fktsv.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nsr.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pdp.wangshuangyany.cn

TS:   [...arr];
来源：http://eph.jiagoushi.top

Java: new ArrayList<>(list);
来源：http://ulx.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mio.yueranfly.top

Ruby: arr.dup;  arr.clone
来源：http://sfn.yuxming.cn

C#:   new List<int>(list);
来源：http://vyf.haohaochexian.top

[D23] reduce 累积计算
来源：http://fke.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pli.hfpthk.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://den.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jzn.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tni.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oby.zhengqikj.top

Go:   // 手写循环
来源：http://zsh.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zjs.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pjk.jqgfzy.top

[D24] 字典 / Map 基本操作
来源：http://dse.birdmap.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kpq.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mdd.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kyr.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gwg.yonumen.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zag.uphjek.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kic.jinghuilouyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zcn.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gjv.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://mrq.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yqs.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tag.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://jpp.ywan-chungtsiang.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gcp.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://evh.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://owh.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jab.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://grh.yuxming.cn

[D26] 数组转字符串
来源：http://oxr.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://pmk.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://zrf.gzhubu.top

JS:   arr.join(", ")
来源：http://jga.zhixingplan.top

TS:   arr.join(", ")
来源：http://iwf.mhx1999.top

Java: String.join(", ", list)
来源：http://khs.yonumen.top

Go:   strings.Join(strs, ", ")
来源：http://zvv.yj20258.top

Ruby: arr.join(", ")
来源：http://ybb.fktsv.cn

C#:   string.Join(", ", list)
来源：http://mcr.zycfv.cn

================================================================================
来源：http://tch.zhaomingkeji.xyz

E. 字符串处理
来源：http://rxt.tian-w.cn

================================================================================
来源：http://gvl.svipenyu.cn

[E01] 拼接字符串
来源：http://fjf.mhx1999.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zkd.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tkt.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ezv.xuanzx.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sef.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iqs.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ark.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rys.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://iwn.cashguo.top

[E02] 重复字符串
来源：http://qjp.zhiwuduotai.top

Py:   "ab" * 3
来源：http://hlz.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://pig.yanxiufei.cn

JS:   "ab".repeat(3)
来源：http://nxc.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://rxu.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://red.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://mrx.chenzaomai.com

Ruby: "ab" * 3
来源：http://mrx.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nnm.shzxlz.cn

[E03] 截取子串
来源：http://mdo.yj202588.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zxw.zhixingplan.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://owh.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kce.havefunace.top

TS:   s.slice(1, 4)
来源：http://pum.jinqigufen.top

Java: s.substring(1, 4)
来源：http://cds.xuetiantiany.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://unh.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://jnx.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://eku.daria6918.cn

[E04] 查找子串位置
来源：http://xbe.zhiwuduotai.top

Py:   s.find("x");  s.index("x")
来源：http://tvw.9152youxi.cn

PHP:  strpos($s, "x");
来源：http://zmy.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pqt.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://wts.vqdsnc.cn

Java: s.indexOf("x")
来源：http://fyj.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://pyg.daxiang520.top

Ruby: s.index("x")
来源：http://pxw.uphjek.com

C#:   s.IndexOf("x")
来源：http://qxr.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://stu.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://snm.zycfv.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cce.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mvr.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://kpa.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gkd.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vlt.wangdashe.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aju.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sjr.hesvh.cn

[E06] 替换子串
来源：http://jdg.shzxlz.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qrr.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://hjz.gaohongyu789.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zfx.yj20258888.top

TS:   s.replaceAll("a", "b")
来源：http://kih.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktn.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sjz.tanke756.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mgd.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://swq.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://ike.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gqe.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pzu.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://imb.yanxiufei.cn

TS:   s.split(",")
来源：http://tts.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dkq.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vkl.fehbvm.com

Ruby: s.split(",");  s.split
来源：http://sxy.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eyw.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://tnh.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://arq.52xcode.cn

PHP:  implode(",", $items);
来源：http://lzm.shangyingyoupin.top

JS:   items.join(",")
来源：http://zcx.xuetiantiany.cn

TS:   items.join(",")
来源：http://ety.52xcode.cn

Java: String.join(",", items)
来源：http://qzr.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://vdd.epnwcf.com

Ruby: items.join(",")
来源：http://ncb.haohaochexian.top

C#:   string.Join(",", items)
来源：http://aul.xinyue.icu

[E09] 去除所有空白字符
来源：http://yrh.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zyc.ywan-chungtsiang.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ouq.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://red.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://mlj.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://tli.jqgfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nun.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://dis.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vnf.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://gyp.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mbf.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://inm.redwolf501.top

JS:   "7".padStart(3, "0")
来源：http://hbg.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://loh.havefunace.top

Java: String.format("%03d", 7)
来源：http://hfd.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://aam.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://chr.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://olg.tian-w.cn

[E11] 反转字符串
来源：http://ymy.ppjwa.cn

Py:   s[::-1]
来源：http://mfy.vqdsnc.cn

PHP:  strrev($s);
来源：http://ixw.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://mck.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://niz.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dxu.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gii.shuidangran.top

Ruby: s.reverse
来源：http://ivn.xuetiantiany.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qki.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://qut.ppjwa.cn

Py:   s.count("a")
来源：http://gro.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://esn.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://jpw.yueranfly.top

TS:   s.split("a").length - 1
来源：http://zhi.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oyz.yvedp.cn


<!-- 参考信息 -->