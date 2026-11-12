代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://spx.yanxiufei.cn

[D08] 合并两个数组
来源：http://gup.guannengcc.top

Py:   a + b;  a.extend(b)
来源：http://thu.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://bbm.tianlin.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://hdn.yj20258888.top

TS:   [...a, ...b];
来源：http://hbi.yuanzhike.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://fcx.xziqi.cn

Go:   append(a, b...)
来源：http://xgz.jinghuilouyu.cn

Ruby: a + b;  a.concat(b)
来源：http://vkm.zhengqikj.top

C#:   a.Concat(b).ToList()
来源：http://cpx.fktsv.cn

[D09] 排序（升序）
来源：http://zqs.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dah.kuanghao11.cn

PHP:  sort($arr);
来源：http://hql.daxiang520.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jer.birdmap.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://jlr.9152youxi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xen.kuanghao11.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qlc.yj202588.top

Ruby: arr.sort
来源：http://ycr.yangfankeji.com

C#:   list.Sort();
来源：http://pfa.fzhhl.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://uxb.cdnleiting.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pjy.fktsv.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nny.yonumen.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wmr.gzhubu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ezn.sysykeji.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://apr.sjlbkw.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wvr.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rrk.0kj1m.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wvl.zhiwuduotai.top

[D11] 反转数组
来源：http://cot.meibo888.top

Py:   arr[::-1];  arr.reverse()
来源：http://xpw.yuanzhike.top

PHP:  array_reverse($arr);
来源：http://fvd.gogol.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ytj.sysykeji.top

TS:   [...arr].reverse();
来源：http://qjh.chenzaomai.com

Java: Collections.reverse(list);
来源：http://zma.havefunace.top

Go:   slices.Reverse(arr)
来源：http://ids.fzhhl.top

Ruby: arr.reverse
来源：http://gbq.9152youxi.cn

C#:   list.Reverse();
来源：http://upu.xylfe.cn

[D12] 查找元素下标
来源：http://eaw.tian-w.cn

Py:   arr.index(x);  x in arr
来源：http://unu.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pxh.ywan-chungtsiang.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ztz.zhaomingkeji.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ixu.cucudq.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ezc.zhixingplan.top

Go:   slices.Index(arr, x)
来源：http://dab.yonumen.top

Ruby: arr.index(x)
来源：http://rbf.shanyushiyangkeji.top

C#:   list.IndexOf(x);
来源：http://bre.pengpengdd.cyou

[D13] 过滤（保留满足条件的）
来源：http://gyt.cashguo.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ran.tianlin.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://rax.cqqwz.cn

JS:   arr.filter(x => x > 3)
来源：http://san.sysykeji.top

TS:   arr.filter(x => x > 3)
来源：http://eas.zdqjudy.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dyd.ctjpmb.com

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nxk.zdbjq.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cqx.guowangkeji.top

C#:   list.Where(x => x > 3).ToList()
来源：http://ceu.yj20258888.top

[D14] 映射转换（每个元素变形）
来源：http://olb.jinghuilouyu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nhr.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aeu.yongpay.top

JS:   arr.map(x => x * 2)
来源：http://gpi.meibo888.top

TS:   arr.map(x => x * 2)
来源：http://cag.shangyingyoupin.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qqq.jiagoushi.top

Go:   // 手写循环
来源：http://qco.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://rjn.zycfv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yus.yj202588.top

[D15] 去重
来源：http://ops.zhongyouzk.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gdk.pycfn.com

PHP:  array_unique($arr);
来源：http://xoi.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://lbn.chenlongwang.top

TS:   [...new Set(arr)]
来源：http://ftm.zhixingplan.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://apy.cdnleiting.top

Go:   // 用 map[T]struct{} 手写
来源：http://uht.chenlongwang.top

Ruby: arr.uniq
来源：http://wtu.uphjek.com

C#:   list.Distinct().ToList()
来源：http://jvl.epnwcf.com

[D16] 求和与平均值
来源：http://azu.hysaishi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hxt.zhengqikj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hsj.snrcjt.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bet.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kod.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jvg.jlsjyb.cn

Go:   // 手写循环累加
来源：http://tkm.jianghu66.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rte.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://dwt.vqdsnc.cn

[D17] 最大值与最小值
来源：http://pko.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://hqe.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://thd.yueranfly.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://drp.yongpay.top

TS:   Math.max(...arr);
来源：http://daf.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wkn.iojbl.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://muf.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://dea.tarul.cn

C#:   list.Max();  list.Min()
来源：http://nhp.gotoacloud.top

[D18] 扁平化嵌套数组
来源：http://joo.hammf.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mzp.pycfn.com

PHP:  array_merge(...$nested);
来源：http://pdu.andypj.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sop.zhengqikj.top

TS:   nested.flat();
来源：http://syc.havefunace.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bhv.hesvh.cn

Go:   // 手写双层循环
来源：http://vqr.cdnleiting.top

Ruby: nested.flatten
来源：http://iwk.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zsd.zhoulong.xyz

[D19] 按字段分组
来源：http://wpn.hesvh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cdb.meibo888.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://llx.wangdashe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zxa.shuidangran.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cwh.xuetiantiany.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iyd.xingfuxueyuan.xyz

Go:   // 手写 map[string][]T
来源：http://ytm.sufxvd.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://icp.pengpengdd.cyou

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vhf.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://jmd.fanxiaobao.xyz

Py:   Counter(arr)
来源：http://gsu.wangdashe.top

PHP:  array_count_values($arr);
来源：http://uue.yuanzhike.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://asi.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ver.meibo888.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aio.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://mes.nwbrower.top

Ruby: arr.tally
来源：http://yki.gzhubu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://khl.daxiang520.top

[D21] 判断是否包含某元素
来源：http://ugt.chenjidiqi.icu

Py:   x in arr
来源：http://csj.fktsv.cn

PHP:  in_array($x, $arr, true);
来源：http://tdo.hywenlv.cn

JS:   arr.includes(x)
来源：http://pra.xziqi.cn

TS:   arr.includes(x)
来源：http://agy.hfpthk.cn

Java: list.contains(x)
来源：http://jqc.shangyingyoupin.top

Go:   slices.Contains(arr, x)
来源：http://xds.guannengcc.top

Ruby: arr.include?(x)
来源：http://ldz.chenlongwang.top

C#:   list.Contains(x)
来源：http://ntm.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://kpp.snrcjt.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ndq.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bkl.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qqj.hcnkem.com

TS:   [...arr];
来源：http://ooo.cucudq.cn

Java: new ArrayList<>(list);
来源：http://yol.hnxiangtu.top

Go:   copied := append([]int(nil), arr...)
来源：http://uuh.tarul.cn

Ruby: arr.dup;  arr.clone
来源：http://hwb.sjlbkw.cn

C#:   new List<int>(list);
来源：http://hzx.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://drx.tian-w.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wtg.havefunace.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yio.uphjek.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yde.tian-w.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://atj.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yws.tarul.cn

Go:   // 手写循环
来源：http://ktk.iojbl.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://izj.hysaishi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ynn.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://wdy.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ecz.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhb.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gkb.nanxuanxn.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lwk.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jhf.xinyue.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kbs.hywenlv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fgu.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rzt.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://cvt.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rin.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kkz.xuanzx.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rtt.bjfxy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yml.xziqi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hgx.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oua.redwolf501.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hhb.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oum.shangyingyoupin.top

[D26] 数组转字符串
来源：http://akb.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://eoa.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://fbs.hywenlv.cn

JS:   arr.join(", ")
来源：http://xgz.redwolf501.top

TS:   arr.join(", ")
来源：http://pmi.xinyue.icu

Java: String.join(", ", list)
来源：http://zju.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://yrl.ydzc1.top

Ruby: arr.join(", ")
来源：http://mhi.jiagoushi.top

C#:   string.Join(", ", list)
来源：http://mbp.bjfxy.top

================================================================================
来源：http://qum.xuanzx.com

E. 字符串处理
来源：http://psa.jinghuilouyu.cn

================================================================================
来源：http://ubo.shuidangran.top

[E01] 拼接字符串
来源：http://avt.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ukx.wangshuangyany.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wjm.gzhubu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ldk.zhiwuduotai.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://axv.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jgo.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fpl.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ryk.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yks.andypj.xyz

[E02] 重复字符串
来源：http://zqk.tarul.cn

Py:   "ab" * 3
来源：http://mwu.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://bms.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ptr.hesvh.cn

TS:   "ab".repeat(3)
来源：http://nzv.chenzaomai.com

Java: "ab".repeat(3)
来源：http://vos.shuidangran.top

Go:   strings.Repeat("ab", 3)
来源：http://ddv.zhongyouzk.top

Ruby: "ab" * 3
来源：http://qfl.pengpengdd.cyou

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gby.dashuyun.cn

[E03] 截取子串
来源：http://aap.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ppy.sweek.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qrp.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ked.xylfe.cn

TS:   s.slice(1, 4)
来源：http://iug.jinqigufen.top

Java: s.substring(1, 4)
来源：http://vhg.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jmt.snrcjt.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iwa.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://nms.yanxiufei.cn

[E04] 查找子串位置
来源：http://awa.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://vxe.nanxuanxn.top

PHP:  strpos($s, "x");
来源：http://xms.guowangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dsk.fzhhl.top

TS:   s.indexOf("x")
来源：http://ruv.yangfankeji.com

Java: s.indexOf("x")
来源：http://qts.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://gcg.yj20258888.top

Ruby: s.index("x")
来源：http://dfb.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://ytt.hongshengwenyu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rkm.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tkp.havefunace.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qsv.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mjp.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hbq.jiagoushi.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lig.yj20258888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kmr.gogol.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://grp.fanxiaobao.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://slc.jiagoushi.top

[E06] 替换子串
来源：http://lxl.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sjx.shanyushiyangtech.top

PHP:  str_replace("a", "b", $s);
来源：http://byz.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ein.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://bux.zhaomingkeji.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vak.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://exm.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lyy.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://mfd.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://yhc.epnwcf.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wzt.gzhubu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://iyf.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kry.snrcjt.cn

TS:   s.split(",")
来源：http://ruc.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bsc.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://voq.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://pop.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sys.cqqwz.cn

[E08] 数组按分隔符合并
来源：http://qxl.xuanzx.com

Py:   ",".join(items)
来源：http://mfl.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://afg.tarul.cn

JS:   items.join(",")
来源：http://sus.fengsongda.top

TS:   items.join(",")
来源：http://rng.bbcook.cn

Java: String.join(",", items)
来源：http://mzf.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://ern.wangdashe.top

Ruby: items.join(",")
来源：http://slj.zhixingplan.top

C#:   string.Join(",", items)
来源：http://nzx.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://juy.dashuyun.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ibn.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nka.guannengcc.top

JS:   s.replace(/\s+/g, "")
来源：http://xwn.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://zpx.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://gex.yj20258.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aoa.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gjb.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zbr.zdbjq.cn

[E10] 左侧补零 / 定长填充
来源：http://crz.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pdo.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nja.zhengqikj.top

JS:   "7".padStart(3, "0")
来源：http://xvm.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://kxy.aizwys.cn

Java: String.format("%03d", 7)
来源：http://nkq.fktsv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ftv.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nmu.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bdf.chenjidiqi.icu

[E11] 反转字符串
来源：http://iox.c1oappe.top

Py:   s[::-1]
来源：http://wxt.c1oappe.top

PHP:  strrev($s);
来源：http://ouq.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://wct.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://yeq.0kj1m.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qai.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hha.kuanghao11.cn

Ruby: s.reverse
来源：http://xvx.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xrx.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://nxk.9152youxi.cn

Py:   s.count("a")
来源：http://jak.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://rvo.sxryk.cn

JS:   s.split("a").length - 1
来源：http://moi.xuanzx.com

TS:   s.split("a").length - 1
来源：http://fap.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvq.0kj1m.cn

Go:   strings.Count(s, "a")
来源：http://teh.svipenyu.cn

Ruby: s.count("a")
来源：http://tsu.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://sjz.tarul.cn

[E13] 逐字符遍历
来源：http://cox.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://egm.hfpthk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://egw.ydzc1.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ibs.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xff.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oyk.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zxf.zhaomingkeji.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://shm.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dmg.yj20258888.top

[E14] URL 编码与 Base64
来源：http://okx.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vqa.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://oha.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rzr.ppjwa.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gzx.wangshuangyany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ivx.hammf.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nxb.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tgi.zhoulong.xyz


<!-- 参考信息 -->