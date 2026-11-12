代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://ivp.epnwcf.com

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://eke.cheryme.top

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wje.bjfxy.top

[D06] 数组长度
来源：http://oth.316326.xyz

Py:   len(arr)
来源：http://yvq.jyoumei.cn

PHP:  count($arr);
来源：http://bct.shangyingyoupin.top

JS:   arr.length
来源：http://zpm.feifeiyinyue.top

TS:   arr.length
来源：http://lck.ehwqpu.com

Java: list.size();
来源：http://nyq.iojbl.cn

Go:   len(arr)
来源：http://ygl.andypj.xyz

Ruby: arr.length; arr.size
来源：http://sut.jianghu66.top

C#:   list.Count;
来源：http://dqv.c1oappe.top

[D07] 切片 / 取子数组
来源：http://iin.zhaomingkeji.xyz

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wqr.yfazqb.com

PHP:  array_slice($arr, 1, 3);
来源：http://wdx.hnqzz.top

JS:   arr.slice(1, 4);
来源：http://ekx.iojbl.cn

TS:   arr.slice(1, 4);
来源：http://uol.chenzaomai.com

Java: list.subList(1, 4);
来源：http://elr.tanke756.top

Go:   arr[1:4]
来源：http://dwu.wangshuangyany.cn

Ruby: arr[1, 3]
来源：http://rwo.52xcode.cn

C#:   list.GetRange(1, 3);
来源：http://ebk.zhijiandao.cn

[D08] 合并两个数组
来源：http://lwz.jqgfzy.top

Py:   a + b;  a.extend(b)
来源：http://gwt.gaohongyu789.top

PHP:  array_merge($a, $b);
来源：http://yoo.ehwqpu.com

JS:   [...a, ...b];  a.concat(b);
来源：http://juy.haohaochexian.top

TS:   [...a, ...b];
来源：http://qjv.shanyushiyangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gme.hongshengwenyu.top

Go:   append(a, b...)
来源：http://lrc.mhx1999.top

Ruby: a + b;  a.concat(b)
来源：http://twi.yonumen.top

C#:   a.Concat(b).ToList()
来源：http://ihg.ppjwa.cn

[D09] 排序（升序）
来源：http://vfj.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ose.wangdashe.top

PHP:  sort($arr);
来源：http://bkn.hongshengwenyu.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vrs.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rfl.zdbjq.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://php.fehbvm.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iue.xuetiantiany.cn

Ruby: arr.sort
来源：http://lkt.andypj.xyz

C#:   list.Sort();
来源：http://zfh.zdqjudy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://epj.kuanghao11.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://oxa.ywan-chungtsiang.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qll.shuidangran.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://tgd.ppjwa.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ztl.yvedp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ygj.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://los.zhoulong.xyz

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pfy.sweek.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://qyv.zycfv.cn

[D11] 反转数组
来源：http://fnl.aizwys.cn

Py:   arr[::-1];  arr.reverse()
来源：http://tsf.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://fhg.svipenyu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ykg.meibo888.top

TS:   [...arr].reverse();
来源：http://wso.sysykeji.top

Java: Collections.reverse(list);
来源：http://rtz.vqdsnc.cn

Go:   slices.Reverse(arr)
来源：http://bwh.vqdsnc.cn

Ruby: arr.reverse
来源：http://rkp.yj20258888.top

C#:   list.Reverse();
来源：http://zky.bbcook.cn

[D12] 查找元素下标
来源：http://vva.zhixingplan.top

Py:   arr.index(x);  x in arr
来源：http://qvq.pycfn.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wtv.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cwz.yongpay.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qle.hnxiangtu.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dkq.yanxiufei.cn

Go:   slices.Index(arr, x)
来源：http://acg.birdmap.top

Ruby: arr.index(x)
来源：http://cxt.shanyushiyangtech.top

C#:   list.IndexOf(x);
来源：http://rgr.ydjk.org.cn

[D13] 过滤（保留满足条件的）
来源：http://nie.hongshengwenyu.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hbx.jinqigfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gvh.yvedp.cn

JS:   arr.filter(x => x > 3)
来源：http://aas.nwbrower.top

TS:   arr.filter(x => x > 3)
来源：http://zwh.sjlbkw.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ckg.chenlongwang.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yci.yuxming.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wcq.pycfn.com

C#:   list.Where(x => x > 3).ToList()
来源：http://rsh.bjfxy.top

[D14] 映射转换（每个元素变形）
来源：http://igg.hfpthk.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uny.zhaomingkeji.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://djj.ivvv.top

JS:   arr.map(x => x * 2)
来源：http://sgb.quarkkingdee.top

TS:   arr.map(x => x * 2)
来源：http://tyw.jinghuilouyu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qfi.yueranfly.top

Go:   // 手写循环
来源：http://rkg.zhixingplan.top

Ruby: arr.map { |x| x * 2 }
来源：http://zsh.shzxlz.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://skn.9152youxi.cn

[D15] 去重
来源：http://xfo.hongshengwenyu.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cun.tarul.cn

PHP:  array_unique($arr);
来源：http://tgx.hesvh.cn

JS:   [...new Set(arr)]
来源：http://txa.vehdjk.com

TS:   [...new Set(arr)]
来源：http://ehy.yanxiufei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ovl.cheryme.top

Go:   // 用 map[T]struct{} 手写
来源：http://otw.yongpay.top

Ruby: arr.uniq
来源：http://loq.yj20258.top

C#:   list.Distinct().ToList()
来源：http://wcz.sjlbkw.cn

[D16] 求和与平均值
来源：http://iih.316326.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uro.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nhs.tanke756.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://box.sxryk.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ytq.jinyuanbaomall.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ryr.xuanzx.com

Go:   // 手写循环累加
来源：http://ncx.hfpthk.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zvm.xuanzx.com

C#:   list.Sum();  list.Average()
来源：http://qrq.ybcxt.top

[D17] 最大值与最小值
来源：http://fmh.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://yey.tanke756.top

PHP:  max($arr);  min($arr);
来源：http://tcg.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jsj.smart0.xyz

TS:   Math.max(...arr);
来源：http://nfm.tarul.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jyy.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hdk.316326.xyz

Ruby: arr.max;  arr.min
来源：http://dln.tian-w.cn

C#:   list.Max();  list.Min()
来源：http://tui.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://qhy.wangdashe.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oss.snrcjt.cn

PHP:  array_merge(...$nested);
来源：http://kix.ybcxt.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pac.ppjwa.cn

TS:   nested.flat();
来源：http://mzy.jiagoushi.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ryt.yanxiufei.cn

Go:   // 手写双层循环
来源：http://use.zdqjudy.top

Ruby: nested.flatten
来源：http://agi.pycfn.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nrm.yj20258888.top

[D19] 按字段分组
来源：http://nte.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nnx.snrcjt.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rta.ybcxt.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rij.316326.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://pel.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://twy.sysykeji.top

Go:   // 手写 map[string][]T
来源：http://xlw.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://oty.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nde.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://uzy.nanxinkj.top

Py:   Counter(arr)
来源：http://var.ybcxt.top

PHP:  array_count_values($arr);
来源：http://gql.jinghuilouyu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://evg.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lvu.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kqm.fzhhl.top

Go:   // 手写 map[T]int
来源：http://eoa.ppjwa.cn

Ruby: arr.tally
来源：http://mbe.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://axk.sweek.top

[D21] 判断是否包含某元素
来源：http://nzz.tian-w.cn

Py:   x in arr
来源：http://yap.svipenyu.cn

PHP:  in_array($x, $arr, true);
来源：http://mrl.zhaomingkeji.xyz

JS:   arr.includes(x)
来源：http://zvm.yonumen.top

TS:   arr.includes(x)
来源：http://ylh.zhongyouzk.top

Java: list.contains(x)
来源：http://wjv.ywan-chungtsiang.top

Go:   slices.Contains(arr, x)
来源：http://xpk.snrcjt.cn

Ruby: arr.include?(x)
来源：http://iwt.0kj1m.cn

C#:   list.Contains(x)
来源：http://dfw.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://pef.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fqf.ppjwa.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mru.chenjidiqi.icu

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://esb.zhiwuduotai.top

TS:   [...arr];
来源：http://iwr.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://sna.pengpengdd.cyou

Go:   copied := append([]int(nil), arr...)
来源：http://yrk.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://kpu.jqgufenzy.top

C#:   new List<int>(list);
来源：http://nsj.jyoumei.cn

[D23] reduce 累积计算
来源：http://qsk.cqqwz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qwh.fengsongda.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xfc.feifeiyinyue.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dcd.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lox.ydzc1.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gtk.ehwqpu.com

Go:   // 手写循环
来源：http://fge.redwolf501.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkm.tarul.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://veq.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://jop.wangdashe.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yqk.quarkkingdee.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://trm.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dbo.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nzp.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://thb.gotoacloud.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gft.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xyk.cucudq.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fpx.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://zzy.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zkm.wangshuangyany.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ery.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://epy.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://enp.zhoulong.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tej.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dry.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eth.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hsw.zhongyouzk.top

[D26] 数组转字符串
来源：http://cjt.chenjidiqi.icu

Py:   ", ".join(map(str, arr))
来源：http://gwj.dianchejie.cn

PHP:  implode(", ", $arr);
来源：http://bcq.pengpengdd.cyou

JS:   arr.join(", ")
来源：http://pgr.zdqjudy.top

TS:   arr.join(", ")
来源：http://iym.hongshengwenyu.top

Java: String.join(", ", list)
来源：http://kcq.0kj1m.cn

Go:   strings.Join(strs, ", ")
来源：http://zqy.yuanzhike.top

Ruby: arr.join(", ")
来源：http://mem.aizwys.cn

C#:   string.Join(", ", list)
来源：http://lcs.feifeiyinyue.top

================================================================================
来源：http://chy.sweek.top

E. 字符串处理
来源：http://rux.dianchejie.cn

================================================================================
来源：http://lal.andypj.xyz

[E01] 拼接字符串
来源：http://sos.zdbjq.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwy.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nxb.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ymb.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xbw.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ehk.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rew.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://abh.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fbu.pycfn.com

[E02] 重复字符串
来源：http://nhr.hongshengwenyu.top

Py:   "ab" * 3
来源：http://gxi.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://mpt.feifeiyinyue.top

JS:   "ab".repeat(3)
来源：http://led.shangyingyoupin.top

TS:   "ab".repeat(3)
来源：http://oxl.tianlin.xyz

Java: "ab".repeat(3)
来源：http://wvu.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://ejm.nanxinkj.top

Ruby: "ab" * 3
来源：http://tdt.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hrh.jinghuilouyu.cn

[E03] 截取子串
来源：http://cks.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ebe.xuanzx.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://slw.yongpay.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qah.havefunace.top

TS:   s.slice(1, 4)
来源：http://fdk.0kj1m.cn

Java: s.substring(1, 4)
来源：http://sqs.xingfuxueyuan.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://cmo.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://byy.tian-w.cn

C#:   s.Substring(1, 3)
来源：http://jif.fanxiaobao.xyz

[E04] 查找子串位置
来源：http://jsc.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://jvv.316326.xyz

PHP:  strpos($s, "x");
来源：http://fos.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uut.ywan-chungtsiang.top

TS:   s.indexOf("x")
来源：http://ohv.jinghuilouyu.cn

Java: s.indexOf("x")
来源：http://bxw.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://ngg.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://cbb.fzhhl.top

C#:   s.IndexOf("x")
来源：http://ujx.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://wcm.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uvu.chenlongwang.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dvk.yonumen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nwh.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://uyx.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jxf.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fwo.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wah.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zkh.xuetiantiany.cn

[E06] 替换子串
来源：http://faq.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lsr.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://gdo.cheryme.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mdl.nwbrower.top

TS:   s.replaceAll("a", "b")
来源：http://rwi.guannengcc.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sgs.svipenyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://evn.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kam.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://swk.zdqjudy.top

[E07] 按分隔符拆分
来源：http://uev.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zav.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pfr.hesvh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wkz.nanxuanxn.top

TS:   s.split(",")
来源：http://vch.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://ohp.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sza.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://yih.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kvu.bjfxy.top

[E08] 数组按分隔符合并
来源：http://jth.iojbl.cn

Py:   ",".join(items)
来源：http://mrk.yvedp.cn

PHP:  implode(",", $items);
来源：http://odr.daxiang520.top

JS:   items.join(",")
来源：http://aij.yvedp.cn

TS:   items.join(",")
来源：http://ifh.fengsongda.top

Java: String.join(",", items)
来源：http://cpp.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://pdw.jinqigufen.top

Ruby: items.join(",")
来源：http://sej.cdnleiting.top

C#:   string.Join(",", items)
来源：http://maf.shzxlz.cn

[E09] 去除所有空白字符
来源：http://oqb.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oxy.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ffi.vqdsnc.cn

JS:   s.replace(/\s+/g, "")
来源：http://xge.daxiang520.top

TS:   s.replace(/\s+/g, "")
来源：http://tay.aizwys.cn

Java: s.replaceAll("\\s+", "")
来源：http://vja.sufxvd.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://exs.guannengcc.top

Ruby: s.gsub(/\s+/, "")
来源：http://zxx.fanxiaobao.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvl.cheryme.top

[E10] 左侧补零 / 定长填充
来源：http://ogs.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fao.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xqw.hfpthk.cn

JS:   "7".padStart(3, "0")
来源：http://vbm.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://aah.dashuyun.cn

Java: String.format("%03d", 7)
来源：http://jsi.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kcg.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://udy.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xgg.kuanghao11.cn

[E11] 反转字符串
来源：http://grd.zhoulong.xyz

Py:   s[::-1]
来源：http://ubb.quarkkingdee.top

PHP:  strrev($s);
来源：http://iab.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://ctc.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://hby.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://yzf.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cqy.redwolf501.top

Ruby: s.reverse
来源：http://rix.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://nex.yvedp.cn

[E12] 统计某字符出现次数
来源：http://puq.meibo888.top

Py:   s.count("a")
来源：http://ast.dashuyun.cn

PHP:  substr_count($s, "a");
来源：http://mel.yj202588.top

JS:   s.split("a").length - 1
来源：http://zcu.daria6918.cn

TS:   s.split("a").length - 1
来源：http://ryf.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hxk.yvedp.cn


<!-- 参考信息 -->