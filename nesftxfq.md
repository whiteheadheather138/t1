代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://pnt.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://tlj.tarul.cn

[D09] 排序（升序）
来源：http://fys.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://fam.ehwqpu.com

PHP:  sort($arr);
来源：http://xuh.svipenyu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mty.wangshuangyany.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ngy.wangshuangyany.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://mxs.shanyushiyangkeji.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rye.c1oappe.top

Ruby: arr.sort
来源：http://xpw.yanxiufei.cn

C#:   list.Sort();
来源：http://xpx.52xcode.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lsh.52xcode.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mmb.zhixingplan.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gbt.yj202588.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dym.aibaodan.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://cpg.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dho.jqgufenzy.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hsf.jianghu66.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dht.hywenlv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rnq.zdqjudy.top

[D11] 反转数组
来源：http://pwk.zhixingplan.top

Py:   arr[::-1];  arr.reverse()
来源：http://daq.pengpengdd.cyou

PHP:  array_reverse($arr);
来源：http://baq.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pup.dashuyun.cn

TS:   [...arr].reverse();
来源：http://oim.ydzc1.top

Java: Collections.reverse(list);
来源：http://tkq.yanxiufei.cn

Go:   slices.Reverse(arr)
来源：http://tuz.jinghuilouyu.cn

Ruby: arr.reverse
来源：http://ioc.9152youxi.cn

C#:   list.Reverse();
来源：http://itx.yangfankeji.com

[D12] 查找元素下标
来源：http://coe.sjlbkw.cn

Py:   arr.index(x);  x in arr
来源：http://syl.redwolf501.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gsc.cheryme.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://naf.fanxiaobao.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpb.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wcv.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://shf.hysaishi.cn

Ruby: arr.index(x)
来源：http://dep.hfpthk.cn

C#:   list.IndexOf(x);
来源：http://dfj.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://ngs.tianlin.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bzc.yanxiufei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ojr.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://ixa.daxiang520.top

TS:   arr.filter(x => x > 3)
来源：http://kxl.yangfankeji.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zzy.shanyushiyangtech.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xeb.uphjek.com

Ruby: arr.select { |x| x > 3 }
来源：http://mdq.vqdsnc.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://iij.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://nek.guowangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wxb.nwbrower.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vya.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://ghb.yvedp.cn

TS:   arr.map(x => x * 2)
来源：http://otm.hongshengwenyu.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://dje.jinqigufen.top

Go:   // 手写循环
来源：http://neo.jinqigufen.top

Ruby: arr.map { |x| x * 2 }
来源：http://gqa.bbcook.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://gjr.shanyushiyangtech.top

[D15] 去重
来源：http://mnb.yuxming.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tct.aibaodan.cn

PHP:  array_unique($arr);
来源：http://dom.iojbl.cn

JS:   [...new Set(arr)]
来源：http://tda.hnqzz.top

TS:   [...new Set(arr)]
来源：http://ldp.xinyue.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://irv.xuanzx.com

Go:   // 用 map[T]struct{} 手写
来源：http://hpe.sufxvd.cn

Ruby: arr.uniq
来源：http://uuo.zhiwuduotai.top

C#:   list.Distinct().ToList()
来源：http://mvy.tarul.cn

[D16] 求和与平均值
来源：http://yjt.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://apa.shanyushiyangtech.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rfj.shangyingyoupin.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://axk.meibo888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lic.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cgf.ywan-chungtsiang.top

Go:   // 手写循环累加
来源：http://cpn.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kxa.zhoulong.xyz

C#:   list.Sum();  list.Average()
来源：http://dym.hesvh.cn

[D17] 最大值与最小值
来源：http://sav.yj202588.top

Py:   max(arr);  min(arr)
来源：http://xxk.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://jso.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://imp.aibaodan.cn

TS:   Math.max(...arr);
来源：http://dhf.tianlin.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://sey.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xzc.birdmap.top

Ruby: arr.max;  arr.min
来源：http://jlv.yanxiufei.cn

C#:   list.Max();  list.Min()
来源：http://nuk.zhengqikj.top

[D18] 扁平化嵌套数组
来源：http://ckm.jlsjyb.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zmw.yueranfly.top

PHP:  array_merge(...$nested);
来源：http://mgn.epnwcf.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sqx.cheryme.top

TS:   nested.flat();
来源：http://bje.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nqj.birdmap.top

Go:   // 手写双层循环
来源：http://epz.hongshengwenyu.top

Ruby: nested.flatten
来源：http://chw.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://vij.hammf.cn

[D19] 按字段分组
来源：http://vrc.zhongyouzk.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fdo.cucudq.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://awf.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://krv.tarul.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://met.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dea.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://wik.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://eyt.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://evf.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://bpk.svipenyu.cn

Py:   Counter(arr)
来源：http://kat.0kj1m.cn

PHP:  array_count_values($arr);
来源：http://dlm.fehbvm.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cqk.hesvh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xwv.0kj1m.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ivp.zdqjudy.top

Go:   // 手写 map[T]int
来源：http://vgv.jqgfzy.top

Ruby: arr.tally
来源：http://kck.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cjf.svipenyu.cn

[D21] 判断是否包含某元素
来源：http://ldq.yangfankeji.com

Py:   x in arr
来源：http://afb.chenjidiqi.icu

PHP:  in_array($x, $arr, true);
来源：http://kcl.jqgfzy.top

JS:   arr.includes(x)
来源：http://box.wangshuangyany.cn

TS:   arr.includes(x)
来源：http://dcn.kuanghao11.cn

Java: list.contains(x)
来源：http://hbd.fktsv.cn

Go:   slices.Contains(arr, x)
来源：http://ohj.yj202588.top

Ruby: arr.include?(x)
来源：http://adh.c1oappe.top

C#:   list.Contains(x)
来源：http://tri.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://uhp.shanyushiyangkeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mcm.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tcz.shzxlz.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jal.yuxming.cn

TS:   [...arr];
来源：http://cqw.bbcook.cn

Java: new ArrayList<>(list);
来源：http://kfm.shuidangran.top

Go:   copied := append([]int(nil), arr...)
来源：http://msv.cdnleiting.top

Ruby: arr.dup;  arr.clone
来源：http://bnm.yonumen.top

C#:   new List<int>(list);
来源：http://fro.cqqwz.cn

[D23] reduce 累积计算
来源：http://zsc.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qqh.fzhhl.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mse.jqgfzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uga.guowangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bxo.fehbvm.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://jup.sysykeji.top

Go:   // 手写循环
来源：http://yda.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kpq.hnxiangtu.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://chf.cucudq.cn

[D24] 字典 / Map 基本操作
来源：http://cxm.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://spk.9152youxi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vtz.redwolf501.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lno.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://abj.yj202588.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://afo.birdmap.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hmp.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ffi.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bpa.wangshuangyany.cn

[D25] Set 集合去重与交并差
来源：http://qcj.aizwys.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fsf.xuetiantiany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hfa.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hye.svipenyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://klc.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://swt.xuetiantiany.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nri.xingfuxueyuan.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vso.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cbd.cucudq.cn

[D26] 数组转字符串
来源：http://uzj.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://kee.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://wyp.nanxinkj.top

JS:   arr.join(", ")
来源：http://aik.cashguo.top

TS:   arr.join(", ")
来源：http://luw.yuxming.cn

Java: String.join(", ", list)
来源：http://mze.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://kef.xuanzx.com

Ruby: arr.join(", ")
来源：http://tau.xinyue.icu

C#:   string.Join(", ", list)
来源：http://hqs.jianghu66.top

================================================================================
来源：http://xdt.ybcxt.top

E. 字符串处理
来源：http://jvk.c1oappe.top

================================================================================
来源：http://fan.tarul.cn

[E01] 拼接字符串
来源：http://tfb.sjlbkw.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yyv.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wsr.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ynv.jqgufenzy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyn.gzhubu.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ckc.yj20258888.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gbz.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lfj.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fsi.gogol.net.cn

[E02] 重复字符串
来源：http://otl.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://rco.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://ftn.dashuyun.cn

JS:   "ab".repeat(3)
来源：http://dqu.ppjwa.cn

TS:   "ab".repeat(3)
来源：http://bed.birdmap.top

Java: "ab".repeat(3)
来源：http://wfg.jqgufenzy.top

Go:   strings.Repeat("ab", 3)
来源：http://wlg.nanxinkj.top

Ruby: "ab" * 3
来源：http://kar.jlsjyb.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fju.jinghuilouyu.cn

[E03] 截取子串
来源：http://epr.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xcj.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwq.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://knj.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://dfx.jiagoushi.top

Java: s.substring(1, 4)
来源：http://mse.guowangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qvm.guannengcc.top

Ruby: s[1, 3];  s[1..3]
来源：http://ltd.pycfn.com

C#:   s.Substring(1, 3)
来源：http://all.dianchejie.cn

[E04] 查找子串位置
来源：http://ceh.zycfv.cn

Py:   s.find("x");  s.index("x")
来源：http://rcf.shuidangran.top

PHP:  strpos($s, "x");
来源：http://pkm.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://etp.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://coh.zhijiandao.cn

Java: s.indexOf("x")
来源：http://xme.haohaochexian.top

Go:   strings.Index(s, "x")
来源：http://gwn.iojbl.cn

Ruby: s.index("x")
来源：http://qtw.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://jrn.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nyf.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vzg.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://awx.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dus.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cza.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tye.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zbn.zhoulong.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ayd.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zbt.shangyingyoupin.top

[E06] 替换子串
来源：http://oqq.epnwcf.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://opv.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://xkz.yueranfly.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lti.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://siw.vqdsnc.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ysc.52xcode.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mcp.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rtd.hammf.cn

C#:   s.Replace("a", "b")
来源：http://hnh.jyoumei.cn

[E07] 按分隔符拆分
来源：http://pmr.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nin.vqdsnc.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fib.fehbvm.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://zfk.bbcook.cn

TS:   s.split(",")
来源：http://rkz.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://svy.yuxming.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fea.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://sec.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ysn.shuidangran.top

[E08] 数组按分隔符合并
来源：http://uoc.daxiang520.top

Py:   ",".join(items)
来源：http://amk.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://cxf.cashguo.top

JS:   items.join(",")
来源：http://ugv.yj202588.top

TS:   items.join(",")
来源：http://fgj.cdnleiting.top

Java: String.join(",", items)
来源：http://num.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://ldr.aibaodan.cn

Ruby: items.join(",")
来源：http://ugl.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://xsn.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://ywd.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dlv.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fbm.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://jfv.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://okx.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://skt.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pzz.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://kxa.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fis.jiagoushi.top

[E10] 左侧补零 / 定长填充
来源：http://enm.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wec.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pow.sxryk.cn

JS:   "7".padStart(3, "0")
来源：http://xqy.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://jvn.epnwcf.com

Java: String.format("%03d", 7)
来源：http://brv.yuanzhike.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uaz.zhongyouzk.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qdm.mhx1999.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wcb.fengsongda.top

[E11] 反转字符串
来源：http://jsw.52xcode.cn

Py:   s[::-1]
来源：http://dnd.jianghu66.top

PHP:  strrev($s);
来源：http://yue.yj20258.top

JS:   [...s].reverse().join("")
来源：http://zmc.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://bvd.xingfuxueyuan.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://bzt.ywan-chungtsiang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sre.tanke756.top

Ruby: s.reverse
来源：http://drh.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://mxd.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://wdh.fzhhl.top

Py:   s.count("a")
来源：http://uaf.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://ael.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://mxx.316326.xyz

TS:   s.split("a").length - 1
来源：http://jzj.kuanghao11.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qxy.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://gid.ehwqpu.com

Ruby: s.count("a")
来源：http://emn.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://sqh.bbcook.cn

[E13] 逐字符遍历
来源：http://bgd.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://hzt.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://csg.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://oim.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ixy.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mst.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dje.hammf.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://khm.ydzc1.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uqv.cheryme.top

[E14] URL 编码与 Base64
来源：http://xxv.redwolf501.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ssn.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://onj.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dqg.yvedp.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aaf.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://amp.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mdq.hongshengwenyu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dvb.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lcb.gogol.net.cn

[E15] HTML 转义 / 反转义
来源：http://ubb.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://pvr.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ctx.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tpz.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fey.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fnb.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wps.nwbrower.top


<!-- 参考信息 -->