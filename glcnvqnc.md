代发 wailian999

TS:   arr.slice(1, 4);
来源：http://buh.redwolf501.top

Java: list.subList(1, 4);
来源：http://nsp.andypj.xyz

Go:   arr[1:4]
来源：http://iqd.zhengqikj.top

Ruby: arr[1, 3]
来源：http://hkr.zhaomingkeji.xyz

C#:   list.GetRange(1, 3);
来源：http://ash.zycfv.cn

[D08] 合并两个数组
来源：http://luo.gaohongyu789.top

Py:   a + b;  a.extend(b)
来源：http://huj.yj20258888.top

PHP:  array_merge($a, $b);
来源：http://jcs.shangyingyoupin.top

JS:   [...a, ...b];  a.concat(b);
来源：http://nhu.guowangkeji.top

TS:   [...a, ...b];
来源：http://xlx.aizwys.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://eeo.wangdashe.top

Go:   append(a, b...)
来源：http://tvk.fanxiaobao.xyz

Ruby: a + b;  a.concat(b)
来源：http://vzj.chenlongwang.top

C#:   a.Concat(b).ToList()
来源：http://apd.tarul.cn

[D09] 排序（升序）
来源：http://ocf.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://stf.hywenlv.cn

PHP:  sort($arr);
来源：http://jth.tarul.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://asy.cheryme.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://qey.haohaochexian.top

Java: Collections.sort(list);  list.sort(null);
来源：http://drk.iojbl.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://idz.cucudq.cn

Ruby: arr.sort
来源：http://vnm.yj20258.top

C#:   list.Sort();
来源：http://dgx.c1oappe.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://lle.guannengcc.top

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://qyj.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mdm.shanyushiyangtech.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rsx.yvedp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nfs.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aui.smart0.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://afu.aizwys.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://tym.hongshengwenyu.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bnf.shanyushiyangtech.top

[D11] 反转数组
来源：http://bus.vqdsnc.cn

Py:   arr[::-1];  arr.reverse()
来源：http://uyh.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://hfu.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://avy.yangfankeji.com

TS:   [...arr].reverse();
来源：http://oen.chenzaomai.com

Java: Collections.reverse(list);
来源：http://lsj.haohaochexian.top

Go:   slices.Reverse(arr)
来源：http://ztx.guannengcc.top

Ruby: arr.reverse
来源：http://mfd.aizwys.cn

C#:   list.Reverse();
来源：http://ezh.dashuyun.cn

[D12] 查找元素下标
来源：http://ckl.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://jcd.smart0.xyz

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://apq.hnqzz.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rlh.jiagoushi.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://epl.vehdjk.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hiq.smart0.xyz

Go:   slices.Index(arr, x)
来源：http://bts.hysaishi.cn

Ruby: arr.index(x)
来源：http://lok.tanke756.top

C#:   list.IndexOf(x);
来源：http://dym.andypj.xyz

[D13] 过滤（保留满足条件的）
来源：http://ovp.tian-w.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vde.ydzc1.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sbb.uphjek.com

JS:   arr.filter(x => x > 3)
来源：http://vyv.zhixingplan.top

TS:   arr.filter(x => x > 3)
来源：http://rqt.ppjwa.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gaq.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bfj.xuanzx.com

Ruby: arr.select { |x| x > 3 }
来源：http://cmy.ydjk.org.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://tsf.ywan-chungtsiang.top

[D14] 映射转换（每个元素变形）
来源：http://pkt.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jwv.wangdashe.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nfm.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://fpl.yangfankeji.com

TS:   arr.map(x => x * 2)
来源：http://czf.shanyushiyangtech.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://adk.sweek.top

Go:   // 手写循环
来源：http://izy.316326.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://nse.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://bts.ydzc1.top

[D15] 去重
来源：http://xak.jinghuilouyu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kck.yongpay.top

PHP:  array_unique($arr);
来源：http://jjd.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://wsu.shanyushiyangkeji.top

TS:   [...new Set(arr)]
来源：http://hrt.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vux.316326.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://lik.9152youxi.cn

Ruby: arr.uniq
来源：http://tig.sufxvd.cn

C#:   list.Distinct().ToList()
来源：http://ugz.chenzaomai.com

[D16] 求和与平均值
来源：http://viy.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iif.xinyue.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://djx.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgu.wangshuangyany.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lqy.yongpay.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jak.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://wac.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fvg.hongshengwenyu.top

C#:   list.Sum();  list.Average()
来源：http://cfy.daxiang520.top

[D17] 最大值与最小值
来源：http://jid.jqgfzy.top

Py:   max(arr);  min(arr)
来源：http://zox.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://inz.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ktb.yuanzhike.top

TS:   Math.max(...arr);
来源：http://cfw.jqgfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://utr.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ujb.zhijiandao.cn

Ruby: arr.max;  arr.min
来源：http://sbk.xylfe.cn

C#:   list.Max();  list.Min()
来源：http://brr.svipenyu.cn

[D18] 扁平化嵌套数组
来源：http://sqt.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ayz.havefunace.top

PHP:  array_merge(...$nested);
来源：http://dqf.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nkh.yj202588.top

TS:   nested.flat();
来源：http://kiu.zhiwuduotai.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iyh.xinyue.icu

Go:   // 手写双层循环
来源：http://zua.uphjek.com

Ruby: nested.flatten
来源：http://npt.sxryk.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sun.cdnleiting.top

[D19] 按字段分组
来源：http://jwo.yanxiufei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://smg.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvh.zhiwuduotai.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://boi.9152youxi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://iay.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xnb.yangfankeji.com

Go:   // 手写 map[string][]T
来源：http://pqu.fktsv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://tvo.shangyingyoupin.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://umd.jianghu66.top

[D20] 统计每个元素出现次数
来源：http://mgt.yanxiufei.cn

Py:   Counter(arr)
来源：http://bpr.jqgfzy.top

PHP:  array_count_values($arr);
来源：http://kbs.daria6918.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jai.svipenyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jzx.hcnkem.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wdz.ppjwa.cn

Go:   // 手写 map[T]int
来源：http://yfv.316326.xyz

Ruby: arr.tally
来源：http://peq.sysykeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lea.jianghu66.top

[D21] 判断是否包含某元素
来源：http://jnv.xuanzx.com

Py:   x in arr
来源：http://qty.zhoulong.xyz

PHP:  in_array($x, $arr, true);
来源：http://qaw.jyoumei.cn

JS:   arr.includes(x)
来源：http://ryj.quarkkingdee.top

TS:   arr.includes(x)
来源：http://vcf.snrcjt.cn

Java: list.contains(x)
来源：http://auj.hnqzz.top

Go:   slices.Contains(arr, x)
来源：http://xcj.jyoumei.cn

Ruby: arr.include?(x)
来源：http://abk.nanxinkj.top

C#:   list.Contains(x)
来源：http://kyg.yueranfly.top

[D22] 复制数组（避免共享引用）
来源：http://pah.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sqp.c1oappe.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://goy.xziqi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://drr.dianchejie.cn

TS:   [...arr];
来源：http://lct.aizwys.cn

Java: new ArrayList<>(list);
来源：http://nuk.xinyue.icu

Go:   copied := append([]int(nil), arr...)
来源：http://rjo.andypj.xyz

Ruby: arr.dup;  arr.clone
来源：http://isn.xuanzx.com

C#:   new List<int>(list);
来源：http://vhw.guannengcc.top

[D23] reduce 累积计算
来源：http://ebn.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mcr.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nbv.ctjpmb.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://okh.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fpa.jyoumei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://smo.guowangkeji.top

Go:   // 手写循环
来源：http://pil.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bgz.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ptb.xziqi.cn

[D24] 字典 / Map 基本操作
来源：http://gqv.sjlbkw.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mdq.nanxinkj.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yjq.cheryme.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cbe.epnwcf.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dmk.bjfxy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uhu.tanke756.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://aou.yueranfly.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pvz.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dwv.jinyuanbaomall.cn

[D25] Set 集合去重与交并差
来源：http://wmf.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lbv.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nlr.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://uso.shuidangran.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bqg.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://syj.shuidangran.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://aqo.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kvn.nanxuanxn.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hpy.sweek.top

[D26] 数组转字符串
来源：http://yyp.jinyuanbaomall.cn

Py:   ", ".join(map(str, arr))
来源：http://viq.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://mmw.chenlongwang.top

JS:   arr.join(", ")
来源：http://zik.kuanghao11.cn

TS:   arr.join(", ")
来源：http://dse.zhijiandao.cn

Java: String.join(", ", list)
来源：http://imh.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://bwq.hammf.cn

Ruby: arr.join(", ")
来源：http://dew.yongpay.top

C#:   string.Join(", ", list)
来源：http://evt.gaohongyu789.top

================================================================================
来源：http://cgv.hnxiangtu.top

E. 字符串处理
来源：http://jti.tanke756.top

================================================================================
来源：http://enk.tian-w.cn

[E01] 拼接字符串
来源：http://tne.hysaishi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://guy.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mtg.52xcode.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://yox.tanke756.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://byk.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aia.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://onk.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rqz.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lyq.gaohongyu789.top

[E02] 重复字符串
来源：http://acc.daria6918.cn

Py:   "ab" * 3
来源：http://jri.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://jsl.aizwys.cn

JS:   "ab".repeat(3)
来源：http://lwh.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://zie.yj202588.top

Java: "ab".repeat(3)
来源：http://fbt.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://uuw.havefunace.top

Ruby: "ab" * 3
来源：http://nzp.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dkz.pycfn.com

[E03] 截取子串
来源：http://gao.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sgy.zhengqikj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sme.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wjz.fengsongda.top

TS:   s.slice(1, 4)
来源：http://bsm.yangfankeji.com

Java: s.substring(1, 4)
来源：http://frc.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zpn.chenzaomai.com

Ruby: s[1, 3];  s[1..3]
来源：http://dpy.hnxiangtu.top

C#:   s.Substring(1, 3)
来源：http://ozu.guowangkeji.top

[E04] 查找子串位置
来源：http://jgp.aizwys.cn

Py:   s.find("x");  s.index("x")
来源：http://msy.gogol.net.cn

PHP:  strpos($s, "x");
来源：http://ghx.havefunace.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kea.0kj1m.cn

TS:   s.indexOf("x")
来源：http://vvt.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://spa.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://erc.sysykeji.top

Ruby: s.index("x")
来源：http://vcu.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://xyc.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rpv.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fni.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uun.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xlt.wangshuangyany.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vgy.c1oappe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xqx.zhiwuduotai.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvb.ivvv.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hjh.wangdashe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kyc.hnqzz.top

[E06] 替换子串
来源：http://hkl.birdmap.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dry.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://wjn.sxryk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xxm.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://dpp.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rqy.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jbj.yvedp.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dmd.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://rny.aibaodan.cn

[E07] 按分隔符拆分
来源：http://zev.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://doh.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hir.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lns.mhx1999.top

TS:   s.split(",")
来源：http://xyu.shangyingyoupin.top

Java: s.split(",");  s.split("\\s+")
来源：http://jhk.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://obh.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://wnc.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cgj.fzhhl.top

[E08] 数组按分隔符合并
来源：http://alc.smart0.xyz

Py:   ",".join(items)
来源：http://tpm.tanke756.top

PHP:  implode(",", $items);
来源：http://ort.gogol.net.cn

JS:   items.join(",")
来源：http://pwr.sysykeji.top

TS:   items.join(",")
来源：http://byo.9152youxi.cn

Java: String.join(",", items)
来源：http://tmu.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://xve.pengpengdd.cyou

Ruby: items.join(",")
来源：http://hlk.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://fnv.nanxuanxn.top

[E09] 去除所有空白字符
来源：http://oct.ivvv.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://boe.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sun.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://uzz.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://kvm.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://dcb.xziqi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://laq.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://riu.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nng.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://xqt.ywan-chungtsiang.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ptp.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kvy.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://kkv.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://ezg.jinqigfzy.top

Java: String.format("%03d", 7)
来源：http://nbm.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://ruy.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lsr.fanxiaobao.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yle.nanxinkj.top

[E11] 反转字符串
来源：http://rxg.jyoumei.cn

Py:   s[::-1]
来源：http://eej.zhoulong.xyz

PHP:  strrev($s);
来源：http://lbd.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://tsk.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://leb.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wqn.zhiwuduotai.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://myc.ydjk.org.cn

Ruby: s.reverse
来源：http://osx.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cek.redwolf501.top

[E12] 统计某字符出现次数
来源：http://hiz.hesvh.cn

Py:   s.count("a")
来源：http://igb.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://tsg.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://obe.tianlin.xyz

TS:   s.split("a").length - 1
来源：http://dpe.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ccz.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://esi.ppjwa.cn

Ruby: s.count("a")
来源：http://jow.sysykeji.top

C#:   s.Count(c => c == 'a')
来源：http://quy.yanxiufei.cn

[E13] 逐字符遍历
来源：http://sis.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://wnq.iojbl.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ecs.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tyq.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nqq.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yio.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://olw.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hxn.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vfh.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://nzp.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gud.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nnq.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sfo.nwbrower.top


<!-- 参考信息 -->