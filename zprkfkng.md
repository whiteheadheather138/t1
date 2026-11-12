代发 wailian999

Py:   len(arr)
来源：http://nxa.cdnleiting.top

PHP:  count($arr);
来源：http://mem.zhoulong.xyz

JS:   arr.length
来源：http://ncv.sufxvd.cn

TS:   arr.length
来源：http://lrx.c1oappe.top

Java: list.size();
来源：http://myd.zdbjq.cn

Go:   len(arr)
来源：http://nsc.chenjidiqi.icu

Ruby: arr.length; arr.size
来源：http://ime.hnxiangtu.top

C#:   list.Count;
来源：http://ioi.redwolf501.top

[D07] 切片 / 取子数组
来源：http://bst.xziqi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jpw.jiagoushi.top

PHP:  array_slice($arr, 1, 3);
来源：http://wfz.cheryme.top

JS:   arr.slice(1, 4);
来源：http://nfs.zhoulong.xyz

TS:   arr.slice(1, 4);
来源：http://cfv.feifeiyinyue.top

Java: list.subList(1, 4);
来源：http://wzz.uphjek.com

Go:   arr[1:4]
来源：http://pqa.cashguo.top

Ruby: arr[1, 3]
来源：http://dms.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://tdp.dianchejie.cn

[D08] 合并两个数组
来源：http://ihi.yj20258.top

Py:   a + b;  a.extend(b)
来源：http://iyt.nanxinkj.top

PHP:  array_merge($a, $b);
来源：http://kze.yvedp.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gcr.yangfankeji.com

TS:   [...a, ...b];
来源：http://wbe.gaohongyu789.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ukl.xingfuxueyuan.xyz

Go:   append(a, b...)
来源：http://hux.xylfe.cn

Ruby: a + b;  a.concat(b)
来源：http://zxu.ehwqpu.com

C#:   a.Concat(b).ToList()
来源：http://kvs.epnwcf.com

[D09] 排序（升序）
来源：http://ynv.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://fuw.hongshengwenyu.top

PHP:  sort($arr);
来源：http://npq.havefunace.top

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qfs.zhongyouzk.top

TS:   [...arr].sort((x, y) => x - y);
来源：http://mtq.chenlongwang.top

Java: Collections.sort(list);  list.sort(null);
来源：http://wnq.epnwcf.com

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rtj.cheryme.top

Ruby: arr.sort
来源：http://zpr.haohaochexian.top

C#:   list.Sort();
来源：http://gkh.cdnleiting.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://sbg.hywenlv.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yrn.yonumen.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kpp.xuetiantiany.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yxt.hcnkem.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ylf.mhx1999.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bzp.havefunace.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qeu.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://huq.fanxiaobao.xyz

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lfv.nanxinkj.top

[D11] 反转数组
来源：http://guh.nanxuanxn.top

Py:   arr[::-1];  arr.reverse()
来源：http://tyg.shzxlz.cn

PHP:  array_reverse($arr);
来源：http://ayj.yangfankeji.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pex.yuxming.cn

TS:   [...arr].reverse();
来源：http://xea.jyoumei.cn

Java: Collections.reverse(list);
来源：http://dnp.tianlin.xyz

Go:   slices.Reverse(arr)
来源：http://jdq.zhijiandao.cn

Ruby: arr.reverse
来源：http://ulz.kuanghao11.cn

C#:   list.Reverse();
来源：http://vbm.dianchejie.cn

[D12] 查找元素下标
来源：http://zfe.wangshuangyany.cn

Py:   arr.index(x);  x in arr
来源：http://tdz.jiagoushi.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gum.ehwqpu.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://grt.zdbjq.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ezu.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://coz.daxiang520.top

Go:   slices.Index(arr, x)
来源：http://fzr.nwbrower.top

Ruby: arr.index(x)
来源：http://oky.vqdsnc.cn

C#:   list.IndexOf(x);
来源：http://sxg.yonumen.top

[D13] 过滤（保留满足条件的）
来源：http://dsr.chenzaomai.com

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://tfh.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uhm.dashuyun.cn

JS:   arr.filter(x => x > 3)
来源：http://pcp.pycfn.com

TS:   arr.filter(x => x > 3)
来源：http://czd.wangdashe.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://esy.smart0.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://okf.sufxvd.cn

Ruby: arr.select { |x| x > 3 }
来源：http://uxc.sxryk.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vkw.xuetiantiany.cn

[D14] 映射转换（每个元素变形）
来源：http://xwi.ehwqpu.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xxr.jinyuanbaomall.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dmp.quarkkingdee.top

JS:   arr.map(x => x * 2)
来源：http://dbz.fktsv.cn

TS:   arr.map(x => x * 2)
来源：http://lgx.hnqzz.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://hvv.wangshuangyany.cn

Go:   // 手写循环
来源：http://emr.bjfxy.top

Ruby: arr.map { |x| x * 2 }
来源：http://esj.zdbjq.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://iyh.daxiang520.top

[D15] 去重
来源：http://gkb.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yyr.shanyushiyangkeji.top

PHP:  array_unique($arr);
来源：http://tnd.hysaishi.cn

JS:   [...new Set(arr)]
来源：http://cng.bbcook.cn

TS:   [...new Set(arr)]
来源：http://jzp.redwolf501.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wdz.yangfankeji.com

Go:   // 用 map[T]struct{} 手写
来源：http://olu.cqqwz.cn

Ruby: arr.uniq
来源：http://rii.yangfankeji.com

C#:   list.Distinct().ToList()
来源：http://awe.316326.xyz

[D16] 求和与平均值
来源：http://tek.gzhubu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mvd.aibaodan.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jjz.uphjek.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsw.zycfv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajh.tian-w.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hpx.xziqi.cn

Go:   // 手写循环累加
来源：http://ylr.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://usv.dianchejie.cn

C#:   list.Sum();  list.Average()
来源：http://zzs.cheryme.top

[D17] 最大值与最小值
来源：http://fvr.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://ujo.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://ycj.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://aqv.xziqi.cn

TS:   Math.max(...arr);
来源：http://yio.jyoumei.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ujj.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fle.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://voj.wangdashe.top

C#:   list.Max();  list.Min()
来源：http://ytf.yj20258888.top

[D18] 扁平化嵌套数组
来源：http://dqr.tanke756.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vnr.hnqzz.top

PHP:  array_merge(...$nested);
来源：http://inf.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wnf.yonumen.top

TS:   nested.flat();
来源：http://jux.feifeiyinyue.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vth.sjlbkw.cn

Go:   // 手写双层循环
来源：http://and.jyoumei.cn

Ruby: nested.flatten
来源：http://yau.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://mcq.gotoacloud.top

[D19] 按字段分组
来源：http://idd.jinqigfzy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yja.gogol.net.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pdy.xuetiantiany.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ylw.fehbvm.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://fno.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iod.yuxming.cn

Go:   // 手写 map[string][]T
来源：http://peo.zdqjudy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wcz.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eft.meibo888.top

[D20] 统计每个元素出现次数
来源：http://aki.dashuyun.cn

Py:   Counter(arr)
来源：http://glq.yuxming.cn

PHP:  array_count_values($arr);
来源：http://olt.zhiwuduotai.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wyi.pycfn.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dha.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gkl.andypj.xyz

Go:   // 手写 map[T]int
来源：http://wwx.meibo888.top

Ruby: arr.tally
来源：http://xys.ehwqpu.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dkr.nanxuanxn.top

[D21] 判断是否包含某元素
来源：http://muk.hammf.cn

Py:   x in arr
来源：http://hum.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://wcq.vqdsnc.cn

JS:   arr.includes(x)
来源：http://xjz.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://oof.tarul.cn

Java: list.contains(x)
来源：http://tjy.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://vju.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://sby.jianghu66.top

C#:   list.Contains(x)
来源：http://hnk.chenlongwang.top

[D22] 复制数组（避免共享引用）
来源：http://kkp.sysykeji.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gjz.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dkb.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://agv.0kj1m.cn

TS:   [...arr];
来源：http://vbj.tarul.cn

Java: new ArrayList<>(list);
来源：http://dqk.xingfuxueyuan.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://ptj.yj20258.top

Ruby: arr.dup;  arr.clone
来源：http://kxa.ywan-chungtsiang.top

C#:   new List<int>(list);
来源：http://cmi.yonumen.top

[D23] reduce 累积计算
来源：http://pci.hesvh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gvm.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://skr.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xqw.daxiang520.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qne.ctjpmb.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://qxx.jiagoushi.top

Go:   // 手写循环
来源：http://sgn.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jwv.ivvv.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hbh.jinqigufen.top

[D24] 字典 / Map 基本操作
来源：http://klp.tianlin.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qba.zhaomingkeji.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://chf.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://srf.xziqi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vhr.gaohongyu789.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ggg.ydzc1.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ese.feifeiyinyue.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://fin.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nep.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://jrv.52xcode.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://czh.chenlongwang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uzx.zhengqikj.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gor.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wrp.zhiwuduotai.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lly.hywenlv.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://trx.pengpengdd.cyou

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bwm.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fhv.9152youxi.cn

[D26] 数组转字符串
来源：http://xdn.pengpengdd.cyou

Py:   ", ".join(map(str, arr))
来源：http://xou.hesvh.cn

PHP:  implode(", ", $arr);
来源：http://yyh.jqgufenzy.top

JS:   arr.join(", ")
来源：http://dnw.yj202588.top

TS:   arr.join(", ")
来源：http://tps.jlsjyb.cn

Java: String.join(", ", list)
来源：http://bcz.mhx1999.top

Go:   strings.Join(strs, ", ")
来源：http://bio.gzhubu.top

Ruby: arr.join(", ")
来源：http://ank.xinyue.icu

C#:   string.Join(", ", list)
来源：http://dwx.nanxinkj.top

================================================================================
来源：http://ykz.sxryk.cn

E. 字符串处理
来源：http://uzc.shanyushiyangtech.top

================================================================================
来源：http://voy.hysaishi.cn

[E01] 拼接字符串
来源：http://rfg.xingfuxueyuan.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://axn.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://prv.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtx.hnxiangtu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tdz.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yde.epnwcf.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sfs.iojbl.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nlo.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dut.hongshengwenyu.top

[E02] 重复字符串
来源：http://rso.xuanzx.com

Py:   "ab" * 3
来源：http://wpu.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://amh.uphjek.com

JS:   "ab".repeat(3)
来源：http://bcz.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://nin.fengsongda.top

Java: "ab".repeat(3)
来源：http://ugr.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://zlu.fzhhl.top

Ruby: "ab" * 3
来源：http://kpr.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aiq.hnxiangtu.top

[E03] 截取子串
来源：http://btv.ydzc1.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dny.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pqz.hammf.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vff.yongpay.top

TS:   s.slice(1, 4)
来源：http://izj.fktsv.cn

Java: s.substring(1, 4)
来源：http://yux.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gdf.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://czz.shanyushiyangkeji.top

C#:   s.Substring(1, 3)
来源：http://uqb.aibaodan.cn

[E04] 查找子串位置
来源：http://gyf.vqdsnc.cn

Py:   s.find("x");  s.index("x")
来源：http://kdr.redwolf501.top

PHP:  strpos($s, "x");
来源：http://bzb.yj20258888.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rqi.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://yxf.uphjek.com

Java: s.indexOf("x")
来源：http://ilb.vqdsnc.cn

Go:   strings.Index(s, "x")
来源：http://zgp.yongpay.top

Ruby: s.index("x")
来源：http://xmk.cashguo.top

C#:   s.IndexOf("x")
来源：http://yhd.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bwm.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pqi.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xxd.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vhd.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cdw.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upf.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://iaj.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rhc.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jul.haohaochexian.top

[E06] 替换子串
来源：http://fft.xingfuxueyuan.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pli.vqdsnc.cn

PHP:  str_replace("a", "b", $s);
来源：http://pql.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yoq.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://pms.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vbk.zhixingplan.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iha.ybcxt.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bzp.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://cjh.guowangkeji.top

[E07] 按分隔符拆分
来源：http://rtb.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mjf.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rnd.ivvv.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbh.nwbrower.top

TS:   s.split(",")
来源：http://bhb.xuetiantiany.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bxn.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://iat.zhongyouzk.top

Ruby: s.split(",");  s.split
来源：http://qjm.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyc.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://wjt.yonumen.top

Py:   ",".join(items)
来源：http://lnl.chenzaomai.com

PHP:  implode(",", $items);
来源：http://ezq.mhx1999.top

JS:   items.join(",")
来源：http://jnu.shzxlz.cn

TS:   items.join(",")
来源：http://dia.yuxming.cn

Java: String.join(",", items)
来源：http://sur.jianghu66.top

Go:   strings.Join(items, ",")
来源：http://mzn.hnqzz.top

Ruby: items.join(",")
来源：http://uzj.ivvv.top

C#:   string.Join(",", items)
来源：http://ztd.xuanzx.com

[E09] 去除所有空白字符
来源：http://dvp.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dwt.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hrh.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://dio.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://ivi.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://owm.yongpay.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mdx.jianghu66.top

Ruby: s.gsub(/\s+/, "")
来源：http://end.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ghm.fzhhl.top

[E10] 左侧补零 / 定长填充
来源：http://ydf.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ndv.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sjz.dashuyun.cn

JS:   "7".padStart(3, "0")
来源：http://hxc.yj202588.top

TS:   "7".padStart(3, "0")
来源：http://skp.smart0.xyz

Java: String.format("%03d", 7)
来源：http://sdo.xuanzx.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://tpi.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zyt.jinyuanbaomall.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ege.hammf.cn

[E11] 反转字符串
来源：http://xbw.xylfe.cn

Py:   s[::-1]
来源：http://axg.wangdashe.top

PHP:  strrev($s);
来源：http://lnj.fanxiaobao.xyz

JS:   [...s].reverse().join("")
来源：http://qoz.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://ltc.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qjh.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://joy.snrcjt.cn

Ruby: s.reverse
来源：http://irj.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://isr.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://iua.iojbl.cn

Py:   s.count("a")
来源：http://ndl.bjfxy.top

PHP:  substr_count($s, "a");
来源：http://tgl.yangfankeji.com

JS:   s.split("a").length - 1
来源：http://cto.pycfn.com

TS:   s.split("a").length - 1
来源：http://sex.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wbu.wangdashe.top

Go:   strings.Count(s, "a")
来源：http://wld.uphjek.com

Ruby: s.count("a")
来源：http://zsf.hesvh.cn

C#:   s.Count(c => c == 'a')
来源：http://qzm.ctjpmb.com

[E13] 逐字符遍历
来源：http://qkr.iojbl.cn


<!-- 参考信息 -->