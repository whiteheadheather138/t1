代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://guu.shanyushiyangtech.top

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ueq.shzxlz.cn

TS:   arr[0]; arr.at(-1);
来源：http://eza.hesvh.cn

Java: list.get(0); list.set(0, 9);
来源：http://cor.yonumen.top

Go:   arr[0]; arr[0] = 9
来源：http://jmr.uphjek.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://dky.xinyue.icu

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kae.zdqjudy.top

[D06] 数组长度
来源：http://lmc.jinyuanbaomall.cn

Py:   len(arr)
来源：http://wwz.daria6918.cn

PHP:  count($arr);
来源：http://xls.epnwcf.com

JS:   arr.length
来源：http://vjr.vehdjk.com

TS:   arr.length
来源：http://kfk.vehdjk.com

Java: list.size();
来源：http://kxa.316326.xyz

Go:   len(arr)
来源：http://ieo.zhengqikj.top

Ruby: arr.length; arr.size
来源：http://tzb.yvedp.cn

C#:   list.Count;
来源：http://kpl.iojbl.cn

[D07] 切片 / 取子数组
来源：http://spm.yueranfly.top

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://egs.hysaishi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lzm.sxryk.cn

JS:   arr.slice(1, 4);
来源：http://mdi.zhaomingkeji.xyz

TS:   arr.slice(1, 4);
来源：http://phd.fzhhl.top

Java: list.subList(1, 4);
来源：http://tsd.aizwys.cn

Go:   arr[1:4]
来源：http://izg.cucudq.cn

Ruby: arr[1, 3]
来源：http://nhh.zycfv.cn

C#:   list.GetRange(1, 3);
来源：http://ypu.aibaodan.cn

[D08] 合并两个数组
来源：http://koi.9152youxi.cn

Py:   a + b;  a.extend(b)
来源：http://pdb.havefunace.top

PHP:  array_merge($a, $b);
来源：http://mli.fanxiaobao.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://vah.yongpay.top

TS:   [...a, ...b];
来源：http://dzj.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hcl.gzhubu.top

Go:   append(a, b...)
来源：http://oub.zhiwuduotai.top

Ruby: a + b;  a.concat(b)
来源：http://afx.epnwcf.com

C#:   a.Concat(b).ToList()
来源：http://ged.jqgfzy.top

[D09] 排序（升序）
来源：http://yxw.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://qqo.yvedp.cn

PHP:  sort($arr);
来源：http://spi.yangfankeji.com

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qvq.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://kbq.pengpengdd.cyou

Java: Collections.sort(list);  list.sort(null);
来源：http://ifo.yj202588.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gta.zhijiandao.cn

Ruby: arr.sort
来源：http://tmf.zhoulong.xyz

C#:   list.Sort();
来源：http://gce.kuanghao11.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cqg.wangdashe.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fxe.xuetiantiany.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yhm.gzhubu.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://asj.zycfv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://djo.316326.xyz

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ukq.gogol.net.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ojh.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dzk.hcnkem.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yqz.jlsjyb.cn

[D11] 反转数组
来源：http://vsy.yuanzhike.top

Py:   arr[::-1];  arr.reverse()
来源：http://tqf.hammf.cn

PHP:  array_reverse($arr);
来源：http://uua.redwolf501.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ryc.havefunace.top

TS:   [...arr].reverse();
来源：http://cyy.jyoumei.cn

Java: Collections.reverse(list);
来源：http://vls.pycfn.com

Go:   slices.Reverse(arr)
来源：http://yja.sufxvd.cn

Ruby: arr.reverse
来源：http://rnx.shangyingyoupin.top

C#:   list.Reverse();
来源：http://agn.ydjk.org.cn

[D12] 查找元素下标
来源：http://kdd.chenlongwang.top

Py:   arr.index(x);  x in arr
来源：http://aui.jianghu66.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://biw.snrcjt.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://djm.yj202588.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xdw.xinyue.icu

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sck.hnxiangtu.top

Go:   slices.Index(arr, x)
来源：http://dfd.vehdjk.com

Ruby: arr.index(x)
来源：http://bwn.haohaochexian.top

C#:   list.IndexOf(x);
来源：http://jld.yvedp.cn

[D13] 过滤（保留满足条件的）
来源：http://ywd.316326.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://dqj.iojbl.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vam.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://szm.yangfankeji.com

TS:   arr.filter(x => x > 3)
来源：http://zvx.52xcode.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qxc.shanyushiyangkeji.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tlp.gotoacloud.top

Ruby: arr.select { |x| x > 3 }
来源：http://vmg.bbcook.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wea.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://mgn.zhengqikj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wjf.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lrj.zhoulong.xyz

JS:   arr.map(x => x * 2)
来源：http://qko.feifeiyinyue.top

TS:   arr.map(x => x * 2)
来源：http://chb.sxryk.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://brw.316326.xyz

Go:   // 手写循环
来源：http://iwv.hysaishi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xks.316326.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://rxg.jinghuilouyu.cn

[D15] 去重
来源：http://oqy.shangyingyoupin.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mor.sweek.top

PHP:  array_unique($arr);
来源：http://vcw.jinghuilouyu.cn

JS:   [...new Set(arr)]
来源：http://vbv.havefunace.top

TS:   [...new Set(arr)]
来源：http://fiu.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://aif.ybcxt.top

Go:   // 用 map[T]struct{} 手写
来源：http://yzo.haohaochexian.top

Ruby: arr.uniq
来源：http://tey.tanke756.top

C#:   list.Distinct().ToList()
来源：http://yjj.svipenyu.cn

[D16] 求和与平均值
来源：http://xss.gogol.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bnd.tarul.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vkp.wangdashe.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nna.havefunace.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dzy.jqgfzy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rpe.tian-w.cn

Go:   // 手写循环累加
来源：http://jky.epnwcf.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zxm.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://njs.wangdashe.top

[D17] 最大值与最小值
来源：http://ogs.hammf.cn

Py:   max(arr);  min(arr)
来源：http://qav.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://oij.c1oappe.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qdt.ctjpmb.com

TS:   Math.max(...arr);
来源：http://nxt.yueranfly.top

Java: Collections.max(list);  Collections.min(list);
来源：http://acm.yj202588.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://iyp.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://vzq.havefunace.top

C#:   list.Max();  list.Min()
来源：http://eog.nanxinkj.top

[D18] 扁平化嵌套数组
来源：http://ufp.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://apb.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://vij.nanxinkj.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bcs.0kj1m.cn

TS:   nested.flat();
来源：http://lih.yonumen.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ccj.ydzc1.top

Go:   // 手写双层循环
来源：http://rol.havefunace.top

Ruby: nested.flatten
来源：http://aml.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lpp.sjlbkw.cn

[D19] 按字段分组
来源：http://fzi.yangfankeji.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://btw.nanxuanxn.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bdp.fehbvm.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://izv.bbcook.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://tqp.cucudq.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hny.xuetiantiany.cn

Go:   // 手写 map[string][]T
来源：http://fof.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dbw.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pdo.nanxinkj.top

[D20] 统计每个元素出现次数
来源：http://eoj.fehbvm.com

Py:   Counter(arr)
来源：http://jbh.hywenlv.cn

PHP:  array_count_values($arr);
来源：http://eyt.yuxming.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dvg.yj20258888.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ale.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yob.svipenyu.cn

Go:   // 手写 map[T]int
来源：http://myo.fktsv.cn

Ruby: arr.tally
来源：http://woq.cdnleiting.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nua.pengpengdd.cyou

[D21] 判断是否包含某元素
来源：http://gpy.yfazqb.com

Py:   x in arr
来源：http://wxo.chenlongwang.top

PHP:  in_array($x, $arr, true);
来源：http://sfm.guowangkeji.top

JS:   arr.includes(x)
来源：http://ogy.shanyushiyangtech.top

TS:   arr.includes(x)
来源：http://izf.shanyushiyangtech.top

Java: list.contains(x)
来源：http://phj.jinqigfzy.top

Go:   slices.Contains(arr, x)
来源：http://ikd.kuanghao11.cn

Ruby: arr.include?(x)
来源：http://mor.gogol.net.cn

C#:   list.Contains(x)
来源：http://wmi.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://qgh.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vzn.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zop.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hkd.xziqi.cn

TS:   [...arr];
来源：http://opf.vqdsnc.cn

Java: new ArrayList<>(list);
来源：http://rbt.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zgp.chenzaomai.com

Ruby: arr.dup;  arr.clone
来源：http://zvr.fengsongda.top

C#:   new List<int>(list);
来源：http://qyv.ehwqpu.com

[D23] reduce 累积计算
来源：http://qkz.gotoacloud.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dmr.mhx1999.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cmf.nanxinkj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zsi.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yxi.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xmc.fanxiaobao.xyz

Go:   // 手写循环
来源：http://tbc.jinqigufen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mdx.tianlin.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lvu.cqqwz.cn

[D24] 字典 / Map 基本操作
来源：http://mov.xuetiantiany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://sjw.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://juj.hesvh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rrq.aizwys.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vsm.shanyushiyangkeji.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hfn.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nrq.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gbt.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejb.havefunace.top

[D25] Set 集合去重与交并差
来源：http://ylu.hnxiangtu.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ymj.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://grj.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nsv.hongshengwenyu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lbq.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rtg.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lqx.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cqu.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zha.yfazqb.com

[D26] 数组转字符串
来源：http://uyd.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://hmk.cdnleiting.top

PHP:  implode(", ", $arr);
来源：http://yla.sweek.top

JS:   arr.join(", ")
来源：http://wyo.dashuyun.cn

TS:   arr.join(", ")
来源：http://owi.9152youxi.cn

Java: String.join(", ", list)
来源：http://lpn.xuetiantiany.cn

Go:   strings.Join(strs, ", ")
来源：http://gho.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://gct.jinghuilouyu.cn

C#:   string.Join(", ", list)
来源：http://ney.tanke756.top

================================================================================
来源：http://syd.haohaochexian.top

E. 字符串处理
来源：http://mmw.aibaodan.cn

================================================================================
来源：http://dsx.jqgufenzy.top

[E01] 拼接字符串
来源：http://okm.yvedp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://miu.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ypa.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xle.yuxming.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lud.smart0.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://skv.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dtv.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bul.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eab.jinghuilouyu.cn

[E02] 重复字符串
来源：http://iwn.bbcook.cn

Py:   "ab" * 3
来源：http://dup.iojbl.cn

PHP:  str_repeat("ab", 3);
来源：http://fgc.zhongyouzk.top

JS:   "ab".repeat(3)
来源：http://iig.cheryme.top

TS:   "ab".repeat(3)
来源：http://zhf.bjfxy.top

Java: "ab".repeat(3)
来源：http://pkd.sjlbkw.cn

Go:   strings.Repeat("ab", 3)
来源：http://flf.chenzaomai.com

Ruby: "ab" * 3
来源：http://lab.fktsv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpf.pengpengdd.cyou

[E03] 截取子串
来源：http://wso.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dnw.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://elo.vqdsnc.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nxh.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://kjd.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://iit.xziqi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bgu.cdnleiting.top

Ruby: s[1, 3];  s[1..3]
来源：http://xiz.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://dgo.yueranfly.top

[E04] 查找子串位置
来源：http://nht.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://ddu.yueranfly.top

PHP:  strpos($s, "x");
来源：http://fru.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ywj.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://iiz.bjfxy.top

Java: s.indexOf("x")
来源：http://thx.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://ocm.mhx1999.top

Ruby: s.index("x")
来源：http://gad.zhixingplan.top

C#:   s.IndexOf("x")
来源：http://lbz.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://kyy.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lvj.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hab.yvedp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nrx.cashguo.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://int.ppjwa.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whi.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ons.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://oeq.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qlo.zhiwuduotai.top

[E06] 替换子串
来源：http://rkh.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://orr.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://anb.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kgu.nanxuanxn.top

TS:   s.replaceAll("a", "b")
来源：http://fvg.yuxming.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nlo.zhengqikj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jrc.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://khn.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://wcu.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://ubh.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wde.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gmv.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://arc.tarul.cn

TS:   s.split(",")
来源：http://kld.daria6918.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zol.redwolf501.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cvo.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://wbt.cheryme.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cpy.uphjek.com

[E08] 数组按分隔符合并
来源：http://kvy.ydzc1.top

Py:   ",".join(items)
来源：http://owr.yuxming.cn

PHP:  implode(",", $items);
来源：http://fiy.yonumen.top

JS:   items.join(",")
来源：http://dem.hfpthk.cn

TS:   items.join(",")
来源：http://rxn.fzhhl.top

Java: String.join(",", items)
来源：http://brw.yonumen.top

Go:   strings.Join(items, ",")
来源：http://bcs.chenjidiqi.icu

Ruby: items.join(",")
来源：http://oep.zdbjq.cn

C#:   string.Join(",", items)
来源：http://uns.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://mza.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://knl.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kik.fanxiaobao.xyz

JS:   s.replace(/\s+/g, "")
来源：http://llq.yongpay.top

TS:   s.replace(/\s+/g, "")
来源：http://hxq.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://pjr.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rgw.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://jmv.xziqi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yds.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://qja.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dmc.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lkk.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://ojq.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://iks.0kj1m.cn

Java: String.format("%03d", 7)
来源：http://ari.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qpz.meibo888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://szr.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mxn.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://upi.shuidangran.top

Py:   s[::-1]
来源：http://nsb.bbcook.cn

PHP:  strrev($s);
来源：http://zem.fzhhl.top

JS:   [...s].reverse().join("")
来源：http://mwb.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://ycc.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://llj.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://icz.nanxinkj.top

Ruby: s.reverse
来源：http://ipj.shanyushiyangtech.top

C#:   new string(s.Reverse().ToArray())
来源：http://yus.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://scj.wangshuangyany.cn

Py:   s.count("a")
来源：http://ceb.feifeiyinyue.top


<!-- 参考信息 -->