代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://pji.yvedp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://azn.c1oappe.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://jxf.fanxiaobao.xyz

[D06] 数组长度
来源：http://ctv.ydjk.org.cn

Py:   len(arr)
来源：http://zor.cucudq.cn

PHP:  count($arr);
来源：http://tyj.fktsv.cn

JS:   arr.length
来源：http://uzw.jlsjyb.cn

TS:   arr.length
来源：http://uzf.9152youxi.cn

Java: list.size();
来源：http://kac.hcnkem.com

Go:   len(arr)
来源：http://vuy.dianchejie.cn

Ruby: arr.length; arr.size
来源：http://irn.daxiang520.top

C#:   list.Count;
来源：http://upb.xylfe.cn

[D07] 切片 / 取子数组
来源：http://qki.bbcook.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zhm.hammf.cn

PHP:  array_slice($arr, 1, 3);
来源：http://guv.fanxiaobao.xyz

JS:   arr.slice(1, 4);
来源：http://lnj.zhijiandao.cn

TS:   arr.slice(1, 4);
来源：http://chb.daxiang520.top

Java: list.subList(1, 4);
来源：http://ioh.yongpay.top

Go:   arr[1:4]
来源：http://wkt.guannengcc.top

Ruby: arr[1, 3]
来源：http://ytk.jianghu66.top

C#:   list.GetRange(1, 3);
来源：http://hsz.daxiang520.top

[D08] 合并两个数组
来源：http://rad.guowangkeji.top

Py:   a + b;  a.extend(b)
来源：http://oup.yj20258.top

PHP:  array_merge($a, $b);
来源：http://ecz.316326.xyz

JS:   [...a, ...b];  a.concat(b);
来源：http://jgj.shanyushiyangtech.top

TS:   [...a, ...b];
来源：http://hre.ywan-chungtsiang.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xsc.aizwys.cn

Go:   append(a, b...)
来源：http://gpv.fktsv.cn

Ruby: a + b;  a.concat(b)
来源：http://lux.zycfv.cn

C#:   a.Concat(b).ToList()
来源：http://sth.zhongyouzk.top

[D09] 排序（升序）
来源：http://tqz.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://fvk.ehwqpu.com

PHP:  sort($arr);
来源：http://vmw.wangshuangyany.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ybx.vqdsnc.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ucf.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://hbm.xinyue.icu

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sjw.jlsjyb.cn

Ruby: arr.sort
来源：http://wpe.jyoumei.cn

C#:   list.Sort();
来源：http://aor.tianlin.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://umc.vehdjk.com

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://frr.ydzc1.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dau.guowangkeji.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cff.0kj1m.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ush.fehbvm.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://trz.dashuyun.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xxn.nanxinkj.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lcf.mhx1999.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fhh.feifeiyinyue.top

[D11] 反转数组
来源：http://qgq.yongpay.top

Py:   arr[::-1];  arr.reverse()
来源：http://xkk.52xcode.cn

PHP:  array_reverse($arr);
来源：http://wil.dianchejie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ajs.hesvh.cn

TS:   [...arr].reverse();
来源：http://axd.gogol.net.cn

Java: Collections.reverse(list);
来源：http://jhk.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://yow.cdnleiting.top

Ruby: arr.reverse
来源：http://exn.xuanzx.com

C#:   list.Reverse();
来源：http://qzv.fanxiaobao.xyz

[D12] 查找元素下标
来源：http://bat.pycfn.com

Py:   arr.index(x);  x in arr
来源：http://phd.yueranfly.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iwi.zhijiandao.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mkh.shzxlz.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yfp.jianghu66.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zra.bjfxy.top

Go:   slices.Index(arr, x)
来源：http://vdd.ydjk.org.cn

Ruby: arr.index(x)
来源：http://imv.cqqwz.cn

C#:   list.IndexOf(x);
来源：http://ayf.jinyuanbaomall.cn

[D13] 过滤（保留满足条件的）
来源：http://rkn.fehbvm.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rzo.jqgufenzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zso.sysykeji.top

JS:   arr.filter(x => x > 3)
来源：http://qdv.daria6918.cn

TS:   arr.filter(x => x > 3)
来源：http://osu.yvedp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ilz.tanke756.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iqv.cqqwz.cn

Ruby: arr.select { |x| x > 3 }
来源：http://std.chenzaomai.com

C#:   list.Where(x => x > 3).ToList()
来源：http://ykc.jianghu66.top

[D14] 映射转换（每个元素变形）
来源：http://feh.quarkkingdee.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cux.uphjek.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pdb.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://zht.fehbvm.com

TS:   arr.map(x => x * 2)
来源：http://kjn.gaohongyu789.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://myu.meibo888.top

Go:   // 手写循环
来源：http://yrw.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rxy.guannengcc.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vfy.316326.xyz

[D15] 去重
来源：http://ren.sufxvd.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ycg.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://ihf.pycfn.com

JS:   [...new Set(arr)]
来源：http://upx.sweek.top

TS:   [...new Set(arr)]
来源：http://oxw.hysaishi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qct.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://pyq.nanxuanxn.top

Ruby: arr.uniq
来源：http://rlf.hcnkem.com

C#:   list.Distinct().ToList()
来源：http://mmk.ctjpmb.com

[D16] 求和与平均值
来源：http://hlk.nanxinkj.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ijr.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://pvw.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://nzk.yanxiufei.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gor.cheryme.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://smi.shanyushiyangtech.top

Go:   // 手写循环累加
来源：http://ydz.hnxiangtu.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uqu.chenzaomai.com

C#:   list.Sum();  list.Average()
来源：http://lye.cdnleiting.top

[D17] 最大值与最小值
来源：http://xyd.c1oappe.top

Py:   max(arr);  min(arr)
来源：http://ist.zhongyouzk.top

PHP:  max($arr);  min($arr);
来源：http://rtw.xuetiantiany.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rri.zdqjudy.top

TS:   Math.max(...arr);
来源：http://fdv.wangshuangyany.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://slg.xziqi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wrn.daxiang520.top

Ruby: arr.max;  arr.min
来源：http://wvh.ybcxt.top

C#:   list.Max();  list.Min()
来源：http://ygj.jqgufenzy.top

[D18] 扁平化嵌套数组
来源：http://kls.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fis.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://rvv.yangfankeji.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gkf.cashguo.top

TS:   nested.flat();
来源：http://lei.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mkc.chenjidiqi.icu

Go:   // 手写双层循环
来源：http://stp.ivvv.top

Ruby: nested.flatten
来源：http://jsw.yvedp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sva.epnwcf.com

[D19] 按字段分组
来源：http://hha.fengsongda.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kzx.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://aqy.zycfv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqr.meibo888.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vsc.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ejc.pycfn.com

Go:   // 手写 map[string][]T
来源：http://brs.quarkkingdee.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zty.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ytr.tanke756.top

[D20] 统计每个元素出现次数
来源：http://mbl.ybcxt.top

Py:   Counter(arr)
来源：http://gss.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://afw.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zrr.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mbs.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jxe.tanke756.top

Go:   // 手写 map[T]int
来源：http://bis.c1oappe.top

Ruby: arr.tally
来源：http://trv.tarul.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aye.wangdashe.top

[D21] 判断是否包含某元素
来源：http://sjn.jinghuilouyu.cn

Py:   x in arr
来源：http://yxa.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://vpr.gzhubu.top

JS:   arr.includes(x)
来源：http://ssz.zdqjudy.top

TS:   arr.includes(x)
来源：http://bli.jlsjyb.cn

Java: list.contains(x)
来源：http://sut.ctjpmb.com

Go:   slices.Contains(arr, x)
来源：http://tbl.fzhhl.top

Ruby: arr.include?(x)
来源：http://rgh.sufxvd.cn

C#:   list.Contains(x)
来源：http://pyy.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://uow.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lzs.bbcook.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://klz.jinghuilouyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zxh.zhongyouzk.top

TS:   [...arr];
来源：http://cuo.tarul.cn

Java: new ArrayList<>(list);
来源：http://kbc.uphjek.com

Go:   copied := append([]int(nil), arr...)
来源：http://jlc.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://blu.nanxinkj.top

C#:   new List<int>(list);
来源：http://ocg.aizwys.cn

[D23] reduce 累积计算
来源：http://ano.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zec.xinyue.icu

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://orc.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dar.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qbu.fanxiaobao.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://kgv.yj20258.top

Go:   // 手写循环
来源：http://rfx.nwbrower.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gsr.yj202588.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bzk.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://dbj.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blf.yvedp.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uvz.xinyue.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://aep.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nvr.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dfr.yj20258888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xlx.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mct.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ejh.jinqigufen.top

[D25] Set 集合去重与交并差
来源：http://uwk.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tpw.dianchejie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://djv.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lqh.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cvp.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zys.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wjm.zhixingplan.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fre.andypj.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mvl.pycfn.com

[D26] 数组转字符串
来源：http://eqa.cdnleiting.top

Py:   ", ".join(map(str, arr))
来源：http://icc.hywenlv.cn

PHP:  implode(", ", $arr);
来源：http://gep.yuxming.cn

JS:   arr.join(", ")
来源：http://iue.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://juk.fktsv.cn

Java: String.join(", ", list)
来源：http://kyu.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://lgf.tarul.cn

Ruby: arr.join(", ")
来源：http://wgy.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://aoo.ydjk.org.cn

================================================================================
来源：http://jsn.cashguo.top

E. 字符串处理
来源：http://hzj.xylfe.cn

================================================================================
来源：http://fft.chenlongwang.top

[E01] 拼接字符串
来源：http://chu.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gdv.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rpk.cashguo.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vhx.ivvv.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uyv.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://orw.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lrt.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ncy.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xme.yangfankeji.com

[E02] 重复字符串
来源：http://vif.yj202588.top

Py:   "ab" * 3
来源：http://ine.yueranfly.top

PHP:  str_repeat("ab", 3);
来源：http://rvr.guannengcc.top

JS:   "ab".repeat(3)
来源：http://jgb.bjfxy.top

TS:   "ab".repeat(3)
来源：http://zav.cqqwz.cn

Java: "ab".repeat(3)
来源：http://guz.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://wvi.jqgufenzy.top

Ruby: "ab" * 3
来源：http://dzu.wangshuangyany.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tfw.ppjwa.cn

[E03] 截取子串
来源：http://kil.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nyz.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zrv.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://prp.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://qyr.9152youxi.cn

Java: s.substring(1, 4)
来源：http://eeo.cashguo.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bvn.hfpthk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ntj.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://xin.ydzc1.top

[E04] 查找子串位置
来源：http://aqr.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://kxb.fengsongda.top

PHP:  strpos($s, "x");
来源：http://aou.nanxuanxn.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qcm.ctjpmb.com

TS:   s.indexOf("x")
来源：http://jey.hcnkem.com

Java: s.indexOf("x")
来源：http://add.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://ooc.zdqjudy.top

Ruby: s.index("x")
来源：http://mic.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://ryu.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://uze.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dsa.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tix.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://idv.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://feb.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ahj.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://alf.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tsn.yueranfly.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bdv.xziqi.cn

[E06] 替换子串
来源：http://brh.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://svs.yvedp.cn

PHP:  str_replace("a", "b", $s);
来源：http://yxb.tianlin.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://srt.shuidangran.top

TS:   s.replaceAll("a", "b")
来源：http://amv.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sjh.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zdb.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ibh.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://flo.gogol.net.cn

[E07] 按分隔符拆分
来源：http://liy.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gyd.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bgi.meibo888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mzb.yfazqb.com

TS:   s.split(",")
来源：http://sqg.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://jqr.aibaodan.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gpr.yj20258.top

Ruby: s.split(",");  s.split
来源：http://bhd.birdmap.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ulr.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://uzi.gogol.net.cn

Py:   ",".join(items)
来源：http://euq.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://bbk.hcnkem.com

JS:   items.join(",")
来源：http://zcn.daria6918.cn

TS:   items.join(",")
来源：http://rtb.sxryk.cn

Java: String.join(",", items)
来源：http://afa.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://oag.epnwcf.com

Ruby: items.join(",")
来源：http://gqu.hysaishi.cn

C#:   string.Join(",", items)
来源：http://uju.chenzaomai.com

[E09] 去除所有空白字符
来源：http://upr.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://afi.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xpz.yvedp.cn

JS:   s.replace(/\s+/g, "")
来源：http://hhe.guannengcc.top

TS:   s.replace(/\s+/g, "")
来源：http://dhf.jqgfzy.top

Java: s.replaceAll("\\s+", "")
来源：http://zqf.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://diw.xingfuxueyuan.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://fru.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://knq.xuanzx.com

[E10] 左侧补零 / 定长填充
来源：http://mbn.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gpk.jinyuanbaomall.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fxw.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://jkv.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://pfw.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://gge.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://erv.cheryme.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hcm.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kxf.gaohongyu789.top

[E11] 反转字符串
来源：http://gow.fehbvm.com

Py:   s[::-1]
来源：http://buy.hongshengwenyu.top

PHP:  strrev($s);
来源：http://vrz.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://wyf.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://kms.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zmj.yj20258888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uqs.tanke756.top

Ruby: s.reverse
来源：http://nvg.ywan-chungtsiang.top

C#:   new string(s.Reverse().ToArray())
来源：http://abf.ctjpmb.com

[E12] 统计某字符出现次数
来源：http://wcj.sysykeji.top

Py:   s.count("a")
来源：http://ukx.jinqigfzy.top

PHP:  substr_count($s, "a");
来源：http://qoa.sweek.top

JS:   s.split("a").length - 1
来源：http://waa.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://hod.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsj.yvedp.cn


<!-- 参考信息 -->