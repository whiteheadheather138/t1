代发 wailian999

[D07] 切片 / 取子数组
来源：http://gtd.ivvv.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xho.hnqzz.top

PHP:  array_slice($arr, 1, 3);
来源：http://hke.xziqi.cn

JS:   arr.slice(1, 4);
来源：http://wxt.yvedp.cn

TS:   arr.slice(1, 4);
来源：http://xva.tianlin.xyz

Java: list.subList(1, 4);
来源：http://wln.ydjk.org.cn

Go:   arr[1:4]
来源：http://euw.nwbrower.top

Ruby: arr[1, 3]
来源：http://lth.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://eqi.quarkkingdee.top

[D08] 合并两个数组
来源：http://lao.hysaishi.cn

Py:   a + b;  a.extend(b)
来源：http://pkq.feifeiyinyue.top

PHP:  array_merge($a, $b);
来源：http://spe.hysaishi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://frf.shanyushiyangkeji.top

TS:   [...a, ...b];
来源：http://mwy.havefunace.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://bcz.hesvh.cn

Go:   append(a, b...)
来源：http://qke.gotoacloud.top

Ruby: a + b;  a.concat(b)
来源：http://oxz.fehbvm.com

C#:   a.Concat(b).ToList()
来源：http://cot.52xcode.cn

[D09] 排序（升序）
来源：http://afm.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://onk.zhaomingkeji.xyz

PHP:  sort($arr);
来源：http://zoh.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gyk.jinqigufen.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://adg.gotoacloud.top

Java: Collections.sort(list);  list.sort(null);
来源：http://udf.sweek.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cqg.yj20258888.top

Ruby: arr.sort
来源：http://fgi.xylfe.cn

C#:   list.Sort();
来源：http://jms.yangfankeji.com

[D10] 自定义排序（按字段 / 多条件）
来源：http://kxi.zycfv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://jog.yuanzhike.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pwk.tarul.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://miz.daxiang520.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://kcl.pycfn.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lws.xziqi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ybh.sysykeji.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://inl.uphjek.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://nol.yuanzhike.top

[D11] 反转数组
来源：http://ktt.pycfn.com

Py:   arr[::-1];  arr.reverse()
来源：http://niu.ppjwa.cn

PHP:  array_reverse($arr);
来源：http://usx.shangyingyoupin.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rma.fehbvm.com

TS:   [...arr].reverse();
来源：http://tma.gogol.net.cn

Java: Collections.reverse(list);
来源：http://mbx.sjlbkw.cn

Go:   slices.Reverse(arr)
来源：http://qxa.9152youxi.cn

Ruby: arr.reverse
来源：http://qei.iojbl.cn

C#:   list.Reverse();
来源：http://cza.yj20258.top

[D12] 查找元素下标
来源：http://kgp.gaohongyu789.top

Py:   arr.index(x);  x in arr
来源：http://kyg.yuanzhike.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kaw.kuanghao11.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ovb.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mtt.316326.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xhu.fanxiaobao.xyz

Go:   slices.Index(arr, x)
来源：http://hxz.9152youxi.cn

Ruby: arr.index(x)
来源：http://sbg.zhengqikj.top

C#:   list.IndexOf(x);
来源：http://tbc.xuanzx.com

[D13] 过滤（保留满足条件的）
来源：http://rgo.ybcxt.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://exi.jinqigufen.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mry.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://rol.ydzc1.top

TS:   arr.filter(x => x > 3)
来源：http://kaa.sxryk.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lry.pycfn.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fuc.vqdsnc.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gnr.0kj1m.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://opd.ydjk.org.cn

[D14] 映射转换（每个元素变形）
来源：http://ndd.chenzaomai.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://glf.ybcxt.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oom.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://pxx.xinyue.icu

TS:   arr.map(x => x * 2)
来源：http://pkm.snrcjt.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sil.zhaomingkeji.xyz

Go:   // 手写循环
来源：http://fcy.yuanzhike.top

Ruby: arr.map { |x| x * 2 }
来源：http://hfj.shuidangran.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xfo.zhoulong.xyz

[D15] 去重
来源：http://ufy.cheryme.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ouj.ppjwa.cn

PHP:  array_unique($arr);
来源：http://ess.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://ugq.xuanzx.com

TS:   [...new Set(arr)]
来源：http://hpt.shuidangran.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ikv.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://mvc.jinqigfzy.top

Ruby: arr.uniq
来源：http://zjv.feifeiyinyue.top

C#:   list.Distinct().ToList()
来源：http://ihi.iojbl.cn

[D16] 求和与平均值
来源：http://sca.aizwys.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hym.hesvh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ojb.iojbl.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pee.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gmd.kuanghao11.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ymh.cdnleiting.top

Go:   // 手写循环累加
来源：http://att.bbcook.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aai.guannengcc.top

C#:   list.Sum();  list.Average()
来源：http://uib.meibo888.top

[D17] 最大值与最小值
来源：http://zbq.tarul.cn

Py:   max(arr);  min(arr)
来源：http://qle.fktsv.cn

PHP:  max($arr);  min($arr);
来源：http://ohy.hnxiangtu.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://coi.sweek.top

TS:   Math.max(...arr);
来源：http://swh.zdqjudy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qtk.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iat.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://met.pycfn.com

C#:   list.Max();  list.Min()
来源：http://tpb.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://oba.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fht.aizwys.cn

PHP:  array_merge(...$nested);
来源：http://pzk.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kfj.jlsjyb.cn

TS:   nested.flat();
来源：http://gmj.cdnleiting.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://unc.birdmap.top

Go:   // 手写双层循环
来源：http://jqr.jinyuanbaomall.cn

Ruby: nested.flatten
来源：http://jyz.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://keq.gaohongyu789.top

[D19] 按字段分组
来源：http://yum.chenlongwang.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fou.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ixb.yj202588.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qft.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dkl.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oxd.fehbvm.com

Go:   // 手写 map[string][]T
来源：http://pkz.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tcx.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ncn.bjfxy.top

[D20] 统计每个元素出现次数
来源：http://atn.havefunace.top

Py:   Counter(arr)
来源：http://zim.bbcook.cn

PHP:  array_count_values($arr);
来源：http://mzj.mhx1999.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://boo.ctjpmb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gkg.yangfankeji.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://swt.daria6918.cn

Go:   // 手写 map[T]int
来源：http://paa.xziqi.cn

Ruby: arr.tally
来源：http://evl.0kj1m.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dcs.yvedp.cn

[D21] 判断是否包含某元素
来源：http://qyv.xylfe.cn

Py:   x in arr
来源：http://swr.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://ksg.havefunace.top

JS:   arr.includes(x)
来源：http://zos.xylfe.cn

TS:   arr.includes(x)
来源：http://sby.xinyue.icu

Java: list.contains(x)
来源：http://fjr.xziqi.cn

Go:   slices.Contains(arr, x)
来源：http://cbd.cheryme.top

Ruby: arr.include?(x)
来源：http://iwi.hongshengwenyu.top

C#:   list.Contains(x)
来源：http://nkt.ydjk.org.cn

[D22] 复制数组（避免共享引用）
来源：http://zum.hfpthk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ncu.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://srz.jinqigfzy.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mfc.nanxuanxn.top

TS:   [...arr];
来源：http://bqw.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://ltm.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://met.cashguo.top

Ruby: arr.dup;  arr.clone
来源：http://cou.zhongyouzk.top

C#:   new List<int>(list);
来源：http://qsz.zycfv.cn

[D23] reduce 累积计算
来源：http://uzg.nwbrower.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vsf.sufxvd.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bir.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jcw.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vix.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://ozf.yj20258888.top

Go:   // 手写循环
来源：http://qyx.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://com.316326.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://iyx.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://atn.shzxlz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mbi.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cjg.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kxx.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://guj.zdqjudy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://voe.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ict.ppjwa.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://try.c1oappe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yid.yanxiufei.cn

[D25] Set 集合去重与交并差
来源：http://xhb.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tnf.nanxinkj.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wff.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://flt.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cpm.shanyushiyangkeji.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nrt.sysykeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vsf.gotoacloud.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://evt.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ctc.iojbl.cn

[D26] 数组转字符串
来源：http://lwb.zhixingplan.top

Py:   ", ".join(map(str, arr))
来源：http://rhq.jinyuanbaomall.cn

PHP:  implode(", ", $arr);
来源：http://agh.jinghuilouyu.cn

JS:   arr.join(", ")
来源：http://efw.mhx1999.top

TS:   arr.join(", ")
来源：http://itd.fzhhl.top

Java: String.join(", ", list)
来源：http://sai.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://vsp.zhixingplan.top

Ruby: arr.join(", ")
来源：http://rty.iojbl.cn

C#:   string.Join(", ", list)
来源：http://utq.ppjwa.cn

================================================================================
来源：http://rrk.zhaomingkeji.xyz

E. 字符串处理
来源：http://spm.ybcxt.top

================================================================================
来源：http://gyw.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://bur.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yqa.9152youxi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://akk.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gif.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://keu.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vwm.jqgfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nvm.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eqj.guannengcc.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fnf.9152youxi.cn

[E02] 重复字符串
来源：http://dfy.zhengqikj.top

Py:   "ab" * 3
来源：http://cdl.fehbvm.com

PHP:  str_repeat("ab", 3);
来源：http://kwj.hesvh.cn

JS:   "ab".repeat(3)
来源：http://dmy.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://och.aibaodan.cn

Java: "ab".repeat(3)
来源：http://phl.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://rzy.sweek.top

Ruby: "ab" * 3
来源：http://onh.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://iur.zhongyouzk.top

[E03] 截取子串
来源：http://rat.aibaodan.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sdj.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://llk.zhaomingkeji.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tqf.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://lrr.tian-w.cn

Java: s.substring(1, 4)
来源：http://dew.xylfe.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hqt.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://ruc.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://oxr.fehbvm.com

[E04] 查找子串位置
来源：http://gfl.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://dgu.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://knh.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csx.yongpay.top

TS:   s.indexOf("x")
来源：http://wtc.bjfxy.top

Java: s.indexOf("x")
来源：http://iti.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://ncc.gogol.net.cn

Ruby: s.index("x")
来源：http://njp.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://scj.sjlbkw.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cka.mhx1999.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yft.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eds.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fls.sxryk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kdg.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://igf.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vsp.haohaochexian.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rxz.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ams.yangfankeji.com

[E06] 替换子串
来源：http://rgh.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qba.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://acy.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jsx.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://smv.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://myx.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sng.hfpthk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zex.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://lid.zhengqikj.top

[E07] 按分隔符拆分
来源：http://xyt.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dpj.yueranfly.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tze.shanyushiyangtech.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ddt.zhongyouzk.top

TS:   s.split(",")
来源：http://lep.cdnleiting.top

Java: s.split(",");  s.split("\\s+")
来源：http://frt.nanxuanxn.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lcx.316326.xyz

Ruby: s.split(",");  s.split
来源：http://ldf.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gbn.zdbjq.cn

[E08] 数组按分隔符合并
来源：http://svz.yuxming.cn

Py:   ",".join(items)
来源：http://npo.tianlin.xyz

PHP:  implode(",", $items);
来源：http://xuz.zycfv.cn

JS:   items.join(",")
来源：http://hzg.daria6918.cn

TS:   items.join(",")
来源：http://nnj.yuxming.cn

Java: String.join(",", items)
来源：http://bku.hysaishi.cn

Go:   strings.Join(items, ",")
来源：http://mcm.andypj.xyz

Ruby: items.join(",")
来源：http://ped.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://bpz.hcnkem.com

[E09] 去除所有空白字符
来源：http://mfc.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xih.0kj1m.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://req.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://ecf.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://dqn.ydjk.org.cn

Java: s.replaceAll("\\s+", "")
来源：http://gjp.ydjk.org.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gfk.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://pxt.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://inv.uphjek.com

[E10] 左侧补零 / 定长填充
来源：http://hym.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kee.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wue.yuxming.cn

JS:   "7".padStart(3, "0")
来源：http://pgu.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://wwo.fzhhl.top

Java: String.format("%03d", 7)
来源：http://pps.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qbl.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gid.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ewp.hammf.cn

[E11] 反转字符串
来源：http://vmu.yueranfly.top

Py:   s[::-1]
来源：http://gwz.nwbrower.top

PHP:  strrev($s);
来源：http://zym.ehwqpu.com

JS:   [...s].reverse().join("")
来源：http://wxz.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://udt.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xek.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kka.jinghuilouyu.cn

Ruby: s.reverse
来源：http://vcj.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iya.yj20258.top

[E12] 统计某字符出现次数
来源：http://cim.xylfe.cn

Py:   s.count("a")
来源：http://jyb.xingfuxueyuan.xyz

PHP:  substr_count($s, "a");
来源：http://rte.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://cjf.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://uff.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgn.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://hlb.vqdsnc.cn

Ruby: s.count("a")
来源：http://qtm.yuxming.cn

C#:   s.Count(c => c == 'a')
来源：http://qbl.xylfe.cn

[E13] 逐字符遍历
来源：http://pgi.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://jvh.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dij.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rdc.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jwr.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://orm.fehbvm.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bym.yvedp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rwv.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tvk.uphjek.com


<!-- 参考信息 -->