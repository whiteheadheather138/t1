代发 wailian999

TS:   arr.slice(1, 4);
来源：http://nxj.daria6918.cn

Java: list.subList(1, 4);
来源：http://xiv.pengpengdd.cyou

Go:   arr[1:4]
来源：http://cxy.hesvh.cn

Ruby: arr[1, 3]
来源：http://xxm.cheryme.top

C#:   list.GetRange(1, 3);
来源：http://xfv.xinyue.icu

[D08] 合并两个数组
来源：http://moa.ydzc1.top

Py:   a + b;  a.extend(b)
来源：http://txh.9152youxi.cn

PHP:  array_merge($a, $b);
来源：http://dnx.c1oappe.top

JS:   [...a, ...b];  a.concat(b);
来源：http://smr.hywenlv.cn

TS:   [...a, ...b];
来源：http://lvt.shuidangran.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gwp.wangdashe.top

Go:   append(a, b...)
来源：http://nts.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://svn.yongpay.top

C#:   a.Concat(b).ToList()
来源：http://gep.jlsjyb.cn

[D09] 排序（升序）
来源：http://kis.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://xwx.guannengcc.top

PHP:  sort($arr);
来源：http://uoo.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://icr.xuetiantiany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hid.dashuyun.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lgn.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kmx.gzhubu.top

Ruby: arr.sort
来源：http://dkh.yangfankeji.com

C#:   list.Sort();
来源：http://vpq.ctjpmb.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://lzo.jyoumei.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wyf.ybcxt.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dut.daria6918.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yzh.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://awf.fengsongda.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pig.sysykeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uou.zhijiandao.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mqj.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sja.jqgfzy.top

[D11] 反转数组
来源：http://vip.guowangkeji.top

Py:   arr[::-1];  arr.reverse()
来源：http://frf.jinghuilouyu.cn

PHP:  array_reverse($arr);
来源：http://eyj.tanke756.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://uir.nanxuanxn.top

TS:   [...arr].reverse();
来源：http://bhd.zhongyouzk.top

Java: Collections.reverse(list);
来源：http://ghz.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://jma.smart0.xyz

Ruby: arr.reverse
来源：http://did.hywenlv.cn

C#:   list.Reverse();
来源：http://ftp.birdmap.top

[D12] 查找元素下标
来源：http://llu.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://jti.hywenlv.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cwi.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zib.zhongyouzk.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rio.svipenyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://crt.cucudq.cn

Go:   slices.Index(arr, x)
来源：http://res.shzxlz.cn

Ruby: arr.index(x)
来源：http://emm.ivvv.top

C#:   list.IndexOf(x);
来源：http://vbq.yuxming.cn

[D13] 过滤（保留满足条件的）
来源：http://vqj.dashuyun.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gyh.316326.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kmw.yonumen.top

JS:   arr.filter(x => x > 3)
来源：http://fdl.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://ivp.jinghuilouyu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lqv.shuidangran.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yyb.ehwqpu.com

Ruby: arr.select { |x| x > 3 }
来源：http://tke.ydzc1.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ikt.sysykeji.top

[D14] 映射转换（每个元素变形）
来源：http://cfb.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uba.guannengcc.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kdr.9152youxi.cn

JS:   arr.map(x => x * 2)
来源：http://sus.gogol.net.cn

TS:   arr.map(x => x * 2)
来源：http://mba.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xge.zhiwuduotai.top

Go:   // 手写循环
来源：http://nah.sysykeji.top

Ruby: arr.map { |x| x * 2 }
来源：http://pat.redwolf501.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ntt.meibo888.top

[D15] 去重
来源：http://sgr.jinqigfzy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tbt.tanke756.top

PHP:  array_unique($arr);
来源：http://zgu.zycfv.cn

JS:   [...new Set(arr)]
来源：http://pht.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://cqy.yongpay.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rdv.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://alp.zycfv.cn

Ruby: arr.uniq
来源：http://xkp.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://fwt.yueranfly.top

[D16] 求和与平均值
来源：http://kkd.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wsx.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yak.hfpthk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fep.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pdr.ydjk.org.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bgr.yfazqb.com

Go:   // 手写循环累加
来源：http://ayn.guannengcc.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hon.chenlongwang.top

C#:   list.Sum();  list.Average()
来源：http://xno.fengsongda.top

[D17] 最大值与最小值
来源：http://qto.hywenlv.cn

Py:   max(arr);  min(arr)
来源：http://nga.zhixingplan.top

PHP:  max($arr);  min($arr);
来源：http://uop.yonumen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ddq.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://oyx.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://zvc.nanxinkj.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mrq.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://wja.jinqigfzy.top

C#:   list.Max();  list.Min()
来源：http://fqn.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://rnr.zhiwuduotai.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://poa.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://qhp.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xnz.wangdashe.top

TS:   nested.flat();
来源：http://mfr.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cok.yanxiufei.cn

Go:   // 手写双层循环
来源：http://akt.hammf.cn

Ruby: nested.flatten
来源：http://pon.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kta.jinghuilouyu.cn

[D19] 按字段分组
来源：http://qnn.meibo888.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zud.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bww.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lqd.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ihx.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qor.zhongyouzk.top

Go:   // 手写 map[string][]T
来源：http://nnu.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://owh.vqdsnc.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lek.316326.xyz

[D20] 统计每个元素出现次数
来源：http://pax.vqdsnc.cn

Py:   Counter(arr)
来源：http://yfc.cashguo.top

PHP:  array_count_values($arr);
来源：http://dep.jiagoushi.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gjf.ivvv.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mui.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tvx.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://rwp.jinyuanbaomall.cn

Ruby: arr.tally
来源：http://tsg.ivvv.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ujh.cucudq.cn

[D21] 判断是否包含某元素
来源：http://igf.52xcode.cn

Py:   x in arr
来源：http://vrh.yfazqb.com

PHP:  in_array($x, $arr, true);
来源：http://jjm.pycfn.com

JS:   arr.includes(x)
来源：http://cbv.hfpthk.cn

TS:   arr.includes(x)
来源：http://vui.jinqigufen.top

Java: list.contains(x)
来源：http://wvl.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://vmc.316326.xyz

Ruby: arr.include?(x)
来源：http://dnc.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://qab.xingfuxueyuan.xyz

[D22] 复制数组（避免共享引用）
来源：http://edv.daria6918.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mds.xylfe.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ufm.jyoumei.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bta.0kj1m.cn

TS:   [...arr];
来源：http://kdd.shanyushiyangkeji.top

Java: new ArrayList<>(list);
来源：http://jku.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://glb.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://txr.yangfankeji.com

C#:   new List<int>(list);
来源：http://vkz.daria6918.cn

[D23] reduce 累积计算
来源：http://hpg.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://amj.yongpay.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tfe.hfpthk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxv.aibaodan.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pvi.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://mmf.0kj1m.cn

Go:   // 手写循环
来源：http://eii.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fbw.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bzy.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://bxn.jianghu66.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gxe.redwolf501.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zyb.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ifl.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://chj.sysykeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jla.yongpay.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tbg.shanyushiyangkeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kcw.zhijiandao.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hyg.shangyingyoupin.top

[D25] Set 集合去重与交并差
来源：http://jgw.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fhz.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://flk.zycfv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fnp.316326.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wwc.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sws.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cud.sysykeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rhh.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pic.zhijiandao.cn

[D26] 数组转字符串
来源：http://ofm.kuanghao11.cn

Py:   ", ".join(map(str, arr))
来源：http://yyu.haohaochexian.top

PHP:  implode(", ", $arr);
来源：http://odk.yongpay.top

JS:   arr.join(", ")
来源：http://ibs.0kj1m.cn

TS:   arr.join(", ")
来源：http://gtq.sxryk.cn

Java: String.join(", ", list)
来源：http://rwk.dashuyun.cn

Go:   strings.Join(strs, ", ")
来源：http://tqa.iojbl.cn

Ruby: arr.join(", ")
来源：http://bkt.yuxming.cn

C#:   string.Join(", ", list)
来源：http://sxh.tian-w.cn

================================================================================
来源：http://hfu.fehbvm.com

E. 字符串处理
来源：http://cvv.zhiwuduotai.top

================================================================================
来源：http://gkw.sweek.top

[E01] 拼接字符串
来源：http://egh.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qct.zhaomingkeji.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vsc.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://geg.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vak.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xzn.quarkkingdee.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ozk.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://poy.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://egh.feifeiyinyue.top

[E02] 重复字符串
来源：http://nyr.zycfv.cn

Py:   "ab" * 3
来源：http://epu.svipenyu.cn

PHP:  str_repeat("ab", 3);
来源：http://pjf.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://ydz.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://fho.sysykeji.top

Java: "ab".repeat(3)
来源：http://uyb.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://wtp.uphjek.com

Ruby: "ab" * 3
来源：http://xzf.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nxs.hnqzz.top

[E03] 截取子串
来源：http://ccm.andypj.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jhi.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zmw.fengsongda.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iej.shanyushiyangkeji.top

TS:   s.slice(1, 4)
来源：http://tca.ydzc1.top

Java: s.substring(1, 4)
来源：http://uao.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vdv.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://wti.hywenlv.cn

C#:   s.Substring(1, 3)
来源：http://qcx.shanyushiyangkeji.top

[E04] 查找子串位置
来源：http://tax.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://wgl.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://czn.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wpq.bbcook.cn

TS:   s.indexOf("x")
来源：http://iou.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://zvt.nanxinkj.top

Go:   strings.Index(s, "x")
来源：http://qpv.nanxinkj.top

Ruby: s.index("x")
来源：http://xqr.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://gfh.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dqu.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xmq.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ksb.aizwys.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ory.yj20258888.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hdb.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hrv.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ubc.cqqwz.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tvi.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdq.gogol.net.cn

[E06] 替换子串
来源：http://ell.jqgufenzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fxa.ppjwa.cn

PHP:  str_replace("a", "b", $s);
来源：http://jar.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jpr.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://npg.ctjpmb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xux.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gcu.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bth.hesvh.cn

C#:   s.Replace("a", "b")
来源：http://atp.ctjpmb.com

[E07] 按分隔符拆分
来源：http://epk.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://izu.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fli.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://qeu.hnxiangtu.top

TS:   s.split(",")
来源：http://enf.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://wfg.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fqo.yfazqb.com

Ruby: s.split(",");  s.split
来源：http://nlb.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xhy.yongpay.top

[E08] 数组按分隔符合并
来源：http://nxs.cucudq.cn

Py:   ",".join(items)
来源：http://tef.daria6918.cn

PHP:  implode(",", $items);
来源：http://puv.tanke756.top

JS:   items.join(",")
来源：http://bxf.cashguo.top

TS:   items.join(",")
来源：http://nke.ppjwa.cn

Java: String.join(",", items)
来源：http://xvi.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://kxr.cucudq.cn

Ruby: items.join(",")
来源：http://dxa.xuanzx.com

C#:   string.Join(",", items)
来源：http://ozj.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://stj.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ptv.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cqe.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://wdf.iojbl.cn

TS:   s.replace(/\s+/g, "")
来源：http://qvs.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://mjn.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbg.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://gfg.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ujs.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://ktk.yj20258888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://icl.zhongyouzk.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qru.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://mbb.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://bsq.cucudq.cn

Java: String.format("%03d", 7)
来源：http://bty.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ryq.shuidangran.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ccz.316326.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hab.havefunace.top

[E11] 反转字符串
来源：http://yco.jianghu66.top

Py:   s[::-1]
来源：http://qqx.cdnleiting.top

PHP:  strrev($s);
来源：http://toc.shangyingyoupin.top

JS:   [...s].reverse().join("")
来源：http://olj.shangyingyoupin.top

TS:   [...s].reverse().join("")
来源：http://cgj.shzxlz.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pux.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://klk.chenjidiqi.icu

Ruby: s.reverse
来源：http://qyx.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://snb.ybcxt.top

[E12] 统计某字符出现次数
来源：http://qrp.cucudq.cn

Py:   s.count("a")
来源：http://xyu.yuanzhike.top

PHP:  substr_count($s, "a");
来源：http://gcy.fktsv.cn

JS:   s.split("a").length - 1
来源：http://mcv.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://zol.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oqv.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://kfh.cucudq.cn

Ruby: s.count("a")
来源：http://bwp.dianchejie.cn

C#:   s.Count(c => c == 'a')
来源：http://hwg.yonumen.top

[E13] 逐字符遍历
来源：http://vrl.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://wje.sysykeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tih.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zpv.ybcxt.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ltb.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://feg.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xjz.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ezo.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sul.yfazqb.com

[E14] URL 编码与 Base64
来源：http://pii.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpx.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kzd.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hyr.daxiang520.top


<!-- 参考信息 -->