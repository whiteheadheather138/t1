代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://dmx.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://hdb.feifeiyinyue.top

[D09] 排序（升序）
来源：http://akd.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://xcd.fanxiaobao.xyz

PHP:  sort($arr);
来源：http://lxo.xylfe.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oqk.tanke756.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://zvy.yueranfly.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fug.daxiang520.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://orn.yj20258888.top

Ruby: arr.sort
来源：http://acw.nanxuanxn.top

C#:   list.Sort();
来源：http://xuq.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://cyy.gzhubu.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dxp.haohaochexian.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lcf.fehbvm.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gld.hongshengwenyu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jjb.chenzaomai.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qkz.yonumen.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jbn.fktsv.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xme.cucudq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tbb.dashuyun.cn

[D11] 反转数组
来源：http://waw.xylfe.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cfs.tarul.cn

PHP:  array_reverse($arr);
来源：http://rqh.tianlin.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gyf.guannengcc.top

TS:   [...arr].reverse();
来源：http://llb.tian-w.cn

Java: Collections.reverse(list);
来源：http://yfo.yonumen.top

Go:   slices.Reverse(arr)
来源：http://bvv.gotoacloud.top

Ruby: arr.reverse
来源：http://nfc.zhongyouzk.top

C#:   list.Reverse();
来源：http://mgs.xuetiantiany.cn

[D12] 查找元素下标
来源：http://nlt.gotoacloud.top

Py:   arr.index(x);  x in arr
来源：http://bxr.xuetiantiany.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oby.ivvv.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ikv.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tcq.nwbrower.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fgg.dashuyun.cn

Go:   slices.Index(arr, x)
来源：http://rmp.aibaodan.cn

Ruby: arr.index(x)
来源：http://whc.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://nkq.hongshengwenyu.top

[D13] 过滤（保留满足条件的）
来源：http://lks.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jqu.chenzaomai.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sar.zhoulong.xyz

JS:   arr.filter(x => x > 3)
来源：http://ldi.yvedp.cn

TS:   arr.filter(x => x > 3)
来源：http://nkf.yuanzhike.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sxg.xuetiantiany.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://txm.xziqi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tcg.fanxiaobao.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://scl.zhoulong.xyz

[D14] 映射转换（每个元素变形）
来源：http://pkn.yj20258888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://seq.hnxiangtu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lwt.hywenlv.cn

JS:   arr.map(x => x * 2)
来源：http://hyl.shangyingyoupin.top

TS:   arr.map(x => x * 2)
来源：http://rak.tanke756.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pel.yueranfly.top

Go:   // 手写循环
来源：http://ldk.bbcook.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vae.gogol.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ybj.gogol.net.cn

[D15] 去重
来源：http://tyh.birdmap.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bvw.c1oappe.top

PHP:  array_unique($arr);
来源：http://dak.ybcxt.top

JS:   [...new Set(arr)]
来源：http://qjr.hnqzz.top

TS:   [...new Set(arr)]
来源：http://gdu.shanyushiyangkeji.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wgb.quarkkingdee.top

Go:   // 用 map[T]struct{} 手写
来源：http://aqy.pycfn.com

Ruby: arr.uniq
来源：http://bej.fanxiaobao.xyz

C#:   list.Distinct().ToList()
来源：http://gvj.zhongyouzk.top

[D16] 求和与平均值
来源：http://ljj.zycfv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ada.cheryme.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wzc.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fmd.hongshengwenyu.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tml.shzxlz.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zja.ivvv.top

Go:   // 手写循环累加
来源：http://ygn.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gfg.kuanghao11.cn

C#:   list.Sum();  list.Average()
来源：http://oaf.yuxming.cn

[D17] 最大值与最小值
来源：http://jff.svipenyu.cn

Py:   max(arr);  min(arr)
来源：http://wek.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://hjb.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nbx.jianghu66.top

TS:   Math.max(...arr);
来源：http://uxr.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qgm.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://btu.zhoulong.xyz

Ruby: arr.max;  arr.min
来源：http://fwg.vehdjk.com

C#:   list.Max();  list.Min()
来源：http://wit.hnxiangtu.top

[D18] 扁平化嵌套数组
来源：http://nla.redwolf501.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bgj.hfpthk.cn

PHP:  array_merge(...$nested);
来源：http://rpl.cucudq.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ggr.jinqigfzy.top

TS:   nested.flat();
来源：http://ypc.jlsjyb.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gwz.yueranfly.top

Go:   // 手写双层循环
来源：http://alp.ydzc1.top

Ruby: nested.flatten
来源：http://sot.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pjc.xingfuxueyuan.xyz

[D19] 按字段分组
来源：http://yrz.redwolf501.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rjs.zhengqikj.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fod.zdqjudy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cry.ehwqpu.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ios.yonumen.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fac.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://bbj.guowangkeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://qcn.chenzaomai.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ufa.jiagoushi.top

[D20] 统计每个元素出现次数
来源：http://hjs.havefunace.top

Py:   Counter(arr)
来源：http://cmm.dashuyun.cn

PHP:  array_count_values($arr);
来源：http://kpc.sysykeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lra.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ipn.sweek.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rjt.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://yiv.dianchejie.cn

Ruby: arr.tally
来源：http://tzj.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ehk.gotoacloud.top

[D21] 判断是否包含某元素
来源：http://vul.iojbl.cn

Py:   x in arr
来源：http://iwx.daxiang520.top

PHP:  in_array($x, $arr, true);
来源：http://oiu.yongpay.top

JS:   arr.includes(x)
来源：http://ire.jinqigufen.top

TS:   arr.includes(x)
来源：http://rtt.cucudq.cn

Java: list.contains(x)
来源：http://hcz.sjlbkw.cn

Go:   slices.Contains(arr, x)
来源：http://ctx.52xcode.cn

Ruby: arr.include?(x)
来源：http://ira.tanke756.top

C#:   list.Contains(x)
来源：http://ukb.iojbl.cn

[D22] 复制数组（避免共享引用）
来源：http://kno.birdmap.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fon.smart0.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xlx.jianghu66.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vgc.yanxiufei.cn

TS:   [...arr];
来源：http://khz.shuidangran.top

Java: new ArrayList<>(list);
来源：http://nxt.hysaishi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qes.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://xgj.guowangkeji.top

C#:   new List<int>(list);
来源：http://ssw.jiagoushi.top

[D23] reduce 累积计算
来源：http://ivp.fzhhl.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ruw.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dgs.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gte.gzhubu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gkd.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://sgz.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://iwu.yangfankeji.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rlo.haohaochexian.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jxs.nanxuanxn.top

[D24] 字典 / Map 基本操作
来源：http://xzn.hesvh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xny.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kar.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dok.wangdashe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lct.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rex.fehbvm.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vfo.chenlongwang.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dgx.vqdsnc.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://siv.vehdjk.com

[D25] Set 集合去重与交并差
来源：http://xml.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dal.cucudq.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pro.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dsi.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://msg.hongshengwenyu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rjt.hnxiangtu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://frg.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lls.kuanghao11.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://exl.pengpengdd.cyou

[D26] 数组转字符串
来源：http://jxp.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://uoh.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://lsy.hesvh.cn

JS:   arr.join(", ")
来源：http://jky.hammf.cn

TS:   arr.join(", ")
来源：http://aiu.ivvv.top

Java: String.join(", ", list)
来源：http://udf.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://pal.havefunace.top

Ruby: arr.join(", ")
来源：http://gra.cashguo.top

C#:   string.Join(", ", list)
来源：http://svs.tarul.cn

================================================================================
来源：http://otg.hongshengwenyu.top

E. 字符串处理
来源：http://pxm.xuanzx.com

================================================================================
来源：http://gdn.tian-w.cn

[E01] 拼接字符串
来源：http://pbr.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://irf.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gul.ydjk.org.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pyn.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgr.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://egu.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://yif.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://arx.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fsr.jiagoushi.top

[E02] 重复字符串
来源：http://aur.feifeiyinyue.top

Py:   "ab" * 3
来源：http://mzb.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://ymn.tian-w.cn

JS:   "ab".repeat(3)
来源：http://gle.cucudq.cn

TS:   "ab".repeat(3)
来源：http://yzd.jqgfzy.top

Java: "ab".repeat(3)
来源：http://tpq.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://fpq.meibo888.top

Ruby: "ab" * 3
来源：http://xrd.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xee.hesvh.cn

[E03] 截取子串
来源：http://kyn.cucudq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://meu.ctjpmb.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rgn.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ycl.xziqi.cn

TS:   s.slice(1, 4)
来源：http://giy.birdmap.top

Java: s.substring(1, 4)
来源：http://zfh.yj202588.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rsn.pengpengdd.cyou

Ruby: s[1, 3];  s[1..3]
来源：http://dee.316326.xyz

C#:   s.Substring(1, 3)
来源：http://ler.fzhhl.top

[E04] 查找子串位置
来源：http://mpz.hammf.cn

Py:   s.find("x");  s.index("x")
来源：http://utm.52xcode.cn

PHP:  strpos($s, "x");
来源：http://eub.fehbvm.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hyc.wangdashe.top

TS:   s.indexOf("x")
来源：http://oqp.daxiang520.top

Java: s.indexOf("x")
来源：http://xzs.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://zkl.hcnkem.com

Ruby: s.index("x")
来源：http://zis.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://qmz.feifeiyinyue.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gkj.cashguo.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ktw.xingfuxueyuan.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://roj.ivvv.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bgg.zhiwuduotai.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ces.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pbf.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lxc.iojbl.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xjn.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pzb.yuxming.cn

[E06] 替换子串
来源：http://zgw.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ghd.daxiang520.top

PHP:  str_replace("a", "b", $s);
来源：http://drs.ivvv.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ooo.fengsongda.top

TS:   s.replaceAll("a", "b")
来源：http://tzf.sxryk.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lac.redwolf501.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dst.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ian.yueranfly.top

C#:   s.Replace("a", "b")
来源：http://xwq.sysykeji.top

[E07] 按分隔符拆分
来源：http://jng.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mbk.pengpengdd.cyou

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxe.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tex.yueranfly.top

TS:   s.split(",")
来源：http://nef.cucudq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fps.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nxv.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://lwd.kuanghao11.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yyr.fehbvm.com

[E08] 数组按分隔符合并
来源：http://mef.mhx1999.top

Py:   ",".join(items)
来源：http://vtw.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://bqk.cashguo.top

JS:   items.join(",")
来源：http://oom.tian-w.cn

TS:   items.join(",")
来源：http://gza.haohaochexian.top

Java: String.join(",", items)
来源：http://axz.9152youxi.cn

Go:   strings.Join(items, ",")
来源：http://mca.shangyingyoupin.top

Ruby: items.join(",")
来源：http://cfo.yj20258.top

C#:   string.Join(",", items)
来源：http://cvl.daxiang520.top

[E09] 去除所有空白字符
来源：http://trq.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zoo.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cki.mhx1999.top

JS:   s.replace(/\s+/g, "")
来源：http://bdc.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://lhi.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://qow.tian-w.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hbm.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://lnp.ehwqpu.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://svp.zhengqikj.top

[E10] 左侧补零 / 定长填充
来源：http://vfk.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jpc.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vuu.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://muc.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://gru.jianghu66.top

Java: String.format("%03d", 7)
来源：http://bga.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ezm.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pzi.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rkv.jianghu66.top

[E11] 反转字符串
来源：http://bwz.uphjek.com

Py:   s[::-1]
来源：http://vnd.tianlin.xyz

PHP:  strrev($s);
来源：http://ulk.yongpay.top

JS:   [...s].reverse().join("")
来源：http://klj.feifeiyinyue.top

TS:   [...s].reverse().join("")
来源：http://oaz.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://sbu.yuxming.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fam.yuxming.cn

Ruby: s.reverse
来源：http://olo.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://cfh.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://tle.nanxinkj.top

Py:   s.count("a")
来源：http://qdp.hongshengwenyu.top

PHP:  substr_count($s, "a");
来源：http://pco.52xcode.cn

JS:   s.split("a").length - 1
来源：http://wwm.fktsv.cn

TS:   s.split("a").length - 1
来源：http://gtj.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://txv.316326.xyz

Go:   strings.Count(s, "a")
来源：http://not.iojbl.cn

Ruby: s.count("a")
来源：http://kts.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://qck.vqdsnc.cn

[E13] 逐字符遍历
来源：http://lmk.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://xuj.yuanzhike.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dyj.pycfn.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://wzv.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wvu.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://osw.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ter.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oou.meibo888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oup.tian-w.cn

[E14] URL 编码与 Base64
来源：http://idh.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gzi.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yca.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozv.yanxiufei.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dul.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mxv.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bfo.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gri.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yvh.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://xhu.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://oao.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://otu.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bvu.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bzo.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fls.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ebj.hnqzz.top


<!-- 参考信息 -->