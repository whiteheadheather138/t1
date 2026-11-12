代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hbt.gogol.net.cn

Java: list.subList(1, 4);
来源：http://upm.vehdjk.com

Go:   arr[1:4]
来源：http://vnx.cqqwz.cn

Ruby: arr[1, 3]
来源：http://wfx.yuxming.cn

C#:   list.GetRange(1, 3);
来源：http://ibd.jqgfzy.top

[D08] 合并两个数组
来源：http://jql.hnqzz.top

Py:   a + b;  a.extend(b)
来源：http://glz.zhaomingkeji.xyz

PHP:  array_merge($a, $b);
来源：http://nui.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://uii.chenjidiqi.icu

TS:   [...a, ...b];
来源：http://vqp.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zou.ydzc1.top

Go:   append(a, b...)
来源：http://kfw.jqgufenzy.top

Ruby: a + b;  a.concat(b)
来源：http://lon.jianghu66.top

C#:   a.Concat(b).ToList()
来源：http://dtb.ehwqpu.com

[D09] 排序（升序）
来源：http://xms.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xsv.hywenlv.cn

PHP:  sort($arr);
来源：http://ihu.hnxiangtu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://awm.ivvv.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://ykb.316326.xyz

Java: Collections.sort(list);  list.sort(null);
来源：http://rjg.redwolf501.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cdf.nanxuanxn.top

Ruby: arr.sort
来源：http://nwn.52xcode.cn

C#:   list.Sort();
来源：http://vsz.ybcxt.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://eih.aizwys.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mre.smart0.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ucw.52xcode.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ntl.kuanghao11.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hom.hcnkem.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tim.jyoumei.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hbm.yfazqb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sba.sxryk.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qip.yj20258888.top

[D11] 反转数组
来源：http://sug.quarkkingdee.top

Py:   arr[::-1];  arr.reverse()
来源：http://nra.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://odw.zhengqikj.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wwt.pycfn.com

TS:   [...arr].reverse();
来源：http://nun.jqgufenzy.top

Java: Collections.reverse(list);
来源：http://qws.birdmap.top

Go:   slices.Reverse(arr)
来源：http://okd.yj20258888.top

Ruby: arr.reverse
来源：http://txl.ivvv.top

C#:   list.Reverse();
来源：http://fmy.wangshuangyany.cn

[D12] 查找元素下标
来源：http://fbv.jinghuilouyu.cn

Py:   arr.index(x);  x in arr
来源：http://yvy.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oec.quarkkingdee.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://syq.guannengcc.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oui.sweek.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ota.ydzc1.top

Go:   slices.Index(arr, x)
来源：http://nob.tarul.cn

Ruby: arr.index(x)
来源：http://shr.dianchejie.cn

C#:   list.IndexOf(x);
来源：http://sdg.zycfv.cn

[D13] 过滤（保留满足条件的）
来源：http://oab.uphjek.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tnr.zhongyouzk.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://owj.jlsjyb.cn

JS:   arr.filter(x => x > 3)
来源：http://ttz.sxryk.cn

TS:   arr.filter(x => x > 3)
来源：http://tjb.hongshengwenyu.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xbc.jinqigufen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tab.shzxlz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cbs.svipenyu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://utu.dashuyun.cn

[D14] 映射转换（每个元素变形）
来源：http://gdp.nanxinkj.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://tim.chenjidiqi.icu

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lbu.wangdashe.top

JS:   arr.map(x => x * 2)
来源：http://lhc.fengsongda.top

TS:   arr.map(x => x * 2)
来源：http://nku.redwolf501.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://tyl.xuetiantiany.cn

Go:   // 手写循环
来源：http://fdc.shanyushiyangtech.top

Ruby: arr.map { |x| x * 2 }
来源：http://dkg.gaohongyu789.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cqk.mhx1999.top

[D15] 去重
来源：http://tud.zdqjudy.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zan.yfazqb.com

PHP:  array_unique($arr);
来源：http://awc.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://xmf.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://ygl.tanke756.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ero.ehwqpu.com

Go:   // 用 map[T]struct{} 手写
来源：http://tgk.nanxinkj.top

Ruby: arr.uniq
来源：http://omt.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://fch.meibo888.top

[D16] 求和与平均值
来源：http://bsd.sxryk.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tqv.dianchejie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mem.bjfxy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uok.yj20258888.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://skw.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vyj.yanxiufei.cn

Go:   // 手写循环累加
来源：http://xru.jqgufenzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xsq.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://ikz.sufxvd.cn

[D17] 最大值与最小值
来源：http://oyr.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://vgl.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://olg.andypj.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qws.hesvh.cn

TS:   Math.max(...arr);
来源：http://xor.daria6918.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dub.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aci.guowangkeji.top

Ruby: arr.max;  arr.min
来源：http://jay.yongpay.top

C#:   list.Max();  list.Min()
来源：http://twj.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://lye.bbcook.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jed.nwbrower.top

PHP:  array_merge(...$nested);
来源：http://srp.cashguo.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://bfd.dashuyun.cn

TS:   nested.flat();
来源：http://fec.birdmap.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ehw.cdnleiting.top

Go:   // 手写双层循环
来源：http://bcg.mhx1999.top

Ruby: nested.flatten
来源：http://txi.zhoulong.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://zkz.yueranfly.top

[D19] 按字段分组
来源：http://vub.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zpk.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://krr.hfpthk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xno.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://max.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xxi.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://vkq.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wmi.zhijiandao.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qrn.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://xkj.hongshengwenyu.top

Py:   Counter(arr)
来源：http://egi.quarkkingdee.top

PHP:  array_count_values($arr);
来源：http://eat.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://npn.zhiwuduotai.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vvx.ppjwa.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xvl.sufxvd.cn

Go:   // 手写 map[T]int
来源：http://vus.guannengcc.top

Ruby: arr.tally
来源：http://cfv.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://sok.cqqwz.cn

[D21] 判断是否包含某元素
来源：http://nsx.tanke756.top

Py:   x in arr
来源：http://ldj.pengpengdd.cyou

PHP:  in_array($x, $arr, true);
来源：http://rsr.yongpay.top

JS:   arr.includes(x)
来源：http://qcl.316326.xyz

TS:   arr.includes(x)
来源：http://uql.aibaodan.cn

Java: list.contains(x)
来源：http://emw.sysykeji.top

Go:   slices.Contains(arr, x)
来源：http://svt.yueranfly.top

Ruby: arr.include?(x)
来源：http://muo.vehdjk.com

C#:   list.Contains(x)
来源：http://hru.zhongyouzk.top

[D22] 复制数组（避免共享引用）
来源：http://nja.zhoulong.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dtv.pycfn.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pes.hnqzz.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://csb.fktsv.cn

TS:   [...arr];
来源：http://sth.daxiang520.top

Java: new ArrayList<>(list);
来源：http://ork.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://wch.ivvv.top

Ruby: arr.dup;  arr.clone
来源：http://qtf.sxryk.cn

C#:   new List<int>(list);
来源：http://irw.zhoulong.xyz

[D23] reduce 累积计算
来源：http://oya.meibo888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jqc.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xxg.tanke756.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shn.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rpq.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://lpt.shangyingyoupin.top

Go:   // 手写循环
来源：http://tju.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hms.yvedp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mnw.nwbrower.top

[D24] 字典 / Map 基本操作
来源：http://awc.sweek.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ogp.zhongyouzk.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ipc.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jex.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wjq.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://slt.hywenlv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yph.yonumen.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vce.xinyue.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yaw.smart0.xyz

[D25] Set 集合去重与交并差
来源：http://hky.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pvj.xylfe.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uck.yfazqb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eyf.snrcjt.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gvt.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cco.ehwqpu.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pbg.yvedp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wtz.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xmt.daxiang520.top

[D26] 数组转字符串
来源：http://aid.zhiwuduotai.top

Py:   ", ".join(map(str, arr))
来源：http://kkd.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://eyc.mhx1999.top

JS:   arr.join(", ")
来源：http://guh.tian-w.cn

TS:   arr.join(", ")
来源：http://ohs.zhiwuduotai.top

Java: String.join(", ", list)
来源：http://avk.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://upa.bbcook.cn

Ruby: arr.join(", ")
来源：http://rov.zhengqikj.top

C#:   string.Join(", ", list)
来源：http://jgl.nwbrower.top

================================================================================
来源：http://ihv.yj202588.top

E. 字符串处理
来源：http://osm.yangfankeji.com

================================================================================
来源：http://zpa.pengpengdd.cyou

[E01] 拼接字符串
来源：http://puj.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ujl.hcnkem.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tsn.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bir.sxryk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://myt.cucudq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ufd.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qvb.zycfv.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vbf.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sey.quarkkingdee.top

[E02] 重复字符串
来源：http://ihr.xuetiantiany.cn

Py:   "ab" * 3
来源：http://uus.xylfe.cn

PHP:  str_repeat("ab", 3);
来源：http://eno.fanxiaobao.xyz

JS:   "ab".repeat(3)
来源：http://gyy.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://wtp.nwbrower.top

Java: "ab".repeat(3)
来源：http://ugj.sysykeji.top

Go:   strings.Repeat("ab", 3)
来源：http://aie.tanke756.top

Ruby: "ab" * 3
来源：http://zjw.svipenyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://euz.zdbjq.cn

[E03] 截取子串
来源：http://bgd.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qoz.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nsf.gaohongyu789.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xbd.vqdsnc.cn

TS:   s.slice(1, 4)
来源：http://lni.vqdsnc.cn

Java: s.substring(1, 4)
来源：http://cma.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fek.epnwcf.com

Ruby: s[1, 3];  s[1..3]
来源：http://chr.jinghuilouyu.cn

C#:   s.Substring(1, 3)
来源：http://hwg.cucudq.cn

[E04] 查找子串位置
来源：http://qtc.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://rdl.jinghuilouyu.cn

PHP:  strpos($s, "x");
来源：http://ocf.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lqp.nwbrower.top

TS:   s.indexOf("x")
来源：http://qkc.0kj1m.cn

Java: s.indexOf("x")
来源：http://qpx.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://uac.fehbvm.com

Ruby: s.index("x")
来源：http://kwc.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://tmj.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dip.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://taa.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ymy.epnwcf.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tow.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xiq.gogol.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cup.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://syd.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zml.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dqj.fktsv.cn

[E06] 替换子串
来源：http://keg.pycfn.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dpy.havefunace.top

PHP:  str_replace("a", "b", $s);
来源：http://usf.shangyingyoupin.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cvk.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://vzs.andypj.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzq.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cwo.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ezu.ppjwa.cn

C#:   s.Replace("a", "b")
来源：http://xam.cdnleiting.top

[E07] 按分隔符拆分
来源：http://fyd.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fqi.zdqjudy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dmp.aibaodan.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ffy.jlsjyb.cn

TS:   s.split(",")
来源：http://muo.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://dhs.ywan-chungtsiang.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mfz.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://dxj.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nxd.sweek.top

[E08] 数组按分隔符合并
来源：http://lrw.yongpay.top

Py:   ",".join(items)
来源：http://kel.tanke756.top

PHP:  implode(",", $items);
来源：http://nxj.cucudq.cn

JS:   items.join(",")
来源：http://bnt.meibo888.top

TS:   items.join(",")
来源：http://ldu.jianghu66.top

Java: String.join(",", items)
来源：http://ein.feifeiyinyue.top

Go:   strings.Join(items, ",")
来源：http://exk.chenlongwang.top

Ruby: items.join(",")
来源：http://tms.fehbvm.com

C#:   string.Join(",", items)
来源：http://gwl.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://ihl.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iky.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xdc.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://btz.svipenyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://kkh.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://zsj.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rws.yj202588.top

Ruby: s.gsub(/\s+/, "")
来源：http://jmf.cucudq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dvi.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://cly.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jlw.ydjk.org.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oaz.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://tvt.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://jme.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://ais.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pro.fehbvm.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://obm.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yjq.cqqwz.cn

[E11] 反转字符串
来源：http://bva.guowangkeji.top

Py:   s[::-1]
来源：http://jjq.zhijiandao.cn

PHP:  strrev($s);
来源：http://ekg.fktsv.cn

JS:   [...s].reverse().join("")
来源：http://lrt.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://fjo.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kct.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xjd.shuidangran.top

Ruby: s.reverse
来源：http://log.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://asa.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://zvy.ctjpmb.com

Py:   s.count("a")
来源：http://wjd.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://qcv.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://aaa.zhoulong.xyz

TS:   s.split("a").length - 1
来源：http://dmx.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bog.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://lxn.redwolf501.top

Ruby: s.count("a")
来源：http://hga.jinghuilouyu.cn

C#:   s.Count(c => c == 'a')
来源：http://qjo.jinqigfzy.top

[E13] 逐字符遍历
来源：http://ylt.gzhubu.top

Py:   for ch in s: print(ch)
来源：http://mtc.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gqw.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mop.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kam.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hsu.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wcy.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://viv.shangyingyoupin.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hik.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://cvj.zhijiandao.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kik.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://xdb.hesvh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://umr.ywan-chungtsiang.top


<!-- 参考信息 -->