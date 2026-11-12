代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ywt.birdmap.top

Ruby: arr.sort
来源：http://imu.hywenlv.cn

C#:   list.Sort();
来源：http://edk.guowangkeji.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://txt.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sfz.cashguo.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aly.gaohongyu789.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bmn.zhengqikj.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://htn.gotoacloud.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qnz.zhijiandao.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wdy.zhaomingkeji.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://urb.fktsv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qnr.ppjwa.cn

[D11] 反转数组
来源：http://amp.9152youxi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://brf.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://hlt.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://lvc.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://ban.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://ohu.wangshuangyany.cn

Go:   slices.Reverse(arr)
来源：http://ixe.yongpay.top

Ruby: arr.reverse
来源：http://lvo.jqgfzy.top

C#:   list.Reverse();
来源：http://iun.jinqigfzy.top

[D12] 查找元素下标
来源：http://rrb.yuanzhike.top

Py:   arr.index(x);  x in arr
来源：http://nwo.shanyushiyangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rlb.bbcook.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nqb.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xzr.ydzc1.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lyr.jqgufenzy.top

Go:   slices.Index(arr, x)
来源：http://dii.aibaodan.cn

Ruby: arr.index(x)
来源：http://ren.zhiwuduotai.top

C#:   list.IndexOf(x);
来源：http://ggz.zhoulong.xyz

[D13] 过滤（保留满足条件的）
来源：http://mqm.nanxuanxn.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://euh.pycfn.com

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ysd.fktsv.cn

JS:   arr.filter(x => x > 3)
来源：http://hxn.cucudq.cn

TS:   arr.filter(x => x > 3)
来源：http://blc.vehdjk.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rod.redwolf501.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ocd.xylfe.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nad.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lbk.shanyushiyangtech.top

[D14] 映射转换（每个元素变形）
来源：http://lxr.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ovb.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bzl.hnxiangtu.top

JS:   arr.map(x => x * 2)
来源：http://wtu.yfazqb.com

TS:   arr.map(x => x * 2)
来源：http://fvj.zhijiandao.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kdz.bjfxy.top

Go:   // 手写循环
来源：http://ott.sxryk.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tgy.9152youxi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qfh.shzxlz.cn

[D15] 去重
来源：http://awm.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ewa.hesvh.cn

PHP:  array_unique($arr);
来源：http://nmt.gzhubu.top

JS:   [...new Set(arr)]
来源：http://vzd.hnxiangtu.top

TS:   [...new Set(arr)]
来源：http://ktn.pycfn.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oak.chenjidiqi.icu

Go:   // 用 map[T]struct{} 手写
来源：http://myn.chenjidiqi.icu

Ruby: arr.uniq
来源：http://fvu.52xcode.cn

C#:   list.Distinct().ToList()
来源：http://oll.chenzaomai.com

[D16] 求和与平均值
来源：http://iuz.cashguo.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jmv.shuidangran.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://inc.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://asm.zhijiandao.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ssv.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pjy.jyoumei.cn

Go:   // 手写循环累加
来源：http://rqm.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uhu.zycfv.cn

C#:   list.Sum();  list.Average()
来源：http://ega.yangfankeji.com

[D17] 最大值与最小值
来源：http://bgq.tian-w.cn

Py:   max(arr);  min(arr)
来源：http://rzb.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://tem.0kj1m.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ntc.mhx1999.top

TS:   Math.max(...arr);
来源：http://xib.pengpengdd.cyou

Java: Collections.max(list);  Collections.min(list);
来源：http://mca.jqgufenzy.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rvg.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://udj.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://dyq.hcnkem.com

[D18] 扁平化嵌套数组
来源：http://qxh.sjlbkw.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzr.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://gtl.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ifi.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://eqs.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tns.yongpay.top

Go:   // 手写双层循环
来源：http://rkb.52xcode.cn

Ruby: nested.flatten
来源：http://rkp.cashguo.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hrr.tianlin.xyz

[D19] 按字段分组
来源：http://nyk.cucudq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ixz.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hky.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mhs.mhx1999.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tmq.wangshuangyany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iua.sxryk.cn

Go:   // 手写 map[string][]T
来源：http://hpk.vehdjk.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://fob.jinyuanbaomall.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wsf.hywenlv.cn

[D20] 统计每个元素出现次数
来源：http://dvp.cheryme.top

Py:   Counter(arr)
来源：http://aft.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://hdf.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mms.snrcjt.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fel.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pdi.ydzc1.top

Go:   // 手写 map[T]int
来源：http://sce.hywenlv.cn

Ruby: arr.tally
来源：http://xcw.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qpd.tarul.cn

[D21] 判断是否包含某元素
来源：http://vah.c1oappe.top

Py:   x in arr
来源：http://upw.ctjpmb.com

PHP:  in_array($x, $arr, true);
来源：http://lkn.chenjidiqi.icu

JS:   arr.includes(x)
来源：http://guw.nanxuanxn.top

TS:   arr.includes(x)
来源：http://hpq.xuanzx.com

Java: list.contains(x)
来源：http://zmj.cqqwz.cn

Go:   slices.Contains(arr, x)
来源：http://pxc.fengsongda.top

Ruby: arr.include?(x)
来源：http://wip.gogol.net.cn

C#:   list.Contains(x)
来源：http://esk.sysykeji.top

[D22] 复制数组（避免共享引用）
来源：http://cbh.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ddl.hesvh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ypz.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mpi.zhixingplan.top

TS:   [...arr];
来源：http://yyv.guannengcc.top

Java: new ArrayList<>(list);
来源：http://vlx.sxryk.cn

Go:   copied := append([]int(nil), arr...)
来源：http://don.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://xqu.tarul.cn

C#:   new List<int>(list);
来源：http://tim.yonumen.top

[D23] reduce 累积计算
来源：http://xsj.guannengcc.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gec.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ymv.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yup.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jds.vqdsnc.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gjk.jyoumei.cn

Go:   // 手写循环
来源：http://yci.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lnr.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blj.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://waj.yuxming.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oev.haohaochexian.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xeh.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ahq.daria6918.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lnh.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fkt.fanxiaobao.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mzn.sysykeji.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tmj.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qpa.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://fhf.hongshengwenyu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://net.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ibo.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ckz.fengsongda.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://twj.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ocl.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vgd.ydjk.org.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ccj.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tub.zhixingplan.top

[D26] 数组转字符串
来源：http://mcr.fengsongda.top

Py:   ", ".join(map(str, arr))
来源：http://lwu.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://jwa.nanxuanxn.top

JS:   arr.join(", ")
来源：http://fho.nanxinkj.top

TS:   arr.join(", ")
来源：http://hiw.c1oappe.top

Java: String.join(", ", list)
来源：http://jkg.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://jgo.redwolf501.top

Ruby: arr.join(", ")
来源：http://bab.yvedp.cn

C#:   string.Join(", ", list)
来源：http://hyu.yuanzhike.top

================================================================================
来源：http://qhi.fehbvm.com

E. 字符串处理
来源：http://hej.hywenlv.cn

================================================================================
来源：http://kls.aizwys.cn

[E01] 拼接字符串
来源：http://mzn.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zlb.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jwt.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://aua.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dcp.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mlf.fzhhl.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pwj.yongpay.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lfm.jinqigufen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://guu.tarul.cn

[E02] 重复字符串
来源：http://vod.zhijiandao.cn

Py:   "ab" * 3
来源：http://ddi.sjlbkw.cn

PHP:  str_repeat("ab", 3);
来源：http://ryt.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://uzx.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://hen.nanxuanxn.top

Java: "ab".repeat(3)
来源：http://unq.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://epv.sxryk.cn

Ruby: "ab" * 3
来源：http://wum.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dew.fanxiaobao.xyz

[E03] 截取子串
来源：http://aji.zdbjq.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qir.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ehp.gzhubu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vno.epnwcf.com

TS:   s.slice(1, 4)
来源：http://fzu.shanyushiyangkeji.top

Java: s.substring(1, 4)
来源：http://bml.epnwcf.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rhw.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://hsv.yvedp.cn

C#:   s.Substring(1, 3)
来源：http://ffg.cdnleiting.top

[E04] 查找子串位置
来源：http://xso.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://bfy.nwbrower.top

PHP:  strpos($s, "x");
来源：http://jdi.mhx1999.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uud.zhaomingkeji.xyz

TS:   s.indexOf("x")
来源：http://wrc.sweek.top

Java: s.indexOf("x")
来源：http://ssg.guannengcc.top

Go:   strings.Index(s, "x")
来源：http://gnq.nanxinkj.top

Ruby: s.index("x")
来源：http://uku.tanke756.top

C#:   s.IndexOf("x")
来源：http://lif.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkl.aibaodan.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wsu.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://arj.zhaomingkeji.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vhe.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lte.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://doh.hongshengwenyu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://btg.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qsu.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://num.xinyue.icu

[E06] 替换子串
来源：http://sgp.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://foh.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://kig.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mqw.jiagoushi.top

TS:   s.replaceAll("a", "b")
来源：http://lex.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hue.hnqzz.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bqz.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mrs.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://bwg.yanxiufei.cn

[E07] 按分隔符拆分
来源：http://pxh.sysykeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yqh.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wqu.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hcz.vehdjk.com

TS:   s.split(",")
来源：http://btd.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://jvr.iojbl.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://muj.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://mdv.jlsjyb.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fml.tarul.cn

[E08] 数组按分隔符合并
来源：http://cnu.ydzc1.top

Py:   ",".join(items)
来源：http://jlx.jqgfzy.top

PHP:  implode(",", $items);
来源：http://rnk.yfazqb.com

JS:   items.join(",")
来源：http://mgh.yonumen.top

TS:   items.join(",")
来源：http://lat.ctjpmb.com

Java: String.join(",", items)
来源：http://xhj.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://yli.xinyue.icu

Ruby: items.join(",")
来源：http://mwy.zdbjq.cn

C#:   string.Join(",", items)
来源：http://ygt.daxiang520.top

[E09] 去除所有空白字符
来源：http://tay.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vza.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://obw.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://jzu.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ouy.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://ame.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ypc.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://rpq.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bud.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://cxu.sweek.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kas.yj20258888.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cht.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://hdd.gogol.net.cn

TS:   "7".padStart(3, "0")
来源：http://ywk.fehbvm.com

Java: String.format("%03d", 7)
来源：http://yfi.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ijf.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cgy.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://liy.guannengcc.top

[E11] 反转字符串
来源：http://bqm.chenjidiqi.icu

Py:   s[::-1]
来源：http://xuu.sweek.top

PHP:  strrev($s);
来源：http://ukb.zdqjudy.top

JS:   [...s].reverse().join("")
来源：http://rtz.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://lmu.pycfn.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ouw.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jxi.xinyue.icu

Ruby: s.reverse
来源：http://zzc.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://hvu.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://pus.jinqigfzy.top

Py:   s.count("a")
来源：http://ian.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://edb.jianghu66.top

JS:   s.split("a").length - 1
来源：http://rcy.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://bxp.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://azk.tian-w.cn

Go:   strings.Count(s, "a")
来源：http://pqu.zhijiandao.cn

Ruby: s.count("a")
来源：http://bbi.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://rsz.vehdjk.com

[E13] 逐字符遍历
来源：http://fxh.xziqi.cn

Py:   for ch in s: print(ch)
来源：http://pnj.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qdw.wangshuangyany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zwk.guannengcc.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wtk.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gye.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ykd.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://aaw.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ngb.316326.xyz

[E14] URL 编码与 Base64
来源：http://eqs.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hqd.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hww.vqdsnc.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oyj.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uby.jinghuilouyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qyv.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uwf.gogol.net.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ogm.daria6918.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ubi.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://xkc.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://aen.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rmn.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kpm.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ypr.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ypb.yj20258888.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pll.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://akv.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kgs.uphjek.com

[E16] 数字千分位
来源：http://naz.cashguo.top

Py:   f"{1234567:,}"
来源：http://aje.guannengcc.top

PHP:  number_format(1234567);
来源：http://vwy.0kj1m.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oev.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vrd.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hkg.yueranfly.top


<!-- 参考信息 -->