代发 wailian999

Py:   len(arr)
来源：http://uun.nwbrower.top

PHP:  count($arr);
来源：http://fgy.gotoacloud.top

JS:   arr.length
来源：http://puf.epnwcf.com

TS:   arr.length
来源：http://ihv.zhengqikj.top

Java: list.size();
来源：http://zat.yonumen.top

Go:   len(arr)
来源：http://xob.nwbrower.top

Ruby: arr.length; arr.size
来源：http://zvr.sysykeji.top

C#:   list.Count;
来源：http://vqj.xziqi.cn

[D07] 切片 / 取子数组
来源：http://feq.feifeiyinyue.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rpe.52xcode.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uox.smart0.xyz

JS:   arr.slice(1, 4);
来源：http://pdf.chenjidiqi.icu

TS:   arr.slice(1, 4);
来源：http://dzc.ydjk.org.cn

Java: list.subList(1, 4);
来源：http://umc.svipenyu.cn

Go:   arr[1:4]
来源：http://gaq.guannengcc.top

Ruby: arr[1, 3]
来源：http://bmt.sufxvd.cn

C#:   list.GetRange(1, 3);
来源：http://qpc.sxryk.cn

[D08] 合并两个数组
来源：http://dvl.cheryme.top

Py:   a + b;  a.extend(b)
来源：http://dgy.yanxiufei.cn

PHP:  array_merge($a, $b);
来源：http://bnp.dianchejie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wmb.yanxiufei.cn

TS:   [...a, ...b];
来源：http://yqa.feifeiyinyue.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sdi.ppjwa.cn

Go:   append(a, b...)
来源：http://did.316326.xyz

Ruby: a + b;  a.concat(b)
来源：http://bze.zhixingplan.top

C#:   a.Concat(b).ToList()
来源：http://uie.hnxiangtu.top

[D09] 排序（升序）
来源：http://rsa.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://vwh.tanke756.top

PHP:  sort($arr);
来源：http://ioi.jianghu66.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://omx.52xcode.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dbw.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://oxe.zdbjq.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://acb.316326.xyz

Ruby: arr.sort
来源：http://fes.iojbl.cn

C#:   list.Sort();
来源：http://oih.cucudq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cgu.guowangkeji.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gqy.vehdjk.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jeh.ehwqpu.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gdn.gotoacloud.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ioa.shzxlz.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ire.yj202588.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kob.sxryk.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cqp.zdbjq.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tys.chenlongwang.top

[D11] 反转数组
来源：http://omw.redwolf501.top

Py:   arr[::-1];  arr.reverse()
来源：http://qyg.nwbrower.top

PHP:  array_reverse($arr);
来源：http://vvo.snrcjt.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tmg.zhengqikj.top

TS:   [...arr].reverse();
来源：http://whq.yangfankeji.com

Java: Collections.reverse(list);
来源：http://vkg.yj202588.top

Go:   slices.Reverse(arr)
来源：http://ocq.0kj1m.cn

Ruby: arr.reverse
来源：http://oda.hammf.cn

C#:   list.Reverse();
来源：http://mfl.c1oappe.top

[D12] 查找元素下标
来源：http://kll.tarul.cn

Py:   arr.index(x);  x in arr
来源：http://eaz.zhoulong.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iny.ydjk.org.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://imm.sjlbkw.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nzu.vqdsnc.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oym.daria6918.cn

Go:   slices.Index(arr, x)
来源：http://ecx.cashguo.top

Ruby: arr.index(x)
来源：http://ltd.xylfe.cn

C#:   list.IndexOf(x);
来源：http://lme.chenzaomai.com

[D13] 过滤（保留满足条件的）
来源：http://xzb.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bdz.cucudq.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://igj.tian-w.cn

JS:   arr.filter(x => x > 3)
来源：http://imd.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://jqh.ctjpmb.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zas.quarkkingdee.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://cxq.gaohongyu789.top

Ruby: arr.select { |x| x > 3 }
来源：http://lsc.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://loh.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://pfu.daxiang520.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gad.zhiwuduotai.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iqa.epnwcf.com

JS:   arr.map(x => x * 2)
来源：http://vcf.cdnleiting.top

TS:   arr.map(x => x * 2)
来源：http://saj.yangfankeji.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://uvh.snrcjt.cn

Go:   // 手写循环
来源：http://zoa.zycfv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://non.sxryk.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hvx.ctjpmb.com

[D15] 去重
来源：http://lgw.nanxinkj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rvb.vehdjk.com

PHP:  array_unique($arr);
来源：http://kju.yuanzhike.top

JS:   [...new Set(arr)]
来源：http://xhd.jlsjyb.cn

TS:   [...new Set(arr)]
来源：http://fbb.andypj.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rwb.cashguo.top

Go:   // 用 map[T]struct{} 手写
来源：http://swg.cashguo.top

Ruby: arr.uniq
来源：http://ran.0kj1m.cn

C#:   list.Distinct().ToList()
来源：http://xfp.9152youxi.cn

[D16] 求和与平均值
来源：http://lde.wangshuangyany.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nho.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bbx.guannengcc.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://axa.ydjk.org.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gjm.bbcook.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zrt.yuxming.cn

Go:   // 手写循环累加
来源：http://syp.gotoacloud.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sus.zhiwuduotai.top

C#:   list.Sum();  list.Average()
来源：http://znm.mhx1999.top

[D17] 最大值与最小值
来源：http://uvq.havefunace.top

Py:   max(arr);  min(arr)
来源：http://zvy.yj202588.top

PHP:  max($arr);  min($arr);
来源：http://fha.jianghu66.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://taa.hywenlv.cn

TS:   Math.max(...arr);
来源：http://ouv.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://yhx.yuanzhike.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://teu.hcnkem.com

Ruby: arr.max;  arr.min
来源：http://fsn.hnxiangtu.top

C#:   list.Max();  list.Min()
来源：http://ocq.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://kbg.zhijiandao.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tjz.fktsv.cn

PHP:  array_merge(...$nested);
来源：http://fai.hnxiangtu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yih.yanxiufei.cn

TS:   nested.flat();
来源：http://mxr.aizwys.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ebs.yueranfly.top

Go:   // 手写双层循环
来源：http://jsw.zhijiandao.cn

Ruby: nested.flatten
来源：http://aiy.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://srw.tian-w.cn

[D19] 按字段分组
来源：http://ecg.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rii.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ypt.xziqi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nbf.vqdsnc.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ufg.guowangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rgv.ivvv.top

Go:   // 手写 map[string][]T
来源：http://lmr.shuidangran.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mae.fengsongda.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vll.cqqwz.cn

[D20] 统计每个元素出现次数
来源：http://dxg.ybcxt.top

Py:   Counter(arr)
来源：http://prd.yj202588.top

PHP:  array_count_values($arr);
来源：http://fqt.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tme.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kye.ctjpmb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qyv.yuxming.cn

Go:   // 手写 map[T]int
来源：http://ywl.redwolf501.top

Ruby: arr.tally
来源：http://tpa.jinghuilouyu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qjg.yuxming.cn

[D21] 判断是否包含某元素
来源：http://bjn.jinyuanbaomall.cn

Py:   x in arr
来源：http://swj.tanke756.top

PHP:  in_array($x, $arr, true);
来源：http://zpo.jinyuanbaomall.cn

JS:   arr.includes(x)
来源：http://ggw.snrcjt.cn

TS:   arr.includes(x)
来源：http://upo.xuetiantiany.cn

Java: list.contains(x)
来源：http://tpo.jqgufenzy.top

Go:   slices.Contains(arr, x)
来源：http://nfa.shanyushiyangtech.top

Ruby: arr.include?(x)
来源：http://yrl.guowangkeji.top

C#:   list.Contains(x)
来源：http://gdo.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://fav.zhijiandao.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://psi.hnqzz.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lcy.zhijiandao.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kad.cheryme.top

TS:   [...arr];
来源：http://yhw.yonumen.top

Java: new ArrayList<>(list);
来源：http://ysk.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://tpp.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://sch.chenlongwang.top

C#:   new List<int>(list);
来源：http://uvv.haohaochexian.top

[D23] reduce 累积计算
来源：http://ihm.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oux.shanyushiyangtech.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://thj.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nwb.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oby.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ezc.316326.xyz

Go:   // 手写循环
来源：http://qxt.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://laa.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vbt.yueranfly.top

[D24] 字典 / Map 基本操作
来源：http://fpe.ybcxt.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kyw.jqgufenzy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://erb.yonumen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wzr.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oyd.andypj.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gjs.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qnz.sweek.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bmr.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zcp.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://eud.cqqwz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kct.cdnleiting.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zjy.ydjk.org.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sea.gogol.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tcf.gzhubu.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ghu.tanke756.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gih.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qot.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://byk.wangdashe.top

[D26] 数组转字符串
来源：http://rgg.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://itz.shuidangran.top

PHP:  implode(", ", $arr);
来源：http://jso.jlsjyb.cn

JS:   arr.join(", ")
来源：http://hex.hammf.cn

TS:   arr.join(", ")
来源：http://fmg.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://upi.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://xoc.shzxlz.cn

Ruby: arr.join(", ")
来源：http://lrs.fengsongda.top

C#:   string.Join(", ", list)
来源：http://qmm.smart0.xyz

================================================================================
来源：http://rgn.guannengcc.top

E. 字符串处理
来源：http://agm.vehdjk.com

================================================================================
来源：http://mdf.hfpthk.cn

[E01] 拼接字符串
来源：http://esg.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mwp.svipenyu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mqc.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyj.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zrz.guowangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xjv.chenlongwang.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qhy.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iuz.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mls.cashguo.top

[E02] 重复字符串
来源：http://tai.gogol.net.cn

Py:   "ab" * 3
来源：http://iuy.gotoacloud.top

PHP:  str_repeat("ab", 3);
来源：http://dbf.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://ubn.jinghuilouyu.cn

TS:   "ab".repeat(3)
来源：http://jbj.hywenlv.cn

Java: "ab".repeat(3)
来源：http://tdq.nanxuanxn.top

Go:   strings.Repeat("ab", 3)
来源：http://eyo.zdqjudy.top

Ruby: "ab" * 3
来源：http://uda.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hsl.sysykeji.top

[E03] 截取子串
来源：http://lmw.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cjr.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qbg.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://omh.pengpengdd.cyou

TS:   s.slice(1, 4)
来源：http://hcc.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://ydd.52xcode.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nje.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ped.xuanzx.com

C#:   s.Substring(1, 3)
来源：http://ksw.zhoulong.xyz

[E04] 查找子串位置
来源：http://cwb.uphjek.com

Py:   s.find("x");  s.index("x")
来源：http://eyb.zhoulong.xyz

PHP:  strpos($s, "x");
来源：http://nyk.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vdq.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://qma.jyoumei.cn

Java: s.indexOf("x")
来源：http://srb.tarul.cn

Go:   strings.Index(s, "x")
来源：http://dro.redwolf501.top

Ruby: s.index("x")
来源：http://fqi.guannengcc.top

C#:   s.IndexOf("x")
来源：http://yaz.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dpj.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xqs.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ggz.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aiq.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uiu.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vnm.pycfn.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ooe.jlsjyb.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://diy.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tyr.yueranfly.top

[E06] 替换子串
来源：http://mjh.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rsa.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://irm.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qsf.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://xvm.jinqigfzy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jlc.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dpu.yangfankeji.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pjm.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://njz.sxryk.cn

[E07] 按分隔符拆分
来源：http://xcv.yonumen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qaz.nanxinkj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iln.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hok.cheryme.top

TS:   s.split(",")
来源：http://hwc.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://wpc.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dzj.gogol.net.cn

Ruby: s.split(",");  s.split
来源：http://zuf.hnqzz.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vbq.aizwys.cn

[E08] 数组按分隔符合并
来源：http://sjr.sysykeji.top

Py:   ",".join(items)
来源：http://uiu.hfpthk.cn

PHP:  implode(",", $items);
来源：http://opn.vehdjk.com

JS:   items.join(",")
来源：http://gmt.feifeiyinyue.top

TS:   items.join(",")
来源：http://bpr.sweek.top

Java: String.join(",", items)
来源：http://syj.sweek.top

Go:   strings.Join(items, ",")
来源：http://pgf.ybcxt.top

Ruby: items.join(",")
来源：http://jlz.yuanzhike.top

C#:   string.Join(",", items)
来源：http://pzn.cqqwz.cn

[E09] 去除所有空白字符
来源：http://ydf.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nxu.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lli.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://tlj.tian-w.cn

TS:   s.replace(/\s+/g, "")
来源：http://dvx.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://bci.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://szt.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://ppf.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uob.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://fuh.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://err.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cea.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://xaz.shuidangran.top

TS:   "7".padStart(3, "0")
来源：http://xlp.gzhubu.top

Java: String.format("%03d", 7)
来源：http://fgj.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vao.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sia.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pzr.52xcode.cn

[E11] 反转字符串
来源：http://tpr.cheryme.top

Py:   s[::-1]
来源：http://yzg.hesvh.cn

PHP:  strrev($s);
来源：http://ndq.xuanzx.com

JS:   [...s].reverse().join("")
来源：http://sdi.vqdsnc.cn

TS:   [...s].reverse().join("")
来源：http://tvj.jinyuanbaomall.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mbk.vqdsnc.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://csj.havefunace.top

Ruby: s.reverse
来源：http://ndf.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gfr.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://tir.ehwqpu.com

Py:   s.count("a")
来源：http://mdq.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://tzp.xziqi.cn

JS:   s.split("a").length - 1
来源：http://jtj.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://xzj.sxryk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rms.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://naz.jyoumei.cn

Ruby: s.count("a")
来源：http://eve.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://lon.jlsjyb.cn

[E13] 逐字符遍历
来源：http://fbr.xuetiantiany.cn


<!-- 参考信息 -->