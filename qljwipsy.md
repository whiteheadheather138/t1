代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://btw.cashguo.top

TS:   [...a, ...b];
来源：http://znt.zdbjq.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nzv.gogol.net.cn

Go:   append(a, b...)
来源：http://fjw.xinyue.icu

Ruby: a + b;  a.concat(b)
来源：http://hoo.hcnkem.com

C#:   a.Concat(b).ToList()
来源：http://crk.yj20258888.top

[D09] 排序（升序）
来源：http://jor.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://ijy.zycfv.cn

PHP:  sort($arr);
来源：http://jko.jyoumei.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://nrq.smart0.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://kvw.iojbl.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vum.birdmap.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yzg.gotoacloud.top

Ruby: arr.sort
来源：http://mof.0kj1m.cn

C#:   list.Sort();
来源：http://dvk.nanxuanxn.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://bow.quarkkingdee.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tps.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://noj.wangdashe.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nlf.svipenyu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://djm.jqgufenzy.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kdt.cheryme.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gcn.yangfankeji.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://arn.chenzaomai.com

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://vwb.yonumen.top

[D11] 反转数组
来源：http://zmn.wangdashe.top

Py:   arr[::-1];  arr.reverse()
来源：http://jgg.iojbl.cn

PHP:  array_reverse($arr);
来源：http://ycu.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qqz.tanke756.top

TS:   [...arr].reverse();
来源：http://iot.yfazqb.com

Java: Collections.reverse(list);
来源：http://inx.yongpay.top

Go:   slices.Reverse(arr)
来源：http://nnx.0kj1m.cn

Ruby: arr.reverse
来源：http://mpx.vqdsnc.cn

C#:   list.Reverse();
来源：http://lgh.iojbl.cn

[D12] 查找元素下标
来源：http://qfw.jinqigfzy.top

Py:   arr.index(x);  x in arr
来源：http://eef.kuanghao11.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://huw.chenlongwang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://isd.hnxiangtu.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fdc.mhx1999.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://nue.chenjidiqi.icu

Go:   slices.Index(arr, x)
来源：http://vmv.mhx1999.top

Ruby: arr.index(x)
来源：http://kuk.xingfuxueyuan.xyz

C#:   list.IndexOf(x);
来源：http://cgt.c1oappe.top

[D13] 过滤（保留满足条件的）
来源：http://vnc.ehwqpu.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hrg.jinyuanbaomall.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wmx.haohaochexian.top

JS:   arr.filter(x => x > 3)
来源：http://mjt.sweek.top

TS:   arr.filter(x => x > 3)
来源：http://apq.yuxming.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rxy.jinghuilouyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://tkc.hammf.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kwp.jinqigfzy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://gut.guowangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://nwe.smart0.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xev.smart0.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yvd.gzhubu.top

JS:   arr.map(x => x * 2)
来源：http://ckr.sweek.top

TS:   arr.map(x => x * 2)
来源：http://elm.bbcook.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nrm.fengsongda.top

Go:   // 手写循环
来源：http://inf.havefunace.top

Ruby: arr.map { |x| x * 2 }
来源：http://qka.yongpay.top

C#:   list.Select(x => x * 2).ToList()
来源：http://cxo.ctjpmb.com

[D15] 去重
来源：http://vhf.svipenyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cbp.yfazqb.com

PHP:  array_unique($arr);
来源：http://uqn.zycfv.cn

JS:   [...new Set(arr)]
来源：http://nsc.ehwqpu.com

TS:   [...new Set(arr)]
来源：http://vuz.wangdashe.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fgt.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pej.zhiwuduotai.top

Ruby: arr.uniq
来源：http://ooh.haohaochexian.top

C#:   list.Distinct().ToList()
来源：http://heg.uphjek.com

[D16] 求和与平均值
来源：http://skh.zhiwuduotai.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sdq.aizwys.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oxs.shzxlz.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jwt.52xcode.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kxa.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ijb.gogol.net.cn

Go:   // 手写循环累加
来源：http://rel.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zby.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://eqw.sysykeji.top

[D17] 最大值与最小值
来源：http://bdg.haohaochexian.top

Py:   max(arr);  min(arr)
来源：http://cty.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://htr.yj20258888.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ahq.hesvh.cn

TS:   Math.max(...arr);
来源：http://bms.smart0.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://hhk.redwolf501.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://shq.hesvh.cn

Ruby: arr.max;  arr.min
来源：http://ery.quarkkingdee.top

C#:   list.Max();  list.Min()
来源：http://jys.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://pyt.cashguo.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dur.jinqigfzy.top

PHP:  array_merge(...$nested);
来源：http://zjp.xinyue.icu

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ofo.jinyuanbaomall.cn

TS:   nested.flat();
来源：http://gqc.sjlbkw.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://nwh.xuetiantiany.cn

Go:   // 手写双层循环
来源：http://rhe.zhengqikj.top

Ruby: nested.flatten
来源：http://ono.shanyushiyangkeji.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://jvu.sysykeji.top

[D19] 按字段分组
来源：http://oug.tian-w.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nus.wangshuangyany.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nrq.kuanghao11.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ymv.yueranfly.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aug.shanyushiyangkeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kbg.shzxlz.cn

Go:   // 手写 map[string][]T
来源：http://azr.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://znd.sxryk.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ilu.pycfn.com

[D20] 统计每个元素出现次数
来源：http://gxm.chenlongwang.top

Py:   Counter(arr)
来源：http://cfm.shanyushiyangtech.top

PHP:  array_count_values($arr);
来源：http://jyy.ydzc1.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jch.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjx.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lzv.ctjpmb.com

Go:   // 手写 map[T]int
来源：http://ljo.daria6918.cn

Ruby: arr.tally
来源：http://ygn.pycfn.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nbg.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://vhd.hywenlv.cn

Py:   x in arr
来源：http://ttm.guowangkeji.top

PHP:  in_array($x, $arr, true);
来源：http://utp.bjfxy.top

JS:   arr.includes(x)
来源：http://upt.ydzc1.top

TS:   arr.includes(x)
来源：http://dxy.ctjpmb.com

Java: list.contains(x)
来源：http://cfk.guowangkeji.top

Go:   slices.Contains(arr, x)
来源：http://rnr.hesvh.cn

Ruby: arr.include?(x)
来源：http://fob.zhijiandao.cn

C#:   list.Contains(x)
来源：http://gyd.xinyue.icu

[D22] 复制数组（避免共享引用）
来源：http://vdt.yangfankeji.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ype.chenzaomai.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rav.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iep.yj202588.top

TS:   [...arr];
来源：http://zjz.bbcook.cn

Java: new ArrayList<>(list);
来源：http://ngw.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qhu.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://zpo.cqqwz.cn

C#:   new List<int>(list);
来源：http://vnp.hywenlv.cn

[D23] reduce 累积计算
来源：http://usu.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rme.shanyushiyangkeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://npm.sysykeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqk.hnqzz.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rfz.zhaomingkeji.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://bji.cashguo.top

Go:   // 手写循环
来源：http://wio.zhaomingkeji.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dhz.xziqi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xer.zdqjudy.top

[D24] 字典 / Map 基本操作
来源：http://vmr.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://niy.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hlu.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ocf.jyoumei.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oxu.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tpd.jlsjyb.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cxu.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lie.hfpthk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bhk.fktsv.cn

[D25] Set 集合去重与交并差
来源：http://hhn.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nem.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ftr.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xdw.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nvr.yueranfly.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://azo.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://luk.tianlin.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kdf.havefunace.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tpw.feifeiyinyue.top

[D26] 数组转字符串
来源：http://kuj.yonumen.top

Py:   ", ".join(map(str, arr))
来源：http://jjp.xylfe.cn

PHP:  implode(", ", $arr);
来源：http://xbo.haohaochexian.top

JS:   arr.join(", ")
来源：http://efv.jinqigfzy.top

TS:   arr.join(", ")
来源：http://joj.52xcode.cn

Java: String.join(", ", list)
来源：http://pgr.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://nvt.yj20258888.top

Ruby: arr.join(", ")
来源：http://zdy.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://ewv.yj202588.top

================================================================================
来源：http://ylj.guannengcc.top

E. 字符串处理
来源：http://drd.yuanzhike.top

================================================================================
来源：http://krf.xuetiantiany.cn

[E01] 拼接字符串
来源：http://aqt.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xor.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xjl.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnr.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xgb.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yby.ctjpmb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vst.hnqzz.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fnu.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://duz.tanke756.top

[E02] 重复字符串
来源：http://xly.birdmap.top

Py:   "ab" * 3
来源：http://exo.tanke756.top

PHP:  str_repeat("ab", 3);
来源：http://kbl.jyoumei.cn

JS:   "ab".repeat(3)
来源：http://acr.gzhubu.top

TS:   "ab".repeat(3)
来源：http://chu.gotoacloud.top

Java: "ab".repeat(3)
来源：http://loh.jinyuanbaomall.cn

Go:   strings.Repeat("ab", 3)
来源：http://gdv.yongpay.top

Ruby: "ab" * 3
来源：http://lvr.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nfz.xuetiantiany.cn

[E03] 截取子串
来源：http://tyt.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ajd.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hjb.hfpthk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wbw.bjfxy.top

TS:   s.slice(1, 4)
来源：http://wzl.c1oappe.top

Java: s.substring(1, 4)
来源：http://izj.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dgm.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://fjw.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://jam.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://lwj.sxryk.cn

Py:   s.find("x");  s.index("x")
来源：http://cgx.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://fpb.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://znr.meibo888.top

TS:   s.indexOf("x")
来源：http://sxe.bjfxy.top

Java: s.indexOf("x")
来源：http://uhw.svipenyu.cn

Go:   strings.Index(s, "x")
来源：http://nmv.tanke756.top

Ruby: s.index("x")
来源：http://brf.wangdashe.top

C#:   s.IndexOf("x")
来源：http://blm.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uzq.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uee.zhijiandao.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bzc.yangfankeji.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tgh.chenzaomai.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jhc.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rpq.0kj1m.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://izi.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://afm.yanxiufei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pxi.yj202588.top

[E06] 替换子串
来源：http://cwg.ctjpmb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nlf.bbcook.cn

PHP:  str_replace("a", "b", $s);
来源：http://anx.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nqk.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://bku.ybcxt.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://duj.hongshengwenyu.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ojq.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eyb.shanyushiyangtech.top

C#:   s.Replace("a", "b")
来源：http://yoj.xinyue.icu

[E07] 按分隔符拆分
来源：http://hkk.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eiw.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jas.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://prx.aizwys.cn

TS:   s.split(",")
来源：http://sdm.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jsb.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wiv.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://hpd.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hpb.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://lwo.hammf.cn

Py:   ",".join(items)
来源：http://qsb.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://qqo.gotoacloud.top

JS:   items.join(",")
来源：http://pos.ivvv.top

TS:   items.join(",")
来源：http://tsq.jyoumei.cn

Java: String.join(",", items)
来源：http://osp.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://bhr.yj20258.top

Ruby: items.join(",")
来源：http://odw.vehdjk.com

C#:   string.Join(",", items)
来源：http://ajc.zdbjq.cn

[E09] 去除所有空白字符
来源：http://xls.epnwcf.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jza.kuanghao11.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wci.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://xqd.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://zjg.gogol.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://wxc.52xcode.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yje.yuanzhike.top

Ruby: s.gsub(/\s+/, "")
来源：http://nbn.xuetiantiany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ksv.fengsongda.top

[E10] 左侧补零 / 定长填充
来源：http://rbq.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tby.svipenyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://esg.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://cdr.aizwys.cn

TS:   "7".padStart(3, "0")
来源：http://teb.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://qqf.nanxuanxn.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://uia.hfpthk.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gfa.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fgc.tanke756.top

[E11] 反转字符串
来源：http://ive.kuanghao11.cn

Py:   s[::-1]
来源：http://buf.ywan-chungtsiang.top

PHP:  strrev($s);
来源：http://tpm.chenzaomai.com

JS:   [...s].reverse().join("")
来源：http://uwo.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://tfc.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://pcs.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yxi.zdqjudy.top

Ruby: s.reverse
来源：http://amx.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://vuz.bjfxy.top

[E12] 统计某字符出现次数
来源：http://npo.jianghu66.top

Py:   s.count("a")
来源：http://bkv.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://sbz.andypj.xyz

JS:   s.split("a").length - 1
来源：http://pwf.52xcode.cn

TS:   s.split("a").length - 1
来源：http://jeu.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iwu.yj20258.top

Go:   strings.Count(s, "a")
来源：http://xph.sufxvd.cn

Ruby: s.count("a")
来源：http://pgo.chenjidiqi.icu

C#:   s.Count(c => c == 'a')
来源：http://pnb.yvedp.cn

[E13] 逐字符遍历
来源：http://ojh.vqdsnc.cn

Py:   for ch in s: print(ch)
来源：http://epa.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zss.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mam.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://alr.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nie.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hcg.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hlp.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mwh.yueranfly.top

[E14] URL 编码与 Base64
来源：http://rtk.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fms.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cni.jiagoushi.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vbw.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oae.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wti.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bfl.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dwq.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxp.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://ydl.yj202588.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ums.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jua.cashguo.top


<!-- 参考信息 -->