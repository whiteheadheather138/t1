代发 wailian999

[D07] 切片 / 取子数组
来源：http://zql.gaohongyu789.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mnz.cqqwz.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dnp.vqdsnc.cn

JS:   arr.slice(1, 4);
来源：http://szi.fengsongda.top

TS:   arr.slice(1, 4);
来源：http://pci.nanxinkj.top

Java: list.subList(1, 4);
来源：http://jfu.tarul.cn

Go:   arr[1:4]
来源：http://omd.chenjidiqi.icu

Ruby: arr[1, 3]
来源：http://cwj.dashuyun.cn

C#:   list.GetRange(1, 3);
来源：http://hcw.dashuyun.cn

[D08] 合并两个数组
来源：http://rmo.ivvv.top

Py:   a + b;  a.extend(b)
来源：http://nsa.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://csu.feifeiyinyue.top

JS:   [...a, ...b];  a.concat(b);
来源：http://uyw.jiagoushi.top

TS:   [...a, ...b];
来源：http://rly.epnwcf.com

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mkv.xylfe.cn

Go:   append(a, b...)
来源：http://geh.sweek.top

Ruby: a + b;  a.concat(b)
来源：http://vxv.yfazqb.com

C#:   a.Concat(b).ToList()
来源：http://ccf.zhengqikj.top

[D09] 排序（升序）
来源：http://org.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://aoz.vehdjk.com

PHP:  sort($arr);
来源：http://qsq.yuanzhike.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ikk.daxiang520.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://lgv.gzhubu.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ffe.sjlbkw.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://heh.xinyue.icu

Ruby: arr.sort
来源：http://qjo.zhiwuduotai.top

C#:   list.Sort();
来源：http://xlh.wangdashe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bet.xylfe.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xpn.bjfxy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://joq.yueranfly.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cqg.jianghu66.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gbw.tanke756.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ghd.jiagoushi.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sqn.jqgfzy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hbd.jqgufenzy.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://eqo.fktsv.cn

[D11] 反转数组
来源：http://bfo.cashguo.top

Py:   arr[::-1];  arr.reverse()
来源：http://dnq.nwbrower.top

PHP:  array_reverse($arr);
来源：http://zni.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ksm.cashguo.top

TS:   [...arr].reverse();
来源：http://bda.zhijiandao.cn

Java: Collections.reverse(list);
来源：http://nmw.gzhubu.top

Go:   slices.Reverse(arr)
来源：http://pzh.hnqzz.top

Ruby: arr.reverse
来源：http://rsp.tanke756.top

C#:   list.Reverse();
来源：http://ivm.fzhhl.top

[D12] 查找元素下标
来源：http://iea.bjfxy.top

Py:   arr.index(x);  x in arr
来源：http://kxf.fehbvm.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gcj.cdnleiting.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmy.pycfn.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://htg.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xcf.zhiwuduotai.top

Go:   slices.Index(arr, x)
来源：http://psk.ctjpmb.com

Ruby: arr.index(x)
来源：http://icq.hnqzz.top

C#:   list.IndexOf(x);
来源：http://hop.daxiang520.top

[D13] 过滤（保留满足条件的）
来源：http://vqq.sufxvd.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yzl.gzhubu.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://kyz.hcnkem.com

JS:   arr.filter(x => x > 3)
来源：http://tdm.9152youxi.cn

TS:   arr.filter(x => x > 3)
来源：http://msc.ydjk.org.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://auu.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ytw.xinyue.icu

Ruby: arr.select { |x| x > 3 }
来源：http://egf.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pdx.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://bnf.zhixingplan.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qui.jlsjyb.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hez.ppjwa.cn

JS:   arr.map(x => x * 2)
来源：http://tht.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://qrx.cucudq.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ooy.dashuyun.cn

Go:   // 手写循环
来源：http://mbd.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://mfq.52xcode.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://knt.redwolf501.top

[D15] 去重
来源：http://pvn.zdbjq.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hfa.sufxvd.cn

PHP:  array_unique($arr);
来源：http://hkk.hesvh.cn

JS:   [...new Set(arr)]
来源：http://bxx.cheryme.top

TS:   [...new Set(arr)]
来源：http://edf.quarkkingdee.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://osx.zdbjq.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kti.vqdsnc.cn

Ruby: arr.uniq
来源：http://ppk.gotoacloud.top

C#:   list.Distinct().ToList()
来源：http://jag.jianghu66.top

[D16] 求和与平均值
来源：http://usu.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ysf.jinqigufen.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nau.yueranfly.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vts.xuetiantiany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ihl.hcnkem.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xfs.zdbjq.cn

Go:   // 手写循环累加
来源：http://hay.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pqg.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://nlc.sxryk.cn

[D17] 最大值与最小值
来源：http://vwv.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://mah.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://akb.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fzx.shanyushiyangtech.top

TS:   Math.max(...arr);
来源：http://srj.yanxiufei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yrs.cheryme.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zzx.chenjidiqi.icu

Ruby: arr.max;  arr.min
来源：http://srn.shzxlz.cn

C#:   list.Max();  list.Min()
来源：http://ymc.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://enh.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://crp.fanxiaobao.xyz

PHP:  array_merge(...$nested);
来源：http://szp.yvedp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://scc.epnwcf.com

TS:   nested.flat();
来源：http://smy.yanxiufei.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nci.xinyue.icu

Go:   // 手写双层循环
来源：http://rlx.dianchejie.cn

Ruby: nested.flatten
来源：http://cwa.yj202588.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://fzg.epnwcf.com

[D19] 按字段分组
来源：http://vzs.jinyuanbaomall.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vjq.ivvv.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mfb.yvedp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zuo.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fyp.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://shz.birdmap.top

Go:   // 手写 map[string][]T
来源：http://gff.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://pek.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ukc.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://iul.uphjek.com

Py:   Counter(arr)
来源：http://xaq.xuanzx.com

PHP:  array_count_values($arr);
来源：http://vld.gaohongyu789.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xaw.jqgufenzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bna.cheryme.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qkz.hnqzz.top

Go:   // 手写 map[T]int
来源：http://csz.nanxuanxn.top

Ruby: arr.tally
来源：http://wvg.yueranfly.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://woa.jlsjyb.cn

[D21] 判断是否包含某元素
来源：http://uef.yuxming.cn

Py:   x in arr
来源：http://pkx.redwolf501.top

PHP:  in_array($x, $arr, true);
来源：http://uuq.vehdjk.com

JS:   arr.includes(x)
来源：http://sau.redwolf501.top

TS:   arr.includes(x)
来源：http://txi.zdqjudy.top

Java: list.contains(x)
来源：http://ddl.jlsjyb.cn

Go:   slices.Contains(arr, x)
来源：http://jrh.yj20258.top

Ruby: arr.include?(x)
来源：http://shj.svipenyu.cn

C#:   list.Contains(x)
来源：http://bzi.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://uxl.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://che.hfpthk.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cdw.sjlbkw.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gli.cdnleiting.top

TS:   [...arr];
来源：http://kta.meibo888.top

Java: new ArrayList<>(list);
来源：http://vxi.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://riy.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://uyn.meibo888.top

C#:   new List<int>(list);
来源：http://ate.epnwcf.com

[D23] reduce 累积计算
来源：http://wqw.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gug.zdbjq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vrf.jqgufenzy.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://txw.ivvv.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://omh.tanke756.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xry.hammf.cn

Go:   // 手写循环
来源：http://kbp.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gyg.tanke756.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://aen.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://ryz.gaohongyu789.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://odc.fengsongda.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bom.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qzy.xinyue.icu

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://eth.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rce.yonumen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zen.shuidangran.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tyc.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ivq.hongshengwenyu.top

[D25] Set 集合去重与交并差
来源：http://iot.feifeiyinyue.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ptg.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ilv.jqgfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kaf.pycfn.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://emr.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dyp.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dvi.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://vfy.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nys.c1oappe.top

[D26] 数组转字符串
来源：http://iss.zycfv.cn

Py:   ", ".join(map(str, arr))
来源：http://nod.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://nke.kuanghao11.cn

JS:   arr.join(", ")
来源：http://ixo.cashguo.top

TS:   arr.join(", ")
来源：http://dfg.0kj1m.cn

Java: String.join(", ", list)
来源：http://rqr.shanyushiyangtech.top

Go:   strings.Join(strs, ", ")
来源：http://kzj.zhijiandao.cn

Ruby: arr.join(", ")
来源：http://jzu.hammf.cn

C#:   string.Join(", ", list)
来源：http://sgh.ydjk.org.cn

================================================================================
来源：http://fnc.cashguo.top

E. 字符串处理
来源：http://gln.nanxinkj.top

================================================================================
来源：http://hbk.chenzaomai.com

[E01] 拼接字符串
来源：http://ouh.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cxx.xinyue.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jes.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qda.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfy.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zdh.hfpthk.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hlw.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vsd.haohaochexian.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sti.zhixingplan.top

[E02] 重复字符串
来源：http://tye.yonumen.top

Py:   "ab" * 3
来源：http://kga.chenlongwang.top

PHP:  str_repeat("ab", 3);
来源：http://huq.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://wmw.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://hui.fehbvm.com

Java: "ab".repeat(3)
来源：http://hid.fanxiaobao.xyz

Go:   strings.Repeat("ab", 3)
来源：http://rmr.xinyue.icu

Ruby: "ab" * 3
来源：http://vpn.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nun.zhixingplan.top

[E03] 截取子串
来源：http://jfx.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://znq.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nyp.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aaa.kuanghao11.cn

TS:   s.slice(1, 4)
来源：http://ybm.cheryme.top

Java: s.substring(1, 4)
来源：http://mtt.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jba.haohaochexian.top

Ruby: s[1, 3];  s[1..3]
来源：http://hmt.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://hhz.cashguo.top

[E04] 查找子串位置
来源：http://swh.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://wjb.yonumen.top

PHP:  strpos($s, "x");
来源：http://tkf.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kdt.sysykeji.top

TS:   s.indexOf("x")
来源：http://qqu.ctjpmb.com

Java: s.indexOf("x")
来源：http://xtt.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://qhe.yanxiufei.cn

Ruby: s.index("x")
来源：http://szg.tanke756.top

C#:   s.IndexOf("x")
来源：http://rzp.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zkx.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bct.ydjk.org.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hua.havefunace.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fyl.316326.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ile.wangshuangyany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://exs.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hbj.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pku.fzhhl.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pek.fehbvm.com

[E06] 替换子串
来源：http://hye.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uij.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://ava.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hgd.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://egz.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://olw.fehbvm.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjb.aizwys.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eta.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://lvq.chenlongwang.top

[E07] 按分隔符拆分
来源：http://qja.jyoumei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hgv.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bxk.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cpk.cdnleiting.top

TS:   s.split(",")
来源：http://mov.nanxinkj.top

Java: s.split(",");  s.split("\\s+")
来源：http://esu.52xcode.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ujk.haohaochexian.top

Ruby: s.split(",");  s.split
来源：http://dfa.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dqi.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://woo.tian-w.cn

Py:   ",".join(items)
来源：http://klf.hammf.cn

PHP:  implode(",", $items);
来源：http://etg.zhixingplan.top

JS:   items.join(",")
来源：http://esy.shzxlz.cn

TS:   items.join(",")
来源：http://rdw.meibo888.top

Java: String.join(",", items)
来源：http://wjb.hammf.cn

Go:   strings.Join(items, ",")
来源：http://mab.redwolf501.top

Ruby: items.join(",")
来源：http://exn.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://fzp.redwolf501.top

[E09] 去除所有空白字符
来源：http://qoj.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ghf.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sok.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://wkn.andypj.xyz

TS:   s.replace(/\s+/g, "")
来源：http://tcf.cheryme.top

Java: s.replaceAll("\\s+", "")
来源：http://rzx.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://umx.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://byx.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yjs.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://ocr.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://inq.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zeu.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://ilj.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://klw.guannengcc.top

Java: String.format("%03d", 7)
来源：http://iji.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://cbs.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vdn.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cmh.gzhubu.top

[E11] 反转字符串
来源：http://nxh.yvedp.cn

Py:   s[::-1]
来源：http://hxm.gotoacloud.top

PHP:  strrev($s);
来源：http://uit.kuanghao11.cn

JS:   [...s].reverse().join("")
来源：http://hxm.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://okw.smart0.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://ubn.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://tdb.sufxvd.cn

Ruby: s.reverse
来源：http://rab.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lqg.birdmap.top

[E12] 统计某字符出现次数
来源：http://pfi.bbcook.cn

Py:   s.count("a")
来源：http://bkv.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://qjm.yongpay.top

JS:   s.split("a").length - 1
来源：http://byb.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://btz.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://obq.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://qie.bjfxy.top

Ruby: s.count("a")
来源：http://npn.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://jqt.jqgufenzy.top

[E13] 逐字符遍历
来源：http://dwm.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://wjw.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eux.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://fkd.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hfe.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vyg.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fmr.xylfe.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ewf.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aku.gotoacloud.top


<!-- 参考信息 -->