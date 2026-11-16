代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://imo.ppjwa.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://bbu.shanyushiyangkeji.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nyx.chenjidiqi.icu

[D06] 数组长度
来源：http://afp.hammf.cn

Py:   len(arr)
来源：http://fcm.birdmap.top

PHP:  count($arr);
来源：http://cjg.yueranfly.top

JS:   arr.length
来源：http://bgy.svipenyu.cn

TS:   arr.length
来源：http://qvu.sjlbkw.cn

Java: list.size();
来源：http://lat.pengpengdd.cyou

Go:   len(arr)
来源：http://rce.sweek.top

Ruby: arr.length; arr.size
来源：http://apv.ybcxt.top

C#:   list.Count;
来源：http://zvv.ppjwa.cn

[D07] 切片 / 取子数组
来源：http://bhq.daria6918.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jnr.yuxming.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lls.jianghu66.top

JS:   arr.slice(1, 4);
来源：http://qge.jqgufenzy.top

TS:   arr.slice(1, 4);
来源：http://nky.ydzc1.top

Java: list.subList(1, 4);
来源：http://mvg.cheryme.top

Go:   arr[1:4]
来源：http://ppd.sxryk.cn

Ruby: arr[1, 3]
来源：http://xdf.9152youxi.cn

C#:   list.GetRange(1, 3);
来源：http://htp.ehwqpu.com

[D08] 合并两个数组
来源：http://zgm.gotoacloud.top

Py:   a + b;  a.extend(b)
来源：http://mmm.xuanzx.com

PHP:  array_merge($a, $b);
来源：http://fxx.gzhubu.top

JS:   [...a, ...b];  a.concat(b);
来源：http://wvo.fanxiaobao.xyz

TS:   [...a, ...b];
来源：http://qvs.zycfv.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ead.hongshengwenyu.top

Go:   append(a, b...)
来源：http://qlw.zhijiandao.cn

Ruby: a + b;  a.concat(b)
来源：http://shz.tarul.cn

C#:   a.Concat(b).ToList()
来源：http://hed.kuanghao11.cn

[D09] 排序（升序）
来源：http://vtb.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://opo.jinyuanbaomall.cn

PHP:  sort($arr);
来源：http://nfw.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ngx.cashguo.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://kih.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://abi.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zmn.chenzaomai.com

Ruby: arr.sort
来源：http://bpg.yuxming.cn

C#:   list.Sort();
来源：http://zxq.zhongyouzk.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://yae.ehwqpu.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lkc.epnwcf.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zlt.jianghu66.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bds.ivvv.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qqf.epnwcf.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wgz.hcnkem.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jru.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lms.aibaodan.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ljg.ydzc1.top

[D11] 反转数组
来源：http://tbm.daria6918.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yag.hammf.cn

PHP:  array_reverse($arr);
来源：http://see.jinqigfzy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ncq.yanxiufei.cn

TS:   [...arr].reverse();
来源：http://qdt.ehwqpu.com

Java: Collections.reverse(list);
来源：http://pur.jqgfzy.top

Go:   slices.Reverse(arr)
来源：http://pgx.yangfankeji.com

Ruby: arr.reverse
来源：http://xpx.guannengcc.top

C#:   list.Reverse();
来源：http://rvc.quarkkingdee.top

[D12] 查找元素下标
来源：http://jxp.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://eaw.iojbl.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ckk.vehdjk.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lfl.jinqigfzy.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ito.xuanzx.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://roi.ehwqpu.com

Go:   slices.Index(arr, x)
来源：http://fng.kuanghao11.cn

Ruby: arr.index(x)
来源：http://nke.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://ijk.aizwys.cn

[D13] 过滤（保留满足条件的）
来源：http://loj.pycfn.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://oia.yj20258888.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vrw.hongshengwenyu.top

JS:   arr.filter(x => x > 3)
来源：http://doy.tianlin.xyz

TS:   arr.filter(x => x > 3)
来源：http://skl.cheryme.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://avz.cqqwz.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://kpa.bjfxy.top

Ruby: arr.select { |x| x > 3 }
来源：http://zmi.gogol.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hna.sufxvd.cn

[D14] 映射转换（每个元素变形）
来源：http://zoh.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://iht.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://crq.yj20258888.top

JS:   arr.map(x => x * 2)
来源：http://dhq.jinghuilouyu.cn

TS:   arr.map(x => x * 2)
来源：http://ymx.cheryme.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ijb.andypj.xyz

Go:   // 手写循环
来源：http://wsp.xylfe.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cyz.yueranfly.top

C#:   list.Select(x => x * 2).ToList()
来源：http://rxc.52xcode.cn

[D15] 去重
来源：http://tyq.xziqi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kcm.havefunace.top

PHP:  array_unique($arr);
来源：http://daa.bjfxy.top

JS:   [...new Set(arr)]
来源：http://krz.sweek.top

TS:   [...new Set(arr)]
来源：http://ncj.gaohongyu789.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lyk.redwolf501.top

Go:   // 用 map[T]struct{} 手写
来源：http://bzm.nwbrower.top

Ruby: arr.uniq
来源：http://rem.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://npk.wangdashe.top

[D16] 求和与平均值
来源：http://jqd.yuxming.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fno.0kj1m.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pwn.chenzaomai.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cgq.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://oti.shanyushiyangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zaw.yongpay.top

Go:   // 手写循环累加
来源：http://tfo.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uzf.hesvh.cn

C#:   list.Sum();  list.Average()
来源：http://swu.gzhubu.top

[D17] 最大值与最小值
来源：http://bdy.ydzc1.top

Py:   max(arr);  min(arr)
来源：http://ptw.ppjwa.cn

PHP:  max($arr);  min($arr);
来源：http://lpj.sufxvd.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hry.ctjpmb.com

TS:   Math.max(...arr);
来源：http://alb.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xrs.yvedp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ftz.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://hhf.ehwqpu.com

C#:   list.Max();  list.Min()
来源：http://jdf.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://wvc.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xcx.zhixingplan.top

PHP:  array_merge(...$nested);
来源：http://byc.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://oov.zhiwuduotai.top

TS:   nested.flat();
来源：http://mju.pycfn.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qtw.zdbjq.cn

Go:   // 手写双层循环
来源：http://hvk.ctjpmb.com

Ruby: nested.flatten
来源：http://stx.tianlin.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://xme.sufxvd.cn

[D19] 按字段分组
来源：http://nyr.xylfe.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ocb.wangdashe.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ott.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fqh.zhaomingkeji.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://ztk.zhengqikj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ujg.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://fcx.meibo888.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mlf.jinqigufen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://urg.havefunace.top

[D20] 统计每个元素出现次数
来源：http://svf.yueranfly.top

Py:   Counter(arr)
来源：http://iau.xinyue.icu

PHP:  array_count_values($arr);
来源：http://xbf.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgf.nanxuanxn.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://izz.gogol.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pwf.hesvh.cn

Go:   // 手写 map[T]int
来源：http://euw.xylfe.cn

Ruby: arr.tally
来源：http://doe.sweek.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qct.wangdashe.top

[D21] 判断是否包含某元素
来源：http://fsm.smart0.xyz

Py:   x in arr
来源：http://ycq.bjfxy.top

PHP:  in_array($x, $arr, true);
来源：http://ide.sxryk.cn

JS:   arr.includes(x)
来源：http://eac.yangfankeji.com

TS:   arr.includes(x)
来源：http://fcd.jqgufenzy.top

Java: list.contains(x)
来源：http://lhd.gaohongyu789.top

Go:   slices.Contains(arr, x)
来源：http://xuo.ydzc1.top

Ruby: arr.include?(x)
来源：http://hfc.nanxinkj.top

C#:   list.Contains(x)
来源：http://sjr.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://ttr.tanke756.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wlu.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sym.yueranfly.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lth.pengpengdd.cyou

TS:   [...arr];
来源：http://ifn.haohaochexian.top

Java: new ArrayList<>(list);
来源：http://tpx.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ruf.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://vze.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://eut.redwolf501.top

[D23] reduce 累积计算
来源：http://aax.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ufw.zhaomingkeji.xyz

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xlx.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gkt.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzv.sysykeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://zow.xinyue.icu

Go:   // 手写循环
来源：http://yrl.ydjk.org.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pmd.jqgufenzy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yul.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://xfj.meibo888.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wpm.yj20258888.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhl.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wus.yangfankeji.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cap.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ywc.jianghu66.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mrq.guowangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qgf.kuanghao11.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hhr.sweek.top

[D25] Set 集合去重与交并差
来源：http://oyg.ydzc1.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aab.yj202588.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://flm.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lri.cashguo.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rds.pengpengdd.cyou

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vck.shanyushiyangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blp.yongpay.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eep.xuetiantiany.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lqi.0kj1m.cn

[D26] 数组转字符串
来源：http://hnv.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://yyn.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://exo.fanxiaobao.xyz

JS:   arr.join(", ")
来源：http://kmy.smart0.xyz

TS:   arr.join(", ")
来源：http://rye.jinghuilouyu.cn

Java: String.join(", ", list)
来源：http://rkl.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://eyz.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://okr.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://sdb.guannengcc.top

================================================================================
来源：http://lrq.nanxinkj.top

E. 字符串处理
来源：http://qwn.xziqi.cn

================================================================================
来源：http://bnh.vqdsnc.cn

[E01] 拼接字符串
来源：http://drd.sysykeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oce.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dia.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ydx.yj20258888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hsv.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://onb.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tek.cashguo.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wyf.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zmd.epnwcf.com

[E02] 重复字符串
来源：http://kta.jinqigufen.top

Py:   "ab" * 3
来源：http://rkk.sxryk.cn

PHP:  str_repeat("ab", 3);
来源：http://tkp.xylfe.cn

JS:   "ab".repeat(3)
来源：http://hyl.xingfuxueyuan.xyz

TS:   "ab".repeat(3)
来源：http://gis.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://xvd.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://nyq.jinyuanbaomall.cn

Ruby: "ab" * 3
来源：http://nst.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://loo.xuetiantiany.cn

[E03] 截取子串
来源：http://uhy.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvp.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ssv.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ota.tanke756.top

TS:   s.slice(1, 4)
来源：http://wwp.fengsongda.top

Java: s.substring(1, 4)
来源：http://qhm.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sji.havefunace.top

Ruby: s[1, 3];  s[1..3]
来源：http://bys.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://hsc.ctjpmb.com

[E04] 查找子串位置
来源：http://icw.xingfuxueyuan.xyz

Py:   s.find("x");  s.index("x")
来源：http://aap.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://mha.tianlin.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rgn.jiagoushi.top

TS:   s.indexOf("x")
来源：http://vqp.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://eus.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://ebj.gzhubu.top

Ruby: s.index("x")
来源：http://xyn.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://irx.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xxj.zhijiandao.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://adm.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pmh.wangshuangyany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jsy.jinghuilouyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://smc.yonumen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ufa.yuanzhike.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lye.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ocn.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aks.c1oappe.top

[E06] 替换子串
来源：http://ijf.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pfv.gotoacloud.top

PHP:  str_replace("a", "b", $s);
来源：http://mfl.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wug.9152youxi.cn

TS:   s.replaceAll("a", "b")
来源：http://oqp.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ets.shuidangran.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mpr.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ein.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://sow.dashuyun.cn

[E07] 按分隔符拆分
来源：http://mbd.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fjh.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rdo.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://otu.fzhhl.top

TS:   s.split(",")
来源：http://svs.tian-w.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ssx.ctjpmb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dfp.tarul.cn

Ruby: s.split(",");  s.split
来源：http://ldm.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cfw.bbcook.cn

[E08] 数组按分隔符合并
来源：http://vhr.svipenyu.cn

Py:   ",".join(items)
来源：http://wze.jiagoushi.top

PHP:  implode(",", $items);
来源：http://giu.cucudq.cn

JS:   items.join(",")
来源：http://riu.guowangkeji.top

TS:   items.join(",")
来源：http://ebp.jlsjyb.cn

Java: String.join(",", items)
来源：http://xsz.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://scq.gzhubu.top

Ruby: items.join(",")
来源：http://yoj.zhixingplan.top

C#:   string.Join(",", items)
来源：http://yfu.bjfxy.top

[E09] 去除所有空白字符
来源：http://twp.xingfuxueyuan.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nof.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kfp.hcnkem.com

JS:   s.replace(/\s+/g, "")
来源：http://sxv.hammf.cn

TS:   s.replace(/\s+/g, "")
来源：http://teg.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://way.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kfm.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dfn.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lgo.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://yjv.ehwqpu.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wha.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wjo.zhaomingkeji.xyz

JS:   "7".padStart(3, "0")
来源：http://eik.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://jwy.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://tth.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cbt.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rqn.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lqa.9152youxi.cn

[E11] 反转字符串
来源：http://kno.andypj.xyz

Py:   s[::-1]
来源：http://jvh.shuidangran.top

PHP:  strrev($s);
来源：http://qhp.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://uiu.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://zpe.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://luh.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lpi.dianchejie.cn

Ruby: s.reverse
来源：http://otv.yuxming.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qrn.xziqi.cn

[E12] 统计某字符出现次数
来源：http://fgz.dianchejie.cn

Py:   s.count("a")
来源：http://wtd.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://gwq.sxryk.cn

JS:   s.split("a").length - 1
来源：http://arn.ydzc1.top

TS:   s.split("a").length - 1
来源：http://sso.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dnt.fanxiaobao.xyz


<!-- 参考信息 -->