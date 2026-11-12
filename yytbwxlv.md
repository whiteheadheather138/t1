代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://ics.fktsv.cn

TS:   [...a, ...b];
来源：http://xws.sjlbkw.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hfd.tianlin.xyz

Go:   append(a, b...)
来源：http://qkr.yj202588.top

Ruby: a + b;  a.concat(b)
来源：http://urp.shuidangran.top

C#:   a.Concat(b).ToList()
来源：http://kdg.jlsjyb.cn

[D09] 排序（升序）
来源：http://gnl.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bfn.ybcxt.top

PHP:  sort($arr);
来源：http://tte.kuanghao11.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xra.zhaomingkeji.xyz

TS:   [...arr].sort((x, y) => x - y);
来源：http://ijs.gogol.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vpb.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jna.xziqi.cn

Ruby: arr.sort
来源：http://dsz.yuxming.cn

C#:   list.Sort();
来源：http://jdl.pengpengdd.cyou

[D10] 自定义排序（按字段 / 多条件）
来源：http://kqp.vqdsnc.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://nze.guowangkeji.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jco.nanxuanxn.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qhs.uphjek.com

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nzw.yangfankeji.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://afi.shanyushiyangkeji.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nog.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dty.hysaishi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gny.jqgufenzy.top

[D11] 反转数组
来源：http://geh.tanke756.top

Py:   arr[::-1];  arr.reverse()
来源：http://wwe.chenzaomai.com

PHP:  array_reverse($arr);
来源：http://cyu.birdmap.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://icx.yj202588.top

TS:   [...arr].reverse();
来源：http://esf.nanxinkj.top

Java: Collections.reverse(list);
来源：http://qvh.chenlongwang.top

Go:   slices.Reverse(arr)
来源：http://rds.jqgufenzy.top

Ruby: arr.reverse
来源：http://sez.nanxuanxn.top

C#:   list.Reverse();
来源：http://wuv.tanke756.top

[D12] 查找元素下标
来源：http://lcl.sufxvd.cn

Py:   arr.index(x);  x in arr
来源：http://gso.aizwys.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gfq.nanxinkj.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yzy.yangfankeji.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zdn.c1oappe.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://huo.9152youxi.cn

Go:   slices.Index(arr, x)
来源：http://mru.tarul.cn

Ruby: arr.index(x)
来源：http://oqx.sjlbkw.cn

C#:   list.IndexOf(x);
来源：http://bal.sweek.top

[D13] 过滤（保留满足条件的）
来源：http://iaw.chenjidiqi.icu

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kic.jyoumei.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tvu.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://phg.ppjwa.cn

TS:   arr.filter(x => x > 3)
来源：http://nyc.yj20258888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ilq.hnqzz.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nsd.ydjk.org.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kar.zhiwuduotai.top

C#:   list.Where(x => x > 3).ToList()
来源：http://pxh.daria6918.cn

[D14] 映射转换（每个元素变形）
来源：http://lho.hywenlv.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://knl.hfpthk.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fal.xingfuxueyuan.xyz

JS:   arr.map(x => x * 2)
来源：http://awr.jinqigfzy.top

TS:   arr.map(x => x * 2)
来源：http://pfs.chenjidiqi.icu

Java: list.stream().map(x -> x * 2).toList()
来源：http://khi.fehbvm.com

Go:   // 手写循环
来源：http://add.redwolf501.top

Ruby: arr.map { |x| x * 2 }
来源：http://hsz.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qov.fanxiaobao.xyz

[D15] 去重
来源：http://ipj.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zud.chenlongwang.top

PHP:  array_unique($arr);
来源：http://hin.jlsjyb.cn

JS:   [...new Set(arr)]
来源：http://pqo.yanxiufei.cn

TS:   [...new Set(arr)]
来源：http://zwm.snrcjt.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wgm.tianlin.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://umk.dianchejie.cn

Ruby: arr.uniq
来源：http://nsk.hnqzz.top

C#:   list.Distinct().ToList()
来源：http://jse.quarkkingdee.top

[D16] 求和与平均值
来源：http://rdt.nanxuanxn.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hid.yvedp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vwm.yangfankeji.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jfv.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zli.quarkkingdee.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wmt.sysykeji.top

Go:   // 手写循环累加
来源：http://rqv.andypj.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qnc.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://cvg.kuanghao11.cn

[D17] 最大值与最小值
来源：http://lty.daxiang520.top

Py:   max(arr);  min(arr)
来源：http://jdl.dashuyun.cn

PHP:  max($arr);  min($arr);
来源：http://yth.ydzc1.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dem.yanxiufei.cn

TS:   Math.max(...arr);
来源：http://egb.aibaodan.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mzv.chenjidiqi.icu

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pdm.svipenyu.cn

Ruby: arr.max;  arr.min
来源：http://tgn.xuetiantiany.cn

C#:   list.Max();  list.Min()
来源：http://wwf.vehdjk.com

[D18] 扁平化嵌套数组
来源：http://omw.yangfankeji.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kxl.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://oms.hesvh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sxa.yonumen.top

TS:   nested.flat();
来源：http://pwu.vqdsnc.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xgj.snrcjt.cn

Go:   // 手写双层循环
来源：http://xbj.yongpay.top

Ruby: nested.flatten
来源：http://vsi.tian-w.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bqk.zhiwuduotai.top

[D19] 按字段分组
来源：http://ogc.bjfxy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://aqx.pycfn.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tho.sufxvd.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xes.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hqv.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gvt.sweek.top

Go:   // 手写 map[string][]T
来源：http://wok.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wiq.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vgb.vqdsnc.cn

[D20] 统计每个元素出现次数
来源：http://jkw.zdbjq.cn

Py:   Counter(arr)
来源：http://hnr.aizwys.cn

PHP:  array_count_values($arr);
来源：http://msq.aibaodan.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xpa.zdqjudy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://afo.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aie.jlsjyb.cn

Go:   // 手写 map[T]int
来源：http://lkq.shanyushiyangkeji.top

Ruby: arr.tally
来源：http://fln.yfazqb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ozj.havefunace.top

[D21] 判断是否包含某元素
来源：http://eae.vqdsnc.cn

Py:   x in arr
来源：http://clx.haohaochexian.top

PHP:  in_array($x, $arr, true);
来源：http://fgw.svipenyu.cn

JS:   arr.includes(x)
来源：http://apr.meibo888.top

TS:   arr.includes(x)
来源：http://qwx.jinqigufen.top

Java: list.contains(x)
来源：http://zvj.zhiwuduotai.top

Go:   slices.Contains(arr, x)
来源：http://krr.zhongyouzk.top

Ruby: arr.include?(x)
来源：http://whw.quarkkingdee.top

C#:   list.Contains(x)
来源：http://fsg.ehwqpu.com

[D22] 复制数组（避免共享引用）
来源：http://uei.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vbp.jinqigufen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://etu.vehdjk.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://joh.hywenlv.cn

TS:   [...arr];
来源：http://jsv.aizwys.cn

Java: new ArrayList<>(list);
来源：http://dpa.wangshuangyany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ueh.xylfe.cn

Ruby: arr.dup;  arr.clone
来源：http://hcs.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://mms.tianlin.xyz

[D23] reduce 累积计算
来源：http://mol.chenzaomai.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hfa.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mph.hongshengwenyu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uhq.fzhhl.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://phv.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pwq.zhijiandao.cn

Go:   // 手写循环
来源：http://prb.zdbjq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pzw.yueranfly.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://koz.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://kmi.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ozv.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://eos.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sef.snrcjt.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mxz.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tau.yvedp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqn.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jjj.zhongyouzk.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rlz.c1oappe.top

[D25] Set 集合去重与交并差
来源：http://igh.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://phi.epnwcf.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tjy.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wfd.jlsjyb.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dwu.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qnj.316326.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ikv.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hsu.jlsjyb.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ufl.yuanzhike.top

[D26] 数组转字符串
来源：http://poq.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://zob.fzhhl.top

PHP:  implode(", ", $arr);
来源：http://ogn.yongpay.top

JS:   arr.join(", ")
来源：http://ztf.ctjpmb.com

TS:   arr.join(", ")
来源：http://vzt.hfpthk.cn

Java: String.join(", ", list)
来源：http://ivr.gaohongyu789.top

Go:   strings.Join(strs, ", ")
来源：http://yxz.jinqigufen.top

Ruby: arr.join(", ")
来源：http://ynv.dianchejie.cn

C#:   string.Join(", ", list)
来源：http://efq.nanxinkj.top

================================================================================
来源：http://bhq.bjfxy.top

E. 字符串处理
来源：http://zzb.fktsv.cn

================================================================================
来源：http://zlb.ivvv.top

[E01] 拼接字符串
来源：http://aog.chenzaomai.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ybm.cashguo.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://opl.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dxq.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpm.uphjek.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nwe.jiagoushi.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cqk.andypj.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kwi.chenjidiqi.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://djq.shzxlz.cn

[E02] 重复字符串
来源：http://lum.sufxvd.cn

Py:   "ab" * 3
来源：http://kau.52xcode.cn

PHP:  str_repeat("ab", 3);
来源：http://gyz.cqqwz.cn

JS:   "ab".repeat(3)
来源：http://mbm.wangdashe.top

TS:   "ab".repeat(3)
来源：http://glh.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://mfi.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://bzu.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://yvz.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mjj.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://xud.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wfs.jyoumei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hez.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ikg.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://yjs.xinyue.icu

Java: s.substring(1, 4)
来源：http://gxk.snrcjt.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eqd.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://cky.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://qzz.sjlbkw.cn

[E04] 查找子串位置
来源：http://mrt.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://amj.pycfn.com

PHP:  strpos($s, "x");
来源：http://hlh.zdbjq.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ynq.shzxlz.cn

TS:   s.indexOf("x")
来源：http://lpv.0kj1m.cn

Java: s.indexOf("x")
来源：http://vqf.cucudq.cn

Go:   strings.Index(s, "x")
来源：http://goj.meibo888.top

Ruby: s.index("x")
来源：http://wfb.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://thv.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lig.316326.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ryw.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://efd.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zlk.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ojo.jianghu66.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://acp.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ebh.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zcr.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://phz.nwbrower.top

[E06] 替换子串
来源：http://xbq.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lnz.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://mdc.ydjk.org.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://exl.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://duo.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://och.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fha.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://otn.fehbvm.com

C#:   s.Replace("a", "b")
来源：http://kur.feifeiyinyue.top

[E07] 按分隔符拆分
来源：http://ayu.svipenyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ays.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vic.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ggl.uphjek.com

TS:   s.split(",")
来源：http://sez.hammf.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zpp.meibo888.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cas.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://ekk.iojbl.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wop.xuanzx.com

[E08] 数组按分隔符合并
来源：http://hph.pengpengdd.cyou

Py:   ",".join(items)
来源：http://fls.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://hzt.ehwqpu.com

JS:   items.join(",")
来源：http://pkm.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://sgu.tianlin.xyz

Java: String.join(",", items)
来源：http://eid.yonumen.top

Go:   strings.Join(items, ",")
来源：http://qqv.jqgufenzy.top

Ruby: items.join(",")
来源：http://ccf.hfpthk.cn

C#:   string.Join(",", items)
来源：http://dlx.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://gqo.ydjk.org.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://plv.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xeh.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://uwj.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://ubp.daria6918.cn

Java: s.replaceAll("\\s+", "")
来源：http://npw.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gln.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://vli.zycfv.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vmv.daria6918.cn

[E10] 左侧补零 / 定长填充
来源：http://pve.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sxn.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xrq.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://tho.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://fpc.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://wfp.ppjwa.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dkc.feifeiyinyue.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tje.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hwz.fzhhl.top

[E11] 反转字符串
来源：http://hqj.xuanzx.com

Py:   s[::-1]
来源：http://fmr.xuanzx.com

PHP:  strrev($s);
来源：http://qhu.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://cfj.hywenlv.cn

TS:   [...s].reverse().join("")
来源：http://pdw.mhx1999.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vvs.zdqjudy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oxo.snrcjt.cn

Ruby: s.reverse
来源：http://iip.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://siv.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://awa.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://ewp.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://xhg.yj202588.top

JS:   s.split("a").length - 1
来源：http://fmv.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://nin.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wyq.yuanzhike.top

Go:   strings.Count(s, "a")
来源：http://gko.hammf.cn

Ruby: s.count("a")
来源：http://kfs.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://xmk.yvedp.cn

[E13] 逐字符遍历
来源：http://cwn.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://axc.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hnf.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ppm.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zuz.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://etd.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fyq.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xnb.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dyh.cheryme.top

[E14] URL 编码与 Base64
来源：http://duj.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qvr.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ttj.shuidangran.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://knr.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iew.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kzn.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mjv.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ipu.yuxming.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dky.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://wdx.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kwl.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bez.gotoacloud.top


<!-- 参考信息 -->