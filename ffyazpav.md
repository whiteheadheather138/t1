代发 wailian999

Py:   len(arr)
来源：http://xlb.zdbjq.cn

PHP:  count($arr);
来源：http://flh.cheryme.top

JS:   arr.length
来源：http://jhd.andypj.xyz

TS:   arr.length
来源：http://kmy.meibo888.top

Java: list.size();
来源：http://pnn.hfpthk.cn

Go:   len(arr)
来源：http://ala.xuanzx.com

Ruby: arr.length; arr.size
来源：http://vto.gaohongyu789.top

C#:   list.Count;
来源：http://pvh.jinqigufen.top

[D07] 切片 / 取子数组
来源：http://mgi.316326.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://sar.ppjwa.cn

PHP:  array_slice($arr, 1, 3);
来源：http://kay.redwolf501.top

JS:   arr.slice(1, 4);
来源：http://dyf.hammf.cn

TS:   arr.slice(1, 4);
来源：http://ufl.aizwys.cn

Java: list.subList(1, 4);
来源：http://hsz.ctjpmb.com

Go:   arr[1:4]
来源：http://wmu.zhongyouzk.top

Ruby: arr[1, 3]
来源：http://fnv.ydjk.org.cn

C#:   list.GetRange(1, 3);
来源：http://nkf.jiagoushi.top

[D08] 合并两个数组
来源：http://xyr.xuanzx.com

Py:   a + b;  a.extend(b)
来源：http://fpi.0kj1m.cn

PHP:  array_merge($a, $b);
来源：http://mrl.gaohongyu789.top

JS:   [...a, ...b];  a.concat(b);
来源：http://rmc.yonumen.top

TS:   [...a, ...b];
来源：http://qrq.redwolf501.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jic.birdmap.top

Go:   append(a, b...)
来源：http://dzd.smart0.xyz

Ruby: a + b;  a.concat(b)
来源：http://mpn.haohaochexian.top

C#:   a.Concat(b).ToList()
来源：http://xfl.9152youxi.cn

[D09] 排序（升序）
来源：http://wsm.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://nbu.jinghuilouyu.cn

PHP:  sort($arr);
来源：http://cfd.hysaishi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfv.ydjk.org.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zoy.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wll.316326.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wao.guowangkeji.top

Ruby: arr.sort
来源：http://eud.chenjidiqi.icu

C#:   list.Sort();
来源：http://mob.yuanzhike.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bjh.zhaomingkeji.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rap.316326.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kjc.jiagoushi.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bor.zdqjudy.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wov.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ibh.yfazqb.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xkd.0kj1m.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jvv.52xcode.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zmv.xuetiantiany.cn

[D11] 反转数组
来源：http://okn.c1oappe.top

Py:   arr[::-1];  arr.reverse()
来源：http://ndu.vqdsnc.cn

PHP:  array_reverse($arr);
来源：http://mvi.yonumen.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gmx.cashguo.top

TS:   [...arr].reverse();
来源：http://kym.bbcook.cn

Java: Collections.reverse(list);
来源：http://fvr.pengpengdd.cyou

Go:   slices.Reverse(arr)
来源：http://oyv.hfpthk.cn

Ruby: arr.reverse
来源：http://dgh.sufxvd.cn

C#:   list.Reverse();
来源：http://bcj.quarkkingdee.top

[D12] 查找元素下标
来源：http://tra.sysykeji.top

Py:   arr.index(x);  x in arr
来源：http://uav.shzxlz.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://omb.jiagoushi.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dat.chenjidiqi.icu

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gzc.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bwv.hywenlv.cn

Go:   slices.Index(arr, x)
来源：http://psa.quarkkingdee.top

Ruby: arr.index(x)
来源：http://blu.yonumen.top

C#:   list.IndexOf(x);
来源：http://uds.yueranfly.top

[D13] 过滤（保留满足条件的）
来源：http://sbm.jqgfzy.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iik.yj202588.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uoe.ybcxt.top

JS:   arr.filter(x => x > 3)
来源：http://igs.xuanzx.com

TS:   arr.filter(x => x > 3)
来源：http://oky.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yku.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nhv.yj202588.top

Ruby: arr.select { |x| x > 3 }
来源：http://kri.hongshengwenyu.top

C#:   list.Where(x => x > 3).ToList()
来源：http://zvf.ppjwa.cn

[D14] 映射转换（每个元素变形）
来源：http://ogq.zycfv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://scm.aibaodan.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://gbw.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://nyr.yj20258.top

TS:   arr.map(x => x * 2)
来源：http://vgo.cashguo.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://znx.jinghuilouyu.cn

Go:   // 手写循环
来源：http://ivv.sweek.top

Ruby: arr.map { |x| x * 2 }
来源：http://ckc.ehwqpu.com

C#:   list.Select(x => x * 2).ToList()
来源：http://lvi.yanxiufei.cn

[D15] 去重
来源：http://hbn.yanxiufei.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jfk.feifeiyinyue.top

PHP:  array_unique($arr);
来源：http://jqk.birdmap.top

JS:   [...new Set(arr)]
来源：http://ruv.chenzaomai.com

TS:   [...new Set(arr)]
来源：http://iwt.gzhubu.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mda.hongshengwenyu.top

Go:   // 用 map[T]struct{} 手写
来源：http://pvj.9152youxi.cn

Ruby: arr.uniq
来源：http://pfb.ybcxt.top

C#:   list.Distinct().ToList()
来源：http://vlm.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://ndz.hfpthk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://spi.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cfk.shuidangran.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lsu.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://amp.fzhhl.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mqt.hnxiangtu.top

Go:   // 手写循环累加
来源：http://gna.chenjidiqi.icu

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dkg.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://rcr.yonumen.top

[D17] 最大值与最小值
来源：http://obe.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://bkf.jinqigufen.top

PHP:  max($arr);  min($arr);
来源：http://kie.ydjk.org.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wdh.yfazqb.com

TS:   Math.max(...arr);
来源：http://pie.sxryk.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mev.shanyushiyangtech.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mqn.gzhubu.top

Ruby: arr.max;  arr.min
来源：http://ben.guannengcc.top

C#:   list.Max();  list.Min()
来源：http://pfj.hammf.cn

[D18] 扁平化嵌套数组
来源：http://pqi.daria6918.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://end.mhx1999.top

PHP:  array_merge(...$nested);
来源：http://nxu.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qwx.aibaodan.cn

TS:   nested.flat();
来源：http://ajq.9152youxi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xms.zhoulong.xyz

Go:   // 手写双层循环
来源：http://wzr.aibaodan.cn

Ruby: nested.flatten
来源：http://vsh.zdqjudy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://anf.cheryme.top

[D19] 按字段分组
来源：http://gqh.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kpf.ehwqpu.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qce.yfazqb.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mgo.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://adl.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mia.tarul.cn

Go:   // 手写 map[string][]T
来源：http://plf.epnwcf.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://mdn.yanxiufei.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ilt.ydzc1.top

[D20] 统计每个元素出现次数
来源：http://ztv.smart0.xyz

Py:   Counter(arr)
来源：http://qam.andypj.xyz

PHP:  array_count_values($arr);
来源：http://dov.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://knw.vehdjk.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wtj.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://eji.pengpengdd.cyou

Go:   // 手写 map[T]int
来源：http://tbg.bbcook.cn

Ruby: arr.tally
来源：http://bxq.yongpay.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbe.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://xws.xziqi.cn

Py:   x in arr
来源：http://tpr.sysykeji.top

PHP:  in_array($x, $arr, true);
来源：http://nnb.jinqigufen.top

JS:   arr.includes(x)
来源：http://gdx.guannengcc.top

TS:   arr.includes(x)
来源：http://wyz.gotoacloud.top

Java: list.contains(x)
来源：http://zzh.hywenlv.cn

Go:   slices.Contains(arr, x)
来源：http://dbh.fengsongda.top

Ruby: arr.include?(x)
来源：http://msz.zhoulong.xyz

C#:   list.Contains(x)
来源：http://dhl.sjlbkw.cn

[D22] 复制数组（避免共享引用）
来源：http://fbm.xinyue.icu

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hek.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mdd.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xmr.jinqigfzy.top

TS:   [...arr];
来源：http://vsa.epnwcf.com

Java: new ArrayList<>(list);
来源：http://hbn.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://apk.bbcook.cn

Ruby: arr.dup;  arr.clone
来源：http://lil.xuetiantiany.cn

C#:   new List<int>(list);
来源：http://dcc.gzhubu.top

[D23] reduce 累积计算
来源：http://kez.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vrw.ehwqpu.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ilu.jinghuilouyu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xlt.yangfankeji.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dmf.snrcjt.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bvg.meibo888.top

Go:   // 手写循环
来源：http://qal.tian-w.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ptk.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ftq.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://mcw.hcnkem.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blp.tanke756.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cae.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aba.hywenlv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://foq.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gso.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xau.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://syk.jinqigfzy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hvm.daxiang520.top

[D25] Set 集合去重与交并差
来源：http://tqy.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ech.shanyushiyangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://muf.mhx1999.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://twy.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ofa.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://bcx.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ole.feifeiyinyue.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qgj.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nkm.cdnleiting.top

[D26] 数组转字符串
来源：http://gox.jinghuilouyu.cn

Py:   ", ".join(map(str, arr))
来源：http://qpk.zdbjq.cn

PHP:  implode(", ", $arr);
来源：http://vtj.yongpay.top

JS:   arr.join(", ")
来源：http://ogt.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://idz.jqgfzy.top

Java: String.join(", ", list)
来源：http://irg.birdmap.top

Go:   strings.Join(strs, ", ")
来源：http://obw.daxiang520.top

Ruby: arr.join(", ")
来源：http://vda.zycfv.cn

C#:   string.Join(", ", list)
来源：http://dyc.xinyue.icu

================================================================================
来源：http://qzo.vehdjk.com

E. 字符串处理
来源：http://rta.yfazqb.com

================================================================================
来源：http://vyb.gotoacloud.top

[E01] 拼接字符串
来源：http://riv.ehwqpu.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fvs.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gnl.feifeiyinyue.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gjg.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rkc.yfazqb.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wlc.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nyk.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xzj.shangyingyoupin.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zlu.nwbrower.top

[E02] 重复字符串
来源：http://lap.pycfn.com

Py:   "ab" * 3
来源：http://ics.cashguo.top

PHP:  str_repeat("ab", 3);
来源：http://rwz.yongpay.top

JS:   "ab".repeat(3)
来源：http://wqc.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://ecu.daria6918.cn

Java: "ab".repeat(3)
来源：http://ixs.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://cot.guowangkeji.top

Ruby: "ab" * 3
来源：http://uzn.yj20258888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zmh.birdmap.top

[E03] 截取子串
来源：http://qyw.kuanghao11.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mpz.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yar.tanke756.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hrj.gogol.net.cn

TS:   s.slice(1, 4)
来源：http://sac.fehbvm.com

Java: s.substring(1, 4)
来源：http://drn.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sku.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hqf.vqdsnc.cn

C#:   s.Substring(1, 3)
来源：http://oeh.guowangkeji.top

[E04] 查找子串位置
来源：http://zdg.yfazqb.com

Py:   s.find("x");  s.index("x")
来源：http://sgp.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://zmc.zhoulong.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nud.yfazqb.com

TS:   s.indexOf("x")
来源：http://uro.birdmap.top

Java: s.indexOf("x")
来源：http://jej.316326.xyz

Go:   strings.Index(s, "x")
来源：http://rqz.fktsv.cn

Ruby: s.index("x")
来源：http://owk.yj20258888.top

C#:   s.IndexOf("x")
来源：http://tqt.yangfankeji.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://kaw.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://foo.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rdp.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jxr.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ynh.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xrf.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ovg.yanxiufei.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ukm.zhixingplan.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oxb.guannengcc.top

[E06] 替换子串
来源：http://lce.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aeo.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://ckq.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbe.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://qxr.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qud.cashguo.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cev.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ono.fzhhl.top

C#:   s.Replace("a", "b")
来源：http://ool.shzxlz.cn

[E07] 按分隔符拆分
来源：http://doa.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://okz.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wba.haohaochexian.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bag.guannengcc.top

TS:   s.split(",")
来源：http://fgq.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://aaf.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://szq.chenlongwang.top

Ruby: s.split(",");  s.split
来源：http://dfn.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kvy.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://cxk.yj20258888.top

Py:   ",".join(items)
来源：http://wqr.ybcxt.top

PHP:  implode(",", $items);
来源：http://dlz.jqgfzy.top

JS:   items.join(",")
来源：http://lmg.hammf.cn

TS:   items.join(",")
来源：http://kan.ydzc1.top

Java: String.join(",", items)
来源：http://qou.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://yhh.ivvv.top

Ruby: items.join(",")
来源：http://klh.yuanzhike.top

C#:   string.Join(",", items)
来源：http://uuj.pycfn.com

[E09] 去除所有空白字符
来源：http://ccw.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ykk.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rat.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://fur.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://nad.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://isw.nwbrower.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mpx.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://qyg.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ktu.daxiang520.top

[E10] 左侧补零 / 定长填充
来源：http://awy.cdnleiting.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://who.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qge.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://oqj.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://alf.52xcode.cn

Java: String.format("%03d", 7)
来源：http://tue.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cwl.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hax.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rzt.shanyushiyangtech.top

[E11] 反转字符串
来源：http://ekm.hammf.cn

Py:   s[::-1]
来源：http://ngb.haohaochexian.top

PHP:  strrev($s);
来源：http://nor.yongpay.top

JS:   [...s].reverse().join("")
来源：http://xij.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://ven.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cgf.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dux.jyoumei.cn

Ruby: s.reverse
来源：http://yat.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://zlr.yj202588.top

[E12] 统计某字符出现次数
来源：http://scp.kuanghao11.cn

Py:   s.count("a")
来源：http://ebw.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://cww.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://eew.hysaishi.cn

TS:   s.split("a").length - 1
来源：http://vyb.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://owi.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://qet.aizwys.cn

Ruby: s.count("a")
来源：http://qrc.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://qtm.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://wjl.zhixingplan.top


<!-- 参考信息 -->