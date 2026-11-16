代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://noi.wangdashe.top

[D08] 合并两个数组
来源：http://xdy.zhongyouzk.top

Py:   a + b;  a.extend(b)
来源：http://bal.jinqigufen.top

PHP:  array_merge($a, $b);
来源：http://gkv.hcnkem.com

JS:   [...a, ...b];  a.concat(b);
来源：http://qwr.yfazqb.com

TS:   [...a, ...b];
来源：http://nbx.yvedp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mcl.gaohongyu789.top

Go:   append(a, b...)
来源：http://usx.tian-w.cn

Ruby: a + b;  a.concat(b)
来源：http://dwa.hammf.cn

C#:   a.Concat(b).ToList()
来源：http://kcl.yj20258888.top

[D09] 排序（升序）
来源：http://eko.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://gsj.jyoumei.cn

PHP:  sort($arr);
来源：http://gaa.wangdashe.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rjf.ctjpmb.com

TS:   [...arr].sort((x, y) => x - y);
来源：http://tug.nanxinkj.top

Java: Collections.sort(list);  list.sort(null);
来源：http://fav.tarul.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zbn.feifeiyinyue.top

Ruby: arr.sort
来源：http://pvq.svipenyu.cn

C#:   list.Sort();
来源：http://mpe.zhixingplan.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://vgm.ivvv.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vkj.andypj.xyz

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ovj.guannengcc.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gac.hywenlv.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nui.xylfe.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ycv.cdnleiting.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lti.vehdjk.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yjm.haohaochexian.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://afa.shanyushiyangtech.top

[D11] 反转数组
来源：http://daa.nwbrower.top

Py:   arr[::-1];  arr.reverse()
来源：http://kio.shangyingyoupin.top

PHP:  array_reverse($arr);
来源：http://cnd.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ceu.bjfxy.top

TS:   [...arr].reverse();
来源：http://mor.xuetiantiany.cn

Java: Collections.reverse(list);
来源：http://mqc.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://swz.zdqjudy.top

Ruby: arr.reverse
来源：http://rll.chenjidiqi.icu

C#:   list.Reverse();
来源：http://uhz.tanke756.top

[D12] 查找元素下标
来源：http://owh.ybcxt.top

Py:   arr.index(x);  x in arr
来源：http://gvr.tanke756.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dpy.yvedp.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hvl.xuetiantiany.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wrx.cqqwz.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://olq.dianchejie.cn

Go:   slices.Index(arr, x)
来源：http://wqv.ivvv.top

Ruby: arr.index(x)
来源：http://tjr.52xcode.cn

C#:   list.IndexOf(x);
来源：http://vqs.aibaodan.cn

[D13] 过滤（保留满足条件的）
来源：http://xif.xuanzx.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://suo.yuxming.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qjp.vqdsnc.cn

JS:   arr.filter(x => x > 3)
来源：http://eht.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://nto.wangshuangyany.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hno.birdmap.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bzw.zhoulong.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://ypa.c1oappe.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qet.hcnkem.com

[D14] 映射转换（每个元素变形）
来源：http://rfb.meibo888.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gvf.yueranfly.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qpa.jqgfzy.top

JS:   arr.map(x => x * 2)
来源：http://mjm.zdbjq.cn

TS:   arr.map(x => x * 2)
来源：http://vqb.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://egu.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://azg.zhengqikj.top

Ruby: arr.map { |x| x * 2 }
来源：http://ris.cashguo.top

C#:   list.Select(x => x * 2).ToList()
来源：http://szs.jinqigufen.top

[D15] 去重
来源：http://udj.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rsu.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://yqv.fengsongda.top

JS:   [...new Set(arr)]
来源：http://hyo.yuxming.cn

TS:   [...new Set(arr)]
来源：http://qka.ydzc1.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rae.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://uyt.jiagoushi.top

Ruby: arr.uniq
来源：http://dig.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://lum.shanyushiyangtech.top

[D16] 求和与平均值
来源：http://ies.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hyi.xylfe.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fhg.zhiwuduotai.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ytg.fengsongda.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xzf.pycfn.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yyr.andypj.xyz

Go:   // 手写循环累加
来源：http://cfg.pengpengdd.cyou

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tur.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://dkd.zhengqikj.top

[D17] 最大值与最小值
来源：http://gkf.yonumen.top

Py:   max(arr);  min(arr)
来源：http://neu.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://jor.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xym.xziqi.cn

TS:   Math.max(...arr);
来源：http://dnd.kuanghao11.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mch.hysaishi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nyn.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://sxj.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://caz.haohaochexian.top

[D18] 扁平化嵌套数组
来源：http://zmv.jqgfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cqa.c1oappe.top

PHP:  array_merge(...$nested);
来源：http://bsx.tian-w.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eft.bbcook.cn

TS:   nested.flat();
来源：http://pfl.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mox.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://nxh.yfazqb.com

Ruby: nested.flatten
来源：http://qgl.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://gbq.yuanzhike.top

[D19] 按字段分组
来源：http://zkl.tarul.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zuv.shanyushiyangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://war.yueranfly.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jbp.hywenlv.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://keb.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sbx.epnwcf.com

Go:   // 手写 map[string][]T
来源：http://shp.shangyingyoupin.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://bfo.xuetiantiany.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tpt.yonumen.top

[D20] 统计每个元素出现次数
来源：http://qxx.daxiang520.top

Py:   Counter(arr)
来源：http://zab.redwolf501.top

PHP:  array_count_values($arr);
来源：http://zkl.xuetiantiany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://skg.hywenlv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eqi.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://axs.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://gdb.cucudq.cn

Ruby: arr.tally
来源：http://haq.andypj.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ghy.bjfxy.top

[D21] 判断是否包含某元素
来源：http://als.0kj1m.cn

Py:   x in arr
来源：http://wjx.jqgufenzy.top

PHP:  in_array($x, $arr, true);
来源：http://qlz.ppjwa.cn

JS:   arr.includes(x)
来源：http://bvu.ctjpmb.com

TS:   arr.includes(x)
来源：http://mcc.hongshengwenyu.top

Java: list.contains(x)
来源：http://ugv.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://vqs.andypj.xyz

Ruby: arr.include?(x)
来源：http://ynb.shuidangran.top

C#:   list.Contains(x)
来源：http://nhp.gzhubu.top

[D22] 复制数组（避免共享引用）
来源：http://brj.fehbvm.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tyi.fzhhl.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yjb.xingfuxueyuan.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yly.smart0.xyz

TS:   [...arr];
来源：http://mqp.svipenyu.cn

Java: new ArrayList<>(list);
来源：http://aed.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://kmp.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://veg.52xcode.cn

C#:   new List<int>(list);
来源：http://mev.vehdjk.com

[D23] reduce 累积计算
来源：http://msk.epnwcf.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nhj.bbcook.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cxg.havefunace.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://myu.jinqigufen.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wrt.shanyushiyangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://dqv.xuanzx.com

Go:   // 手写循环
来源：http://iro.shanyushiyangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kid.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dul.yanxiufei.cn

[D24] 字典 / Map 基本操作
来源：http://iou.hongshengwenyu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ice.guowangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ejt.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://tzl.zycfv.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://icg.cucudq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ngu.ctjpmb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qyh.ybcxt.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cvv.zhiwuduotai.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dmd.zhoulong.xyz

[D25] Set 集合去重与交并差
来源：http://gab.hfpthk.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lfc.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zcg.ctjpmb.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xor.fehbvm.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vpc.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tkl.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xmy.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xvr.yangfankeji.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qvw.jqgfzy.top

[D26] 数组转字符串
来源：http://hre.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://foz.dashuyun.cn

PHP:  implode(", ", $arr);
来源：http://tov.hfpthk.cn

JS:   arr.join(", ")
来源：http://xjf.jqgfzy.top

TS:   arr.join(", ")
来源：http://xgz.ctjpmb.com

Java: String.join(", ", list)
来源：http://dxs.hongshengwenyu.top

Go:   strings.Join(strs, ", ")
来源：http://pbn.shangyingyoupin.top

Ruby: arr.join(", ")
来源：http://jwe.shuidangran.top

C#:   string.Join(", ", list)
来源：http://xco.mhx1999.top

================================================================================
来源：http://qvd.shanyushiyangtech.top

E. 字符串处理
来源：http://joo.smart0.xyz

================================================================================
来源：http://vyy.hywenlv.cn

[E01] 拼接字符串
来源：http://iju.jianghu66.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwb.zhixingplan.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wvd.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rph.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fxl.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rzi.gogol.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ped.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ymo.wangdashe.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eap.daria6918.cn

[E02] 重复字符串
来源：http://qqi.cqqwz.cn

Py:   "ab" * 3
来源：http://hzb.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://syh.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://ulm.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://jfe.cashguo.top

Java: "ab".repeat(3)
来源：http://vdd.zhijiandao.cn

Go:   strings.Repeat("ab", 3)
来源：http://hfm.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://ssc.tianlin.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zwc.nanxinkj.top

[E03] 截取子串
来源：http://ubh.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gzl.yongpay.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nbc.yfazqb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fvc.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://hmf.xuetiantiany.cn

Java: s.substring(1, 4)
来源：http://xtb.tianlin.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vhf.uphjek.com

Ruby: s[1, 3];  s[1..3]
来源：http://awr.guannengcc.top

C#:   s.Substring(1, 3)
来源：http://hqh.zhongyouzk.top

[E04] 查找子串位置
来源：http://vgx.zhijiandao.cn

Py:   s.find("x");  s.index("x")
来源：http://yfn.cucudq.cn

PHP:  strpos($s, "x");
来源：http://bxl.tian-w.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://red.jqgfzy.top

TS:   s.indexOf("x")
来源：http://jub.vqdsnc.cn

Java: s.indexOf("x")
来源：http://qqi.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://nal.sysykeji.top

Ruby: s.index("x")
来源：http://jwr.fanxiaobao.xyz

C#:   s.IndexOf("x")
来源：http://qyo.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qpd.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dbw.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://swq.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivv.tianlin.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://uoh.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wtx.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pme.yueranfly.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zml.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zzn.c1oappe.top

[E06] 替换子串
来源：http://luj.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mqa.zhixingplan.top

PHP:  str_replace("a", "b", $s);
来源：http://slz.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ldl.feifeiyinyue.top

TS:   s.replaceAll("a", "b")
来源：http://kei.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ifs.cqqwz.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uiz.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gij.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://tgm.tarul.cn

[E07] 按分隔符拆分
来源：http://eys.yfazqb.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kca.birdmap.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blb.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bba.dianchejie.cn

TS:   s.split(",")
来源：http://zer.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://ltf.sysykeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xxu.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://bjz.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kof.yueranfly.top

[E08] 数组按分隔符合并
来源：http://lhl.hnqzz.top

Py:   ",".join(items)
来源：http://dof.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://etr.52xcode.cn

JS:   items.join(",")
来源：http://gai.shuidangran.top

TS:   items.join(",")
来源：http://sge.fzhhl.top

Java: String.join(",", items)
来源：http://iml.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://tgu.guannengcc.top

Ruby: items.join(",")
来源：http://nvk.yj20258.top

C#:   string.Join(",", items)
来源：http://fuy.yj20258.top

[E09] 去除所有空白字符
来源：http://zpb.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sfc.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qzy.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://jew.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://tru.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://lwn.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://efa.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://ssf.guowangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jvu.gaohongyu789.top

[E10] 左侧补零 / 定长填充
来源：http://bli.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vwi.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gfz.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://dwk.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://nrh.cashguo.top

Java: String.format("%03d", 7)
来源：http://rzc.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://spg.haohaochexian.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sbf.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dqk.daxiang520.top

[E11] 反转字符串
来源：http://nic.haohaochexian.top

Py:   s[::-1]
来源：http://yye.tarul.cn

PHP:  strrev($s);
来源：http://fxl.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://ynl.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://dlc.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hpj.shanyushiyangtech.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cfa.bjfxy.top

Ruby: s.reverse
来源：http://xqb.haohaochexian.top

C#:   new string(s.Reverse().ToArray())
来源：http://suy.chenjidiqi.icu

[E12] 统计某字符出现次数
来源：http://gve.pengpengdd.cyou

Py:   s.count("a")
来源：http://zhc.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://lyw.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://paw.bjfxy.top

TS:   s.split("a").length - 1
来源：http://dkt.fzhhl.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://spk.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://aqu.hongshengwenyu.top

Ruby: s.count("a")
来源：http://arn.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://mkg.ppjwa.cn

[E13] 逐字符遍历
来源：http://sjm.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://nrx.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kfc.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sfo.cashguo.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aau.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xla.fengsongda.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bzq.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://hrj.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gcq.guannengcc.top

[E14] URL 编码与 Base64
来源：http://trk.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ato.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://cie.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jkn.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xgz.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vla.yonumen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jwy.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jcc.fengsongda.top


<!-- 参考信息 -->