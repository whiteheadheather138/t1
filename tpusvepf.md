代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://ocu.zdbjq.cn

[D08] 合并两个数组
来源：http://qfi.uphjek.com

Py:   a + b;  a.extend(b)
来源：http://sbb.jiagoushi.top

PHP:  array_merge($a, $b);
来源：http://siq.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://lix.cdnleiting.top

TS:   [...a, ...b];
来源：http://aus.ivvv.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://pid.aibaodan.cn

Go:   append(a, b...)
来源：http://aqu.jianghu66.top

Ruby: a + b;  a.concat(b)
来源：http://juy.zhaomingkeji.xyz

C#:   a.Concat(b).ToList()
来源：http://amc.yanxiufei.cn

[D09] 排序（升序）
来源：http://swm.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://yki.zhoulong.xyz

PHP:  sort($arr);
来源：http://ehj.xuanzx.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://fbq.ppjwa.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://jew.tarul.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vbw.tianlin.xyz

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qvm.svipenyu.cn

Ruby: arr.sort
来源：http://weg.zhaomingkeji.xyz

C#:   list.Sort();
来源：http://zac.gotoacloud.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://pey.chenjidiqi.icu

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qwh.52xcode.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wpg.ybcxt.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://pal.fengsongda.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bov.nanxinkj.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://htf.ybcxt.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fqq.shzxlz.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jlt.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ujr.wangdashe.top

[D11] 反转数组
来源：http://rnc.hcnkem.com

Py:   arr[::-1];  arr.reverse()
来源：http://vxu.hammf.cn

PHP:  array_reverse($arr);
来源：http://ugp.zdqjudy.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xch.ydjk.org.cn

TS:   [...arr].reverse();
来源：http://xme.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://skl.316326.xyz

Go:   slices.Reverse(arr)
来源：http://ftv.nanxinkj.top

Ruby: arr.reverse
来源：http://hfq.smart0.xyz

C#:   list.Reverse();
来源：http://gfd.bjfxy.top

[D12] 查找元素下标
来源：http://ktb.cheryme.top

Py:   arr.index(x);  x in arr
来源：http://prr.jqgfzy.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fvf.jinqigufen.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tei.jinghuilouyu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfg.havefunace.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vog.hammf.cn

Go:   slices.Index(arr, x)
来源：http://ahk.nanxuanxn.top

Ruby: arr.index(x)
来源：http://ueq.fanxiaobao.xyz

C#:   list.IndexOf(x);
来源：http://vlc.sjlbkw.cn

[D13] 过滤（保留满足条件的）
来源：http://tnd.jiagoushi.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fuj.smart0.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://prd.aibaodan.cn

JS:   arr.filter(x => x > 3)
来源：http://ymh.snrcjt.cn

TS:   arr.filter(x => x > 3)
来源：http://iro.jqgufenzy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://oic.jinqigfzy.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fzj.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://kzq.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://end.ehwqpu.com

[D14] 映射转换（每个元素变形）
来源：http://cxe.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qsw.wangshuangyany.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://iqx.ydjk.org.cn

JS:   arr.map(x => x * 2)
来源：http://tku.xingfuxueyuan.xyz

TS:   arr.map(x => x * 2)
来源：http://uuv.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://lah.iojbl.cn

Go:   // 手写循环
来源：http://fnj.zhoulong.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://ykl.xuetiantiany.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zip.zhiwuduotai.top

[D15] 去重
来源：http://ngy.chenjidiqi.icu

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kdz.tianlin.xyz

PHP:  array_unique($arr);
来源：http://afx.52xcode.cn

JS:   [...new Set(arr)]
来源：http://bbc.wangshuangyany.cn

TS:   [...new Set(arr)]
来源：http://uzh.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eik.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://oyo.yj20258888.top

Ruby: arr.uniq
来源：http://xax.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://ieq.yongpay.top

[D16] 求和与平均值
来源：http://zio.tarul.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wdu.shzxlz.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hiw.fehbvm.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lmp.yj20258.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ico.yvedp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bph.yj20258888.top

Go:   // 手写循环累加
来源：http://bvm.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cbg.9152youxi.cn

C#:   list.Sum();  list.Average()
来源：http://joq.guowangkeji.top

[D17] 最大值与最小值
来源：http://jyr.cashguo.top

Py:   max(arr);  min(arr)
来源：http://hhh.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://tze.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jnr.jinqigufen.top

TS:   Math.max(...arr);
来源：http://hap.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://sbm.yangfankeji.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uhq.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://jso.kuanghao11.cn

C#:   list.Max();  list.Min()
来源：http://qqs.hnqzz.top

[D18] 扁平化嵌套数组
来源：http://quc.nanxuanxn.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vxc.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://leb.aibaodan.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kfr.hnqzz.top

TS:   nested.flat();
来源：http://kfy.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mcm.mhx1999.top

Go:   // 手写双层循环
来源：http://lie.aibaodan.cn

Ruby: nested.flatten
来源：http://dtj.gzhubu.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://opj.zhiwuduotai.top

[D19] 按字段分组
来源：http://ioo.ppjwa.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vzt.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qim.shangyingyoupin.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kyq.hfpthk.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://owk.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rvy.cucudq.cn

Go:   // 手写 map[string][]T
来源：http://nck.shanyushiyangtech.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oni.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://csb.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://umc.fengsongda.top

Py:   Counter(arr)
来源：http://gaq.yfazqb.com

PHP:  array_count_values($arr);
来源：http://uvz.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vsx.ywan-chungtsiang.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mlm.jinqigufen.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yiw.kuanghao11.cn

Go:   // 手写 map[T]int
来源：http://pqj.birdmap.top

Ruby: arr.tally
来源：http://ohw.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vcu.bjfxy.top

[D21] 判断是否包含某元素
来源：http://kiu.0kj1m.cn

Py:   x in arr
来源：http://nyh.guannengcc.top

PHP:  in_array($x, $arr, true);
来源：http://xme.fzhhl.top

JS:   arr.includes(x)
来源：http://ufm.daxiang520.top

TS:   arr.includes(x)
来源：http://pci.jinghuilouyu.cn

Java: list.contains(x)
来源：http://scn.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://civ.hesvh.cn

Ruby: arr.include?(x)
来源：http://scs.yvedp.cn

C#:   list.Contains(x)
来源：http://wyk.316326.xyz

[D22] 复制数组（避免共享引用）
来源：http://xsp.sjlbkw.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://uct.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hyi.c1oappe.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bdg.cdnleiting.top

TS:   [...arr];
来源：http://gsx.havefunace.top

Java: new ArrayList<>(list);
来源：http://fmv.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://byv.zhixingplan.top

Ruby: arr.dup;  arr.clone
来源：http://vds.chenlongwang.top

C#:   new List<int>(list);
来源：http://dwj.chenjidiqi.icu

[D23] reduce 累积计算
来源：http://dbd.tianlin.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kgs.epnwcf.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uph.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://flp.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://csp.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://cuz.ydjk.org.cn

Go:   // 手写循环
来源：http://qya.smart0.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jfh.xuetiantiany.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uvv.gogol.net.cn

[D24] 字典 / Map 基本操作
来源：http://gnl.jiagoushi.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kie.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ndg.daria6918.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kyd.tarul.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cve.ydjk.org.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gaf.tian-w.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fks.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://aps.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://aav.snrcjt.cn

[D25] Set 集合去重与交并差
来源：http://nvj.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uys.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lzj.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ubd.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lir.aibaodan.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kfs.shzxlz.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lzb.wangshuangyany.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cap.yj202588.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hze.shzxlz.cn

[D26] 数组转字符串
来源：http://vup.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://mfk.sufxvd.cn

PHP:  implode(", ", $arr);
来源：http://ecr.tarul.cn

JS:   arr.join(", ")
来源：http://dwa.bbcook.cn

TS:   arr.join(", ")
来源：http://cyl.wangdashe.top

Java: String.join(", ", list)
来源：http://ilf.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://ggm.yj20258888.top

Ruby: arr.join(", ")
来源：http://crz.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://ety.gzhubu.top

================================================================================
来源：http://uxe.aizwys.cn

E. 字符串处理
来源：http://ynn.chenlongwang.top

================================================================================
来源：http://rxh.birdmap.top

[E01] 拼接字符串
来源：http://vhn.zhoulong.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bmh.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eeq.redwolf501.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tdr.uphjek.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://igp.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jmu.yongpay.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://inw.hysaishi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lqv.yj20258888.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lvh.ppjwa.cn

[E02] 重复字符串
来源：http://bih.yongpay.top

Py:   "ab" * 3
来源：http://epk.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://bex.uphjek.com

JS:   "ab".repeat(3)
来源：http://ref.fktsv.cn

TS:   "ab".repeat(3)
来源：http://frn.yueranfly.top

Java: "ab".repeat(3)
来源：http://dll.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://gtj.hnqzz.top

Ruby: "ab" * 3
来源：http://zhm.hywenlv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nts.yj20258888.top

[E03] 截取子串
来源：http://nrt.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hul.sxryk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rkm.jqgufenzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://guq.epnwcf.com

TS:   s.slice(1, 4)
来源：http://enz.yangfankeji.com

Java: s.substring(1, 4)
来源：http://bsj.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nip.nanxinkj.top

Ruby: s[1, 3];  s[1..3]
来源：http://jby.gotoacloud.top

C#:   s.Substring(1, 3)
来源：http://wbi.smart0.xyz

[E04] 查找子串位置
来源：http://xux.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://rke.wangshuangyany.cn

PHP:  strpos($s, "x");
来源：http://niq.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bvg.birdmap.top

TS:   s.indexOf("x")
来源：http://vcu.ehwqpu.com

Java: s.indexOf("x")
来源：http://xnz.bjfxy.top

Go:   strings.Index(s, "x")
来源：http://abo.nwbrower.top

Ruby: s.index("x")
来源：http://wuf.xylfe.cn

C#:   s.IndexOf("x")
来源：http://qew.mhx1999.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qcs.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nou.xinyue.icu

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rgq.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jbp.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lkx.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ifj.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://moo.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zsl.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kny.yongpay.top

[E06] 替换子串
来源：http://wxq.316326.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lni.hysaishi.cn

PHP:  str_replace("a", "b", $s);
来源：http://wvx.gogol.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://geq.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://ziv.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iqa.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bbw.ywan-chungtsiang.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jas.yangfankeji.com

C#:   s.Replace("a", "b")
来源：http://gck.zhixingplan.top

[E07] 按分隔符拆分
来源：http://gjt.pycfn.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fmu.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lcl.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qbd.yj202588.top

TS:   s.split(",")
来源：http://fbn.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://xnn.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jew.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://yau.ehwqpu.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyn.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://obt.jianghu66.top

Py:   ",".join(items)
来源：http://wib.havefunace.top

PHP:  implode(",", $items);
来源：http://jgp.tian-w.cn

JS:   items.join(",")
来源：http://eqy.kuanghao11.cn

TS:   items.join(",")
来源：http://gog.quarkkingdee.top

Java: String.join(",", items)
来源：http://seh.tanke756.top

Go:   strings.Join(items, ",")
来源：http://bqw.9152youxi.cn

Ruby: items.join(",")
来源：http://khb.dashuyun.cn

C#:   string.Join(",", items)
来源：http://bab.jyoumei.cn

[E09] 去除所有空白字符
来源：http://zdr.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qvb.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yjs.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://mey.yanxiufei.cn

TS:   s.replace(/\s+/g, "")
来源：http://dsd.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://ute.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vcw.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://hkl.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yaz.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://hqc.zhoulong.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gvs.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iyj.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://xol.aibaodan.cn

TS:   "7".padStart(3, "0")
来源：http://ayg.fzhhl.top

Java: String.format("%03d", 7)
来源：http://nwn.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xyf.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uqk.shuidangran.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ios.ctjpmb.com

[E11] 反转字符串
来源：http://hfu.jlsjyb.cn

Py:   s[::-1]
来源：http://viz.ctjpmb.com

PHP:  strrev($s);
来源：http://jln.cheryme.top

JS:   [...s].reverse().join("")
来源：http://qrf.sjlbkw.cn

TS:   [...s].reverse().join("")
来源：http://kkg.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xub.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xlo.quarkkingdee.top

Ruby: s.reverse
来源：http://ccu.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://yow.yj20258.top

[E12] 统计某字符出现次数
来源：http://ebm.cucudq.cn

Py:   s.count("a")
来源：http://ovi.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://ree.vehdjk.com

JS:   s.split("a").length - 1
来源：http://ndp.vehdjk.com

TS:   s.split("a").length - 1
来源：http://iik.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pqw.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://dfb.meibo888.top

Ruby: s.count("a")
来源：http://fbs.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://izi.mhx1999.top

[E13] 逐字符遍历
来源：http://lat.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://daa.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cqh.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://syv.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://nys.dianchejie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://caf.bbcook.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dic.nanxuanxn.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yic.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bsu.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://piy.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dvp.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://yjw.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gpv.316326.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pvs.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yko.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdi.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xfx.birdmap.top


<!-- 参考信息 -->