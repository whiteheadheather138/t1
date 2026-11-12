代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://gmm.yuanzhike.top

C#:   a.Concat(b).ToList()
来源：http://nnv.jqgufenzy.top

[D09] 排序（升序）
来源：http://jko.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://ter.daxiang520.top

PHP:  sort($arr);
来源：http://tpf.pengpengdd.cyou

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bsx.xziqi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://crb.feifeiyinyue.top

Java: Collections.sort(list);  list.sort(null);
来源：http://ymx.yongpay.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://adi.hywenlv.cn

Ruby: arr.sort
来源：http://bmd.sxryk.cn

C#:   list.Sort();
来源：http://fuf.bbcook.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ceq.hcnkem.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xbz.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aac.gotoacloud.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qee.fzhhl.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bgq.daxiang520.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xna.yj20258.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gqq.yuanzhike.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kwx.shangyingyoupin.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vbv.zhaomingkeji.xyz

[D11] 反转数组
来源：http://ytc.ppjwa.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wqs.havefunace.top

PHP:  array_reverse($arr);
来源：http://tdf.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://izd.gotoacloud.top

TS:   [...arr].reverse();
来源：http://hfg.gaohongyu789.top

Java: Collections.reverse(list);
来源：http://uot.andypj.xyz

Go:   slices.Reverse(arr)
来源：http://zmq.jianghu66.top

Ruby: arr.reverse
来源：http://grt.cashguo.top

C#:   list.Reverse();
来源：http://tbu.epnwcf.com

[D12] 查找元素下标
来源：http://rwi.havefunace.top

Py:   arr.index(x);  x in arr
来源：http://twp.yvedp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://yez.yfazqb.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qho.yvedp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lmj.hysaishi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mlx.cheryme.top

Go:   slices.Index(arr, x)
来源：http://gsl.52xcode.cn

Ruby: arr.index(x)
来源：http://swk.sxryk.cn

C#:   list.IndexOf(x);
来源：http://alg.52xcode.cn

[D13] 过滤（保留满足条件的）
来源：http://qox.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://aey.nanxuanxn.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mpy.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://skp.zycfv.cn

TS:   arr.filter(x => x > 3)
来源：http://vzz.xingfuxueyuan.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lvf.yuanzhike.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ady.ydzc1.top

Ruby: arr.select { |x| x > 3 }
来源：http://ayo.ehwqpu.com

C#:   list.Where(x => x > 3).ToList()
来源：http://kbb.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://fhs.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://aqw.fehbvm.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vbq.tarul.cn

JS:   arr.map(x => x * 2)
来源：http://smm.kuanghao11.cn

TS:   arr.map(x => x * 2)
来源：http://tqb.vqdsnc.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qaz.sjlbkw.cn

Go:   // 手写循环
来源：http://rpc.hammf.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qac.fengsongda.top

C#:   list.Select(x => x * 2).ToList()
来源：http://gme.ydjk.org.cn

[D15] 去重
来源：http://lmy.tian-w.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yfj.sweek.top

PHP:  array_unique($arr);
来源：http://iqb.shangyingyoupin.top

JS:   [...new Set(arr)]
来源：http://mii.feifeiyinyue.top

TS:   [...new Set(arr)]
来源：http://bbu.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lai.wangdashe.top

Go:   // 用 map[T]struct{} 手写
来源：http://nxm.sjlbkw.cn

Ruby: arr.uniq
来源：http://piq.meibo888.top

C#:   list.Distinct().ToList()
来源：http://pox.guowangkeji.top

[D16] 求和与平均值
来源：http://crv.jiagoushi.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gbn.uphjek.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://unv.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ycy.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dkd.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ljl.yj202588.top

Go:   // 手写循环累加
来源：http://uzd.wangdashe.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mwg.shzxlz.cn

C#:   list.Sum();  list.Average()
来源：http://mnq.guannengcc.top

[D17] 最大值与最小值
来源：http://vgm.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://adt.hywenlv.cn

PHP:  max($arr);  min($arr);
来源：http://esd.tian-w.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eqp.guowangkeji.top

TS:   Math.max(...arr);
来源：http://cnv.wangdashe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://jwk.chenlongwang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aqx.yvedp.cn

Ruby: arr.max;  arr.min
来源：http://xsd.fzhhl.top

C#:   list.Max();  list.Min()
来源：http://hag.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://opj.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sgy.ydzc1.top

PHP:  array_merge(...$nested);
来源：http://yfk.yanxiufei.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eld.jyoumei.cn

TS:   nested.flat();
来源：http://gld.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zyl.iojbl.cn

Go:   // 手写双层循环
来源：http://ybr.jlsjyb.cn

Ruby: nested.flatten
来源：http://mpw.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ssj.zdbjq.cn

[D19] 按字段分组
来源：http://cic.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cxd.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oth.guowangkeji.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jix.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://fmw.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://usa.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://mgy.nwbrower.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vqt.pycfn.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tjk.mhx1999.top

[D20] 统计每个元素出现次数
来源：http://haw.yueranfly.top

Py:   Counter(arr)
来源：http://elq.ydzc1.top

PHP:  array_count_values($arr);
来源：http://shi.tian-w.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://akj.vqdsnc.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gtw.zdqjudy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dag.aizwys.cn

Go:   // 手写 map[T]int
来源：http://xsj.yvedp.cn

Ruby: arr.tally
来源：http://hsd.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vhv.xziqi.cn

[D21] 判断是否包含某元素
来源：http://ppu.ctjpmb.com

Py:   x in arr
来源：http://dmp.zhaomingkeji.xyz

PHP:  in_array($x, $arr, true);
来源：http://swn.gzhubu.top

JS:   arr.includes(x)
来源：http://tek.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://xlj.hysaishi.cn

Java: list.contains(x)
来源：http://oyf.daria6918.cn

Go:   slices.Contains(arr, x)
来源：http://beg.chenlongwang.top

Ruby: arr.include?(x)
来源：http://llk.yongpay.top

C#:   list.Contains(x)
来源：http://jpb.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://vti.jinqigufen.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mpl.sysykeji.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ian.xuanzx.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rfw.yongpay.top

TS:   [...arr];
来源：http://cfy.chenjidiqi.icu

Java: new ArrayList<>(list);
来源：http://wei.fktsv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ygv.yj20258888.top

Ruby: arr.dup;  arr.clone
来源：http://lfm.smart0.xyz

C#:   new List<int>(list);
来源：http://syh.c1oappe.top

[D23] reduce 累积计算
来源：http://fmo.sxryk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xif.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://onq.jinyuanbaomall.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zuh.shzxlz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ypv.tarul.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zrk.jqgufenzy.top

Go:   // 手写循环
来源：http://nyx.jlsjyb.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rjq.chenlongwang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kuf.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://iaw.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rwh.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sjv.hfpthk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jym.zhaomingkeji.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://itx.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qus.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fvu.jinqigufen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yqn.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qjn.havefunace.top

[D25] Set 集合去重与交并差
来源：http://jng.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bsr.sufxvd.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dnl.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://giw.meibo888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://oop.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wqo.ydzc1.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nmu.wangdashe.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wvk.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zuq.snrcjt.cn

[D26] 数组转字符串
来源：http://mjd.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://tid.jqgufenzy.top

PHP:  implode(", ", $arr);
来源：http://wki.hywenlv.cn

JS:   arr.join(", ")
来源：http://jqj.tian-w.cn

TS:   arr.join(", ")
来源：http://vpl.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://avu.wangshuangyany.cn

Go:   strings.Join(strs, ", ")
来源：http://dht.kuanghao11.cn

Ruby: arr.join(", ")
来源：http://wcz.vehdjk.com

C#:   string.Join(", ", list)
来源：http://otf.sjlbkw.cn

================================================================================
来源：http://wtb.hesvh.cn

E. 字符串处理
来源：http://qwm.nanxuanxn.top

================================================================================
来源：http://mrp.uphjek.com

[E01] 拼接字符串
来源：http://uwd.cdnleiting.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cpg.sufxvd.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hlg.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://omh.zhixingplan.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfl.andypj.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jrw.hesvh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vcu.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gmz.wangshuangyany.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gqc.shanyushiyangtech.top

[E02] 重复字符串
来源：http://ywa.bjfxy.top

Py:   "ab" * 3
来源：http://lsu.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://ksl.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://pek.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://cou.jiagoushi.top

Java: "ab".repeat(3)
来源：http://nze.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://srq.cqqwz.cn

Ruby: "ab" * 3
来源：http://rit.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gug.tianlin.xyz

[E03] 截取子串
来源：http://vno.quarkkingdee.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dmr.sysykeji.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pic.xziqi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ccq.jianghu66.top

TS:   s.slice(1, 4)
来源：http://ahp.tarul.cn

Java: s.substring(1, 4)
来源：http://rmk.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://egs.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uuw.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://olk.snrcjt.cn

[E04] 查找子串位置
来源：http://kzw.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://vnn.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://pch.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dyk.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://jfu.yueranfly.top

Java: s.indexOf("x")
来源：http://dnp.ppjwa.cn

Go:   strings.Index(s, "x")
来源：http://oeh.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://rma.yfazqb.com

C#:   s.IndexOf("x")
来源：http://gtx.yuxming.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cdo.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rzw.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cae.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eff.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zaj.bbcook.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vlz.feifeiyinyue.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dtw.feifeiyinyue.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ait.52xcode.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://joj.shuidangran.top

[E06] 替换子串
来源：http://six.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hfj.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://kia.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://owe.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://iyt.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://weq.tian-w.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jrl.hywenlv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uyv.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://asa.yfazqb.com

[E07] 按分隔符拆分
来源：http://nbz.sxryk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eyb.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wip.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sxj.gogol.net.cn

TS:   s.split(",")
来源：http://gnq.uphjek.com

Java: s.split(",");  s.split("\\s+")
来源：http://czf.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iac.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://ivx.yj20258888.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bqn.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://xnv.zycfv.cn

Py:   ",".join(items)
来源：http://ahq.shuidangran.top

PHP:  implode(",", $items);
来源：http://tox.fengsongda.top

JS:   items.join(",")
来源：http://vhv.jianghu66.top

TS:   items.join(",")
来源：http://rut.havefunace.top

Java: String.join(",", items)
来源：http://cce.yj20258888.top

Go:   strings.Join(items, ",")
来源：http://yzx.xylfe.cn

Ruby: items.join(",")
来源：http://ufh.yj202588.top

C#:   string.Join(",", items)
来源：http://any.sweek.top

[E09] 去除所有空白字符
来源：http://iyc.tianlin.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dnr.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://djh.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://zkb.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://zke.gzhubu.top

Java: s.replaceAll("\\s+", "")
来源：http://wmp.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mze.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ifx.hywenlv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://otc.shzxlz.cn

[E10] 左侧补零 / 定长填充
来源：http://lmf.bbcook.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rgs.haohaochexian.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://myi.pengpengdd.cyou

JS:   "7".padStart(3, "0")
来源：http://koi.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://gxj.hysaishi.cn

Java: String.format("%03d", 7)
来源：http://lwo.gzhubu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kms.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rva.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cwu.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://trs.xinyue.icu

Py:   s[::-1]
来源：http://ezy.zhiwuduotai.top

PHP:  strrev($s);
来源：http://dik.cashguo.top

JS:   [...s].reverse().join("")
来源：http://ipx.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://pdu.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gfq.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bqo.tanke756.top

Ruby: s.reverse
来源：http://svq.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fzx.ybcxt.top

[E12] 统计某字符出现次数
来源：http://fvr.cashguo.top

Py:   s.count("a")
来源：http://hot.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://tat.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://gkb.nwbrower.top

TS:   s.split("a").length - 1
来源：http://tuu.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://isx.meibo888.top

Go:   strings.Count(s, "a")
来源：http://hya.hesvh.cn

Ruby: s.count("a")
来源：http://dlx.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://opm.zhongyouzk.top

[E13] 逐字符遍历
来源：http://rms.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://lfj.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iev.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exu.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://axb.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uic.yonumen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmf.wangdashe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://utz.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uhv.fktsv.cn

[E14] URL 编码与 Base64
来源：http://acy.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mbf.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://unl.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://klr.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uyd.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bot.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rjm.dashuyun.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wpy.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oub.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://ouc.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://quu.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zjk.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mbu.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ygt.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldr.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yal.sxryk.cn


<!-- 参考信息 -->