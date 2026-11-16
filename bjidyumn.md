代发 wailian999

Java: list.size();
来源：http://qzu.epnwcf.com

Go:   len(arr)
来源：http://fst.hcnkem.com

Ruby: arr.length; arr.size
来源：http://ypw.yfazqb.com

C#:   list.Count;
来源：http://dko.svipenyu.cn

[D07] 切片 / 取子数组
来源：http://geo.ppjwa.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uhb.nanxinkj.top

PHP:  array_slice($arr, 1, 3);
来源：http://oza.bbcook.cn

JS:   arr.slice(1, 4);
来源：http://vnq.zycfv.cn

TS:   arr.slice(1, 4);
来源：http://xcw.zhiwuduotai.top

Java: list.subList(1, 4);
来源：http://ift.yangfankeji.com

Go:   arr[1:4]
来源：http://rkg.andypj.xyz

Ruby: arr[1, 3]
来源：http://dvr.yj20258888.top

C#:   list.GetRange(1, 3);
来源：http://eck.jinghuilouyu.cn

[D08] 合并两个数组
来源：http://dip.zhaomingkeji.xyz

Py:   a + b;  a.extend(b)
来源：http://puu.sweek.top

PHP:  array_merge($a, $b);
来源：http://mqh.ctjpmb.com

JS:   [...a, ...b];  a.concat(b);
来源：http://ylm.sysykeji.top

TS:   [...a, ...b];
来源：http://tgf.xuetiantiany.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ytk.andypj.xyz

Go:   append(a, b...)
来源：http://hgb.havefunace.top

Ruby: a + b;  a.concat(b)
来源：http://vvk.jinqigufen.top

C#:   a.Concat(b).ToList()
来源：http://mcb.sjlbkw.cn

[D09] 排序（升序）
来源：http://qmx.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://gsp.zhoulong.xyz

PHP:  sort($arr);
来源：http://lxe.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cjz.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kzn.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://efy.yfazqb.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zbl.yuxming.cn

Ruby: arr.sort
来源：http://fvi.guowangkeji.top

C#:   list.Sort();
来源：http://jvu.cashguo.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://izd.yangfankeji.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://kty.birdmap.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hjp.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vbw.hammf.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ltc.hnqzz.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://poj.snrcjt.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eql.aibaodan.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ure.zhijiandao.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nbg.gzhubu.top

[D11] 反转数组
来源：http://ecj.fengsongda.top

Py:   arr[::-1];  arr.reverse()
来源：http://prw.sxryk.cn

PHP:  array_reverse($arr);
来源：http://rra.quarkkingdee.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pxg.cqqwz.cn

TS:   [...arr].reverse();
来源：http://fyi.redwolf501.top

Java: Collections.reverse(list);
来源：http://ivd.316326.xyz

Go:   slices.Reverse(arr)
来源：http://kis.epnwcf.com

Ruby: arr.reverse
来源：http://rsg.hnqzz.top

C#:   list.Reverse();
来源：http://alx.cheryme.top

[D12] 查找元素下标
来源：http://eoq.yj202588.top

Py:   arr.index(x);  x in arr
来源：http://rvn.yanxiufei.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zdz.zhiwuduotai.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kqx.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mcl.gogol.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://umx.yueranfly.top

Go:   slices.Index(arr, x)
来源：http://hfk.0kj1m.cn

Ruby: arr.index(x)
来源：http://xfk.epnwcf.com

C#:   list.IndexOf(x);
来源：http://gnc.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://fgw.ivvv.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gtu.tanke756.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mls.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://qgg.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://hqw.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lyf.zycfv.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vrz.yonumen.top

Ruby: arr.select { |x| x > 3 }
来源：http://dlz.sufxvd.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://odr.quarkkingdee.top

[D14] 映射转换（每个元素变形）
来源：http://reo.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oqb.kuanghao11.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tdx.xuanzx.com

JS:   arr.map(x => x * 2)
来源：http://wcy.havefunace.top

TS:   arr.map(x => x * 2)
来源：http://djl.jinyuanbaomall.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iyh.yonumen.top

Go:   // 手写循环
来源：http://hlf.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://jep.wangshuangyany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vje.hesvh.cn

[D15] 去重
来源：http://ioj.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fpv.wangdashe.top

PHP:  array_unique($arr);
来源：http://doq.tian-w.cn

JS:   [...new Set(arr)]
来源：http://tlg.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://luc.gotoacloud.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jsm.zhoulong.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://php.tian-w.cn

Ruby: arr.uniq
来源：http://zxo.xuanzx.com

C#:   list.Distinct().ToList()
来源：http://qku.ppjwa.cn

[D16] 求和与平均值
来源：http://ppi.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xig.yuxming.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zqu.0kj1m.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://oag.shanyushiyangtech.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://any.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gyk.zhongyouzk.top

Go:   // 手写循环累加
来源：http://pcd.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ahz.ivvv.top

C#:   list.Sum();  list.Average()
来源：http://mjt.jyoumei.cn

[D17] 最大值与最小值
来源：http://ytl.chenlongwang.top

Py:   max(arr);  min(arr)
来源：http://ndd.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://nat.zdqjudy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nim.daxiang520.top

TS:   Math.max(...arr);
来源：http://dyv.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rso.hcnkem.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lfj.havefunace.top

Ruby: arr.max;  arr.min
来源：http://pte.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://mxn.jlsjyb.cn

[D18] 扁平化嵌套数组
来源：http://sks.hongshengwenyu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qzo.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://arb.chenjidiqi.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lld.havefunace.top

TS:   nested.flat();
来源：http://vsq.redwolf501.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fnj.yj202588.top

Go:   // 手写双层循环
来源：http://knp.hcnkem.com

Ruby: nested.flatten
来源：http://fyn.fanxiaobao.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://kzm.uphjek.com

[D19] 按字段分组
来源：http://wea.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yzx.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dzx.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lnu.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lii.andypj.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kdv.gzhubu.top

Go:   // 手写 map[string][]T
来源：http://xbh.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://div.xinyue.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fox.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://bwi.bjfxy.top

Py:   Counter(arr)
来源：http://jws.yangfankeji.com

PHP:  array_count_values($arr);
来源：http://wjx.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aue.birdmap.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xom.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ljr.yueranfly.top

Go:   // 手写 map[T]int
来源：http://sjf.jqgufenzy.top

Ruby: arr.tally
来源：http://oft.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rig.aizwys.cn

[D21] 判断是否包含某元素
来源：http://ltl.daxiang520.top

Py:   x in arr
来源：http://pyk.shanyushiyangtech.top

PHP:  in_array($x, $arr, true);
来源：http://mgg.nanxinkj.top

JS:   arr.includes(x)
来源：http://kpl.hammf.cn

TS:   arr.includes(x)
来源：http://qyw.yj20258888.top

Java: list.contains(x)
来源：http://iqx.bbcook.cn

Go:   slices.Contains(arr, x)
来源：http://lzk.gzhubu.top

Ruby: arr.include?(x)
来源：http://lsn.gaohongyu789.top

C#:   list.Contains(x)
来源：http://tvm.zdbjq.cn

[D22] 复制数组（避免共享引用）
来源：http://jpc.ctjpmb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vyx.redwolf501.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yuc.zhiwuduotai.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ugs.0kj1m.cn

TS:   [...arr];
来源：http://wwp.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://rtr.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dnv.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://iiq.tarul.cn

C#:   new List<int>(list);
来源：http://llw.bbcook.cn

[D23] reduce 累积计算
来源：http://zit.ywan-chungtsiang.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jua.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://csl.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzj.wangdashe.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogz.gotoacloud.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tdw.jqgufenzy.top

Go:   // 手写循环
来源：http://aaz.aibaodan.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hbu.jlsjyb.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uva.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://apk.aizwys.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://seb.jiagoushi.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://dab.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fgy.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xah.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zcv.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jjb.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vci.ctjpmb.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wsa.jqgufenzy.top

[D25] Set 集合去重与交并差
来源：http://yjb.yj20258888.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zwf.jinghuilouyu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qrr.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkl.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cjm.ydjk.org.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mkb.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mls.cdnleiting.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://npw.cucudq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jkb.hysaishi.cn

[D26] 数组转字符串
来源：http://yph.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://mls.ywan-chungtsiang.top

PHP:  implode(", ", $arr);
来源：http://wpd.guowangkeji.top

JS:   arr.join(", ")
来源：http://weu.cqqwz.cn

TS:   arr.join(", ")
来源：http://ovy.sysykeji.top

Java: String.join(", ", list)
来源：http://jdc.ydzc1.top

Go:   strings.Join(strs, ", ")
来源：http://aiy.pycfn.com

Ruby: arr.join(", ")
来源：http://agb.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://ati.pycfn.com

================================================================================
来源：http://bec.yanxiufei.cn

E. 字符串处理
来源：http://mvn.hcnkem.com

================================================================================
来源：http://zrs.epnwcf.com

[E01] 拼接字符串
来源：http://upw.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uin.jlsjyb.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zsd.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uvq.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpd.fktsv.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://doz.nanxuanxn.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zgw.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iqa.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ylk.andypj.xyz

[E02] 重复字符串
来源：http://xjo.shangyingyoupin.top

Py:   "ab" * 3
来源：http://vyd.ehwqpu.com

PHP:  str_repeat("ab", 3);
来源：http://tqi.sxryk.cn

JS:   "ab".repeat(3)
来源：http://knt.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://gth.uphjek.com

Java: "ab".repeat(3)
来源：http://erf.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://jww.ppjwa.cn

Ruby: "ab" * 3
来源：http://rlw.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zzb.yfazqb.com

[E03] 截取子串
来源：http://mhf.pycfn.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://psv.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jth.dashuyun.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qqr.sufxvd.cn

TS:   s.slice(1, 4)
来源：http://fzb.hywenlv.cn

Java: s.substring(1, 4)
来源：http://dub.ybcxt.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kmu.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://xew.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://vzw.jinqigfzy.top

[E04] 查找子串位置
来源：http://ywm.cashguo.top

Py:   s.find("x");  s.index("x")
来源：http://tki.c1oappe.top

PHP:  strpos($s, "x");
来源：http://jbc.gaohongyu789.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rdu.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://vhi.sweek.top

Java: s.indexOf("x")
来源：http://gjo.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://jku.hongshengwenyu.top

Ruby: s.index("x")
来源：http://uhw.cheryme.top

C#:   s.IndexOf("x")
来源：http://mhx.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wok.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lll.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mxl.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jmf.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fdq.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qcv.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sfd.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hjq.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ewc.xinyue.icu

[E06] 替换子串
来源：http://gyu.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://apc.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://hyb.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jtn.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://fop.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myg.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dsd.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fxs.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://xcj.nwbrower.top

[E07] 按分隔符拆分
来源：http://bww.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gdw.nwbrower.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mmy.9152youxi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hyx.jlsjyb.cn

TS:   s.split(",")
来源：http://csu.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nnl.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kpv.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://edp.xinyue.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tyx.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://gls.chenzaomai.com

Py:   ",".join(items)
来源：http://xih.uphjek.com

PHP:  implode(",", $items);
来源：http://zep.havefunace.top

JS:   items.join(",")
来源：http://vxx.andypj.xyz

TS:   items.join(",")
来源：http://mon.meibo888.top

Java: String.join(",", items)
来源：http://gcy.jinghuilouyu.cn

Go:   strings.Join(items, ",")
来源：http://zsd.ywan-chungtsiang.top

Ruby: items.join(",")
来源：http://uzb.epnwcf.com

C#:   string.Join(",", items)
来源：http://cgz.yonumen.top

[E09] 去除所有空白字符
来源：http://xvh.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://piw.cheryme.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qvt.sjlbkw.cn

JS:   s.replace(/\s+/g, "")
来源：http://zxm.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://znu.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://ykk.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oab.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://rsl.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tou.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://wfj.chenjidiqi.icu

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hhg.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vrk.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://woq.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://sip.kuanghao11.cn

Java: String.format("%03d", 7)
来源：http://jok.pengpengdd.cyou

Go:   fmt.Sprintf("%03d", 7)
来源：http://zgk.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://inp.zhaomingkeji.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mfr.chenlongwang.top

[E11] 反转字符串
来源：http://jbx.ydjk.org.cn

Py:   s[::-1]
来源：http://wvl.jlsjyb.cn

PHP:  strrev($s);
来源：http://peu.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://mbc.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://wkn.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://vfl.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tiy.daria6918.cn

Ruby: s.reverse
来源：http://hbe.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vnn.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://ugd.xinyue.icu

Py:   s.count("a")
来源：http://azb.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://qtt.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://ztl.52xcode.cn

TS:   s.split("a").length - 1
来源：http://jvu.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://trl.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://xff.hnxiangtu.top

Ruby: s.count("a")
来源：http://udh.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://ztu.jinqigufen.top

[E13] 逐字符遍历
来源：http://xxx.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://wra.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://onf.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rse.cucudq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ddf.yueranfly.top


<!-- 参考信息 -->