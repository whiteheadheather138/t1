代发 wailian999

TS:   arr.slice(1, 4);
来源：http://lzy.cqqwz.cn

Java: list.subList(1, 4);
来源：http://odx.shangyingyoupin.top

Go:   arr[1:4]
来源：http://ecz.haohaochexian.top

Ruby: arr[1, 3]
来源：http://rhq.xinyue.icu

C#:   list.GetRange(1, 3);
来源：http://glv.wangshuangyany.cn

[D08] 合并两个数组
来源：http://mbi.zhixingplan.top

Py:   a + b;  a.extend(b)
来源：http://vkm.aizwys.cn

PHP:  array_merge($a, $b);
来源：http://tmz.xuanzx.com

JS:   [...a, ...b];  a.concat(b);
来源：http://wxx.meibo888.top

TS:   [...a, ...b];
来源：http://hza.ydjk.org.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wnn.gaohongyu789.top

Go:   append(a, b...)
来源：http://izd.snrcjt.cn

Ruby: a + b;  a.concat(b)
来源：http://ayw.chenjidiqi.icu

C#:   a.Concat(b).ToList()
来源：http://ogr.gogol.net.cn

[D09] 排序（升序）
来源：http://cie.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://dqr.hesvh.cn

PHP:  sort($arr);
来源：http://npx.sxryk.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cwj.ehwqpu.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://isl.ydzc1.top

Java: Collections.sort(list);  list.sort(null);
来源：http://tjw.hywenlv.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ccj.zhiwuduotai.top

Ruby: arr.sort
来源：http://pdk.bjfxy.top

C#:   list.Sort();
来源：http://veq.birdmap.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jxe.fanxiaobao.xyz

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://whp.mhx1999.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wzm.hesvh.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zte.xuanzx.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://toh.shangyingyoupin.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gyt.fzhhl.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://azt.xuanzx.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pxx.nwbrower.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qsa.mhx1999.top

[D11] 反转数组
来源：http://kjd.smart0.xyz

Py:   arr[::-1];  arr.reverse()
来源：http://qxd.mhx1999.top

PHP:  array_reverse($arr);
来源：http://dqs.zhoulong.xyz

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hvn.sjlbkw.cn

TS:   [...arr].reverse();
来源：http://pzd.gotoacloud.top

Java: Collections.reverse(list);
来源：http://yws.shzxlz.cn

Go:   slices.Reverse(arr)
来源：http://jbd.zhaomingkeji.xyz

Ruby: arr.reverse
来源：http://abq.gaohongyu789.top

C#:   list.Reverse();
来源：http://iiu.haohaochexian.top

[D12] 查找元素下标
来源：http://jpv.zhongyouzk.top

Py:   arr.index(x);  x in arr
来源：http://vgb.guannengcc.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://uiy.shangyingyoupin.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://woa.haohaochexian.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wnh.zhixingplan.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jdr.jianghu66.top

Go:   slices.Index(arr, x)
来源：http://opo.ppjwa.cn

Ruby: arr.index(x)
来源：http://dwt.meibo888.top

C#:   list.IndexOf(x);
来源：http://kqm.epnwcf.com

[D13] 过滤（保留满足条件的）
来源：http://gnm.yuxming.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ynl.nanxinkj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://any.shanyushiyangkeji.top

JS:   arr.filter(x => x > 3)
来源：http://bqd.quarkkingdee.top

TS:   arr.filter(x => x > 3)
来源：http://pjr.xuetiantiany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fgo.svipenyu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uqp.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cxr.daria6918.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hjh.gogol.net.cn

[D14] 映射转换（每个元素变形）
来源：http://pmw.svipenyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bla.fanxiaobao.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ghs.cashguo.top

JS:   arr.map(x => x * 2)
来源：http://gxr.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://sqb.fehbvm.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvd.yj202588.top

Go:   // 手写循环
来源：http://vin.yongpay.top

Ruby: arr.map { |x| x * 2 }
来源：http://new.ppjwa.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zxq.jqgufenzy.top

[D15] 去重
来源：http://xtm.zhaomingkeji.xyz

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dvu.zhengqikj.top

PHP:  array_unique($arr);
来源：http://brl.hnqzz.top

JS:   [...new Set(arr)]
来源：http://fni.xuetiantiany.cn

TS:   [...new Set(arr)]
来源：http://edw.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ptz.iojbl.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ffb.jianghu66.top

Ruby: arr.uniq
来源：http://bma.cucudq.cn

C#:   list.Distinct().ToList()
来源：http://orn.fzhhl.top

[D16] 求和与平均值
来源：http://jxc.xziqi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pas.yuanzhike.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jyr.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ygm.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zkh.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kub.meibo888.top

Go:   // 手写循环累加
来源：http://xaw.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nzm.jqgufenzy.top

C#:   list.Sum();  list.Average()
来源：http://vkt.nanxinkj.top

[D17] 最大值与最小值
来源：http://jfo.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://dgl.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://src.ehwqpu.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kvf.daxiang520.top

TS:   Math.max(...arr);
来源：http://ojq.havefunace.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ybo.daxiang520.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tna.cheryme.top

Ruby: arr.max;  arr.min
来源：http://fjk.ivvv.top

C#:   list.Max();  list.Min()
来源：http://mxy.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://szv.kuanghao11.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ebu.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://bhn.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cbr.xylfe.cn

TS:   nested.flat();
来源：http://yif.smart0.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pox.hesvh.cn

Go:   // 手写双层循环
来源：http://jgj.ppjwa.cn

Ruby: nested.flatten
来源：http://sry.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://pob.shanyushiyangtech.top

[D19] 按字段分组
来源：http://gdw.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ijg.aibaodan.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bmz.ydzc1.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lyz.hongshengwenyu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://khl.iojbl.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vgn.vehdjk.com

Go:   // 手写 map[string][]T
来源：http://ptg.zhengqikj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://pij.52xcode.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://beh.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://xxd.jqgufenzy.top

Py:   Counter(arr)
来源：http://nex.yvedp.cn

PHP:  array_count_values($arr);
来源：http://jma.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ksm.iojbl.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lru.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mtf.sweek.top

Go:   // 手写 map[T]int
来源：http://wch.haohaochexian.top

Ruby: arr.tally
来源：http://abi.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xbh.vehdjk.com

[D21] 判断是否包含某元素
来源：http://xit.daria6918.cn

Py:   x in arr
来源：http://ubx.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://rpl.tanke756.top

JS:   arr.includes(x)
来源：http://xxl.yueranfly.top

TS:   arr.includes(x)
来源：http://atq.hesvh.cn

Java: list.contains(x)
来源：http://oou.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://pjl.guannengcc.top

Ruby: arr.include?(x)
来源：http://xuh.jqgfzy.top

C#:   list.Contains(x)
来源：http://xmf.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://irr.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wrk.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fxr.fehbvm.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://foi.cashguo.top

TS:   [...arr];
来源：http://yze.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://hyi.bjfxy.top

Go:   copied := append([]int(nil), arr...)
来源：http://cwm.pengpengdd.cyou

Ruby: arr.dup;  arr.clone
来源：http://evl.jlsjyb.cn

C#:   new List<int>(list);
来源：http://old.mhx1999.top

[D23] reduce 累积计算
来源：http://lef.bjfxy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qme.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xex.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://muj.xuetiantiany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://glm.yj20258.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xly.pycfn.com

Go:   // 手写循环
来源：http://uuk.zhengqikj.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://von.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cbb.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://etp.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://veg.xinyue.icu

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lih.ybcxt.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pdm.fktsv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://brd.fzhhl.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eds.zdqjudy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nly.zhiwuduotai.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bla.guannengcc.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ewd.nwbrower.top

[D25] Set 集合去重与交并差
来源：http://yac.fzhhl.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://syp.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://glb.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pbq.guannengcc.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dby.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xtw.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgn.jianghu66.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hxa.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwd.bbcook.cn

[D26] 数组转字符串
来源：http://csd.sjlbkw.cn

Py:   ", ".join(map(str, arr))
来源：http://mfy.tianlin.xyz

PHP:  implode(", ", $arr);
来源：http://lxi.smart0.xyz

JS:   arr.join(", ")
来源：http://jay.cqqwz.cn

TS:   arr.join(", ")
来源：http://uar.chenlongwang.top

Java: String.join(", ", list)
来源：http://yfb.cheryme.top

Go:   strings.Join(strs, ", ")
来源：http://mfm.epnwcf.com

Ruby: arr.join(", ")
来源：http://ikn.fktsv.cn

C#:   string.Join(", ", list)
来源：http://mki.9152youxi.cn

================================================================================
来源：http://cru.vehdjk.com

E. 字符串处理
来源：http://aeh.52xcode.cn

================================================================================
来源：http://mza.daxiang520.top

[E01] 拼接字符串
来源：http://nso.ywan-chungtsiang.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yod.hesvh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://heo.iojbl.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jkq.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://npj.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzt.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://azz.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ist.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rzj.xinyue.icu

[E02] 重复字符串
来源：http://lvn.gogol.net.cn

Py:   "ab" * 3
来源：http://ofc.guannengcc.top

PHP:  str_repeat("ab", 3);
来源：http://yjo.ywan-chungtsiang.top

JS:   "ab".repeat(3)
来源：http://osc.jqgufenzy.top

TS:   "ab".repeat(3)
来源：http://dau.haohaochexian.top

Java: "ab".repeat(3)
来源：http://tcs.yj202588.top

Go:   strings.Repeat("ab", 3)
来源：http://gxb.jinqigufen.top

Ruby: "ab" * 3
来源：http://htg.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tfe.sjlbkw.cn

[E03] 截取子串
来源：http://jls.zhiwuduotai.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dio.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://czj.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://htz.pycfn.com

TS:   s.slice(1, 4)
来源：http://wom.nwbrower.top

Java: s.substring(1, 4)
来源：http://zoa.redwolf501.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wqp.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://fxe.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://fwm.9152youxi.cn

[E04] 查找子串位置
来源：http://wyb.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://yut.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://unw.jyoumei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wlm.xinyue.icu

TS:   s.indexOf("x")
来源：http://tmp.bbcook.cn

Java: s.indexOf("x")
来源：http://wnn.fzhhl.top

Go:   strings.Index(s, "x")
来源：http://ihr.316326.xyz

Ruby: s.index("x")
来源：http://qxd.ehwqpu.com

C#:   s.IndexOf("x")
来源：http://qgg.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yxw.hnxiangtu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hyu.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sbp.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ctr.xinyue.icu

TS:   s.includes("x");  s.startsWith("a")
来源：http://rfa.316326.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iiz.jqgfzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cgq.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dgc.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vlj.wangdashe.top

[E06] 替换子串
来源：http://rfm.sjlbkw.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cnq.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://oea.jianghu66.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jcd.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://ids.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://igw.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yfi.fanxiaobao.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bmo.guannengcc.top

C#:   s.Replace("a", "b")
来源：http://wyi.xylfe.cn

[E07] 按分隔符拆分
来源：http://cgm.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yrv.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://inw.yfazqb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hoj.9152youxi.cn

TS:   s.split(",")
来源：http://wwm.jinyuanbaomall.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bdt.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ywz.ivvv.top

Ruby: s.split(",");  s.split
来源：http://iap.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dpv.tarul.cn

[E08] 数组按分隔符合并
来源：http://hvg.tianlin.xyz

Py:   ",".join(items)
来源：http://tfv.sufxvd.cn

PHP:  implode(",", $items);
来源：http://moc.andypj.xyz

JS:   items.join(",")
来源：http://lzn.daria6918.cn

TS:   items.join(",")
来源：http://dms.nanxuanxn.top

Java: String.join(",", items)
来源：http://gag.uphjek.com

Go:   strings.Join(items, ",")
来源：http://hqc.cheryme.top

Ruby: items.join(",")
来源：http://bvn.jqgufenzy.top

C#:   string.Join(",", items)
来源：http://kep.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://ahc.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nyf.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cqx.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://oaq.fehbvm.com

TS:   s.replace(/\s+/g, "")
来源：http://ssa.ctjpmb.com

Java: s.replaceAll("\\s+", "")
来源：http://mnb.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://igo.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lct.xuanzx.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tis.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://ieq.316326.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dkl.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ivf.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://bti.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://han.tian-w.cn

Java: String.format("%03d", 7)
来源：http://kyb.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://kaz.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xsx.ydzc1.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zcb.gaohongyu789.top

[E11] 反转字符串
来源：http://zlo.hfpthk.cn

Py:   s[::-1]
来源：http://ymz.fzhhl.top

PHP:  strrev($s);
来源：http://jys.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://rpm.zhixingplan.top

TS:   [...s].reverse().join("")
来源：http://fow.xuanzx.com

Java: new StringBuilder(s).reverse().toString()
来源：http://exv.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pci.quarkkingdee.top

Ruby: s.reverse
来源：http://oec.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tib.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://ckd.9152youxi.cn

Py:   s.count("a")
来源：http://uob.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://ziu.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://ogy.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://pmc.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yrf.yonumen.top

Go:   strings.Count(s, "a")
来源：http://fcq.yongpay.top

Ruby: s.count("a")
来源：http://zss.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://cfe.haohaochexian.top

[E13] 逐字符遍历
来源：http://iyy.jqgufenzy.top

Py:   for ch in s: print(ch)
来源：http://gwh.daria6918.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xwo.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wtd.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://acn.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kpf.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://knb.zhongyouzk.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fba.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eug.smart0.xyz

[E14] URL 编码与 Base64
来源：http://phb.sysykeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xax.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://osa.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ptq.jinghuilouyu.cn


<!-- 参考信息 -->