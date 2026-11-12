代发 wailian999

Java: list.size();
来源：http://gdf.316326.xyz

Go:   len(arr)
来源：http://lfb.jinyuanbaomall.cn

Ruby: arr.length; arr.size
来源：http://gmm.tianlin.xyz

C#:   list.Count;
来源：http://fxi.jqgufenzy.top

[D07] 切片 / 取子数组
来源：http://ste.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ajd.snrcjt.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yqk.wangdashe.top

JS:   arr.slice(1, 4);
来源：http://rlo.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://yfb.shuidangran.top

Java: list.subList(1, 4);
来源：http://ygp.yueranfly.top

Go:   arr[1:4]
来源：http://dhs.cdnleiting.top

Ruby: arr[1, 3]
来源：http://okb.iojbl.cn

C#:   list.GetRange(1, 3);
来源：http://ccx.fehbvm.com

[D08] 合并两个数组
来源：http://dit.tanke756.top

Py:   a + b;  a.extend(b)
来源：http://tab.yuanzhike.top

PHP:  array_merge($a, $b);
来源：http://jcp.andypj.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://ngx.yj20258.top

TS:   [...a, ...b];
来源：http://eyo.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xcn.svipenyu.cn

Go:   append(a, b...)
来源：http://cts.zhixingplan.top

Ruby: a + b;  a.concat(b)
来源：http://lei.gotoacloud.top

C#:   a.Concat(b).ToList()
来源：http://sij.jqgfzy.top

[D09] 排序（升序）
来源：http://wpz.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://mzw.bbcook.cn

PHP:  sort($arr);
来源：http://eeq.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rhr.hnxiangtu.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://dda.zycfv.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gae.yangfankeji.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qpw.dashuyun.cn

Ruby: arr.sort
来源：http://frg.yj20258.top

C#:   list.Sort();
来源：http://hvd.gogol.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ztb.birdmap.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aot.aibaodan.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehl.yangfankeji.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vnp.jqgufenzy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ymr.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tpj.daria6918.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rbg.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ztn.dianchejie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xbm.guowangkeji.top

[D11] 反转数组
来源：http://rfn.ehwqpu.com

Py:   arr[::-1];  arr.reverse()
来源：http://fsu.gaohongyu789.top

PHP:  array_reverse($arr);
来源：http://ybc.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://djb.pengpengdd.cyou

TS:   [...arr].reverse();
来源：http://dcq.dashuyun.cn

Java: Collections.reverse(list);
来源：http://knc.zdqjudy.top

Go:   slices.Reverse(arr)
来源：http://vti.nwbrower.top

Ruby: arr.reverse
来源：http://mjc.tarul.cn

C#:   list.Reverse();
来源：http://kog.jyoumei.cn

[D12] 查找元素下标
来源：http://sna.daria6918.cn

Py:   arr.index(x);  x in arr
来源：http://nrb.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jyh.zhoulong.xyz

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pnj.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gue.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://tzx.andypj.xyz

Go:   slices.Index(arr, x)
来源：http://wbr.ywan-chungtsiang.top

Ruby: arr.index(x)
来源：http://tgv.kuanghao11.cn

C#:   list.IndexOf(x);
来源：http://bjp.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://pge.0kj1m.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uww.sysykeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://poe.jqgufenzy.top

JS:   arr.filter(x => x > 3)
来源：http://cny.haohaochexian.top

TS:   arr.filter(x => x > 3)
来源：http://uob.ydzc1.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iwv.jqgufenzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zlz.iojbl.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wmg.jlsjyb.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ski.jinqigufen.top

[D14] 映射转换（每个元素变形）
来源：http://nmd.vehdjk.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hxl.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://stm.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://mdn.bjfxy.top

TS:   arr.map(x => x * 2)
来源：http://tqf.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ddo.xylfe.cn

Go:   // 手写循环
来源：http://gmu.chenjidiqi.icu

Ruby: arr.map { |x| x * 2 }
来源：http://rbj.dianchejie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uku.vehdjk.com

[D15] 去重
来源：http://ewo.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jyv.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://xjj.yj202588.top

JS:   [...new Set(arr)]
来源：http://ofe.nanxinkj.top

TS:   [...new Set(arr)]
来源：http://yna.xziqi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://loy.zhiwuduotai.top

Go:   // 用 map[T]struct{} 手写
来源：http://hfg.birdmap.top

Ruby: arr.uniq
来源：http://dgh.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://kav.ywan-chungtsiang.top

[D16] 求和与平均值
来源：http://pba.shzxlz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yvk.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xzm.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bmd.aibaodan.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://twx.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://adx.gotoacloud.top

Go:   // 手写循环累加
来源：http://xja.yonumen.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mzm.zdqjudy.top

C#:   list.Sum();  list.Average()
来源：http://yon.yonumen.top

[D17] 最大值与最小值
来源：http://fdt.yueranfly.top

Py:   max(arr);  min(arr)
来源：http://oxi.jlsjyb.cn

PHP:  max($arr);  min($arr);
来源：http://juy.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://upk.aibaodan.cn

TS:   Math.max(...arr);
来源：http://qqk.jinqigufen.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qfh.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rmw.jinqigfzy.top

Ruby: arr.max;  arr.min
来源：http://hur.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://xqu.52xcode.cn

[D18] 扁平化嵌套数组
来源：http://cwy.gogol.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ets.jqgufenzy.top

PHP:  array_merge(...$nested);
来源：http://eoz.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xav.mhx1999.top

TS:   nested.flat();
来源：http://wtl.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vfw.yj20258.top

Go:   // 手写双层循环
来源：http://hrz.gogol.net.cn

Ruby: nested.flatten
来源：http://nxs.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ggf.aizwys.cn

[D19] 按字段分组
来源：http://cvo.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://snh.daria6918.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ppk.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fna.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ypw.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ptx.svipenyu.cn

Go:   // 手写 map[string][]T
来源：http://cez.dianchejie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yvt.sjlbkw.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gfb.yuanzhike.top

[D20] 统计每个元素出现次数
来源：http://yzc.jinqigufen.top

Py:   Counter(arr)
来源：http://rex.fktsv.cn

PHP:  array_count_values($arr);
来源：http://aho.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kla.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzo.daria6918.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bnb.tanke756.top

Go:   // 手写 map[T]int
来源：http://rdu.jinqigfzy.top

Ruby: arr.tally
来源：http://fwo.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qwb.tianlin.xyz

[D21] 判断是否包含某元素
来源：http://pmz.meibo888.top

Py:   x in arr
来源：http://qdc.sweek.top

PHP:  in_array($x, $arr, true);
来源：http://otr.quarkkingdee.top

JS:   arr.includes(x)
来源：http://mpv.sysykeji.top

TS:   arr.includes(x)
来源：http://bcu.chenzaomai.com

Java: list.contains(x)
来源：http://kph.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://zhc.yvedp.cn

Ruby: arr.include?(x)
来源：http://fot.ydjk.org.cn

C#:   list.Contains(x)
来源：http://blj.zhaomingkeji.xyz

[D22] 复制数组（避免共享引用）
来源：http://idi.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpq.sjlbkw.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ayx.zdbjq.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hkf.pengpengdd.cyou

TS:   [...arr];
来源：http://qhl.yonumen.top

Java: new ArrayList<>(list);
来源：http://apq.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://hvj.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://iwi.hysaishi.cn

C#:   new List<int>(list);
来源：http://gsx.gogol.net.cn

[D23] reduce 累积计算
来源：http://vxh.jqgfzy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zuh.yvedp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bag.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kts.zhijiandao.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cnm.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vmn.gaohongyu789.top

Go:   // 手写循环
来源：http://wdf.vehdjk.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gwx.nanxinkj.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://acw.tanke756.top

[D24] 字典 / Map 基本操作
来源：http://ozf.shanyushiyangtech.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fpq.gotoacloud.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://egl.xuanzx.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cez.tanke756.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kaa.yj20258.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kgn.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://scj.hammf.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bex.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mvc.gaohongyu789.top

[D25] Set 集合去重与交并差
来源：http://suu.tian-w.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dlo.chenjidiqi.icu

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://awh.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qju.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fbj.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dfd.havefunace.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ito.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vsx.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jym.316326.xyz

[D26] 数组转字符串
来源：http://qfk.pycfn.com

Py:   ", ".join(map(str, arr))
来源：http://obf.yongpay.top

PHP:  implode(", ", $arr);
来源：http://ofo.xuanzx.com

JS:   arr.join(", ")
来源：http://fte.gotoacloud.top

TS:   arr.join(", ")
来源：http://gua.sufxvd.cn

Java: String.join(", ", list)
来源：http://wvq.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://xbu.tian-w.cn

Ruby: arr.join(", ")
来源：http://cfg.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://tlo.xuanzx.com

================================================================================
来源：http://mzq.jinyuanbaomall.cn

E. 字符串处理
来源：http://xng.tanke756.top

================================================================================
来源：http://fht.fengsongda.top

[E01] 拼接字符串
来源：http://rkf.jyoumei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bnp.shzxlz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ojy.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://omi.fanxiaobao.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jwe.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vqz.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cky.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rsk.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ouf.yuanzhike.top

[E02] 重复字符串
来源：http://ung.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://jwh.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://fwt.jinqigfzy.top

JS:   "ab".repeat(3)
来源：http://oam.pengpengdd.cyou

TS:   "ab".repeat(3)
来源：http://dqk.yj20258888.top

Java: "ab".repeat(3)
来源：http://cqi.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://pgl.hammf.cn

Ruby: "ab" * 3
来源：http://typ.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kpb.yanxiufei.cn

[E03] 截取子串
来源：http://ikq.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yme.shuidangran.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ale.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ixi.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://yci.ehwqpu.com

Java: s.substring(1, 4)
来源：http://rfc.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vmy.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://czf.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://kpz.tanke756.top

[E04] 查找子串位置
来源：http://enn.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://aqx.snrcjt.cn

PHP:  strpos($s, "x");
来源：http://toj.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ogk.birdmap.top

TS:   s.indexOf("x")
来源：http://ytw.sjlbkw.cn

Java: s.indexOf("x")
来源：http://ugd.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://cqr.sufxvd.cn

Ruby: s.index("x")
来源：http://aot.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://iek.xuetiantiany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qjt.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uvl.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mja.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwt.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfb.zdqjudy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yng.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://csw.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://syj.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://umn.chenzaomai.com

[E06] 替换子串
来源：http://pko.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ija.yj20258.top

PHP:  str_replace("a", "b", $s);
来源：http://aar.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://srz.zhiwuduotai.top

TS:   s.replaceAll("a", "b")
来源：http://mma.sysykeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rrh.hysaishi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bhh.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kao.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://ptj.shzxlz.cn

[E07] 按分隔符拆分
来源：http://bvl.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tib.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://edd.dianchejie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://syb.daria6918.cn

TS:   s.split(",")
来源：http://juf.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://rml.bbcook.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hck.uphjek.com

Ruby: s.split(",");  s.split
来源：http://wim.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bys.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://ttu.gogol.net.cn

Py:   ",".join(items)
来源：http://psi.52xcode.cn

PHP:  implode(",", $items);
来源：http://eve.dianchejie.cn

JS:   items.join(",")
来源：http://xnq.aizwys.cn

TS:   items.join(",")
来源：http://bvo.quarkkingdee.top

Java: String.join(",", items)
来源：http://fsc.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://qqm.nwbrower.top

Ruby: items.join(",")
来源：http://zdw.mhx1999.top

C#:   string.Join(",", items)
来源：http://tzb.yj202588.top

[E09] 去除所有空白字符
来源：http://bab.jinghuilouyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zrj.hesvh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lun.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://tan.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://guk.xinyue.icu

Java: s.replaceAll("\\s+", "")
来源：http://diu.zhoulong.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://cgn.hnxiangtu.top

Ruby: s.gsub(/\s+/, "")
来源：http://sxl.quarkkingdee.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nyn.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://goc.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ebn.jinqigufen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mez.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://bpy.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://naw.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://eda.cheryme.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lmg.nwbrower.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://otk.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jxa.cucudq.cn

[E11] 反转字符串
来源：http://wos.9152youxi.cn

Py:   s[::-1]
来源：http://gkp.fengsongda.top

PHP:  strrev($s);
来源：http://sjn.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://atg.yangfankeji.com

TS:   [...s].reverse().join("")
来源：http://ytx.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kff.redwolf501.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://esv.fzhhl.top

Ruby: s.reverse
来源：http://con.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://opk.guannengcc.top

[E12] 统计某字符出现次数
来源：http://kal.pengpengdd.cyou

Py:   s.count("a")
来源：http://gmh.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://fjx.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://fni.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://zid.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rao.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://ynh.cashguo.top

Ruby: s.count("a")
来源：http://owl.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://msl.yj20258.top

[E13] 逐字符遍历
来源：http://cgb.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://tsw.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lqi.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zkw.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cvn.uphjek.com


<!-- 参考信息 -->