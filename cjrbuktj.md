代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://xtb.zhengqikj.top

TS:   [...a, ...b];
来源：http://hiz.mhx1999.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kqs.ivvv.top

Go:   append(a, b...)
来源：http://uss.ctjpmb.com

Ruby: a + b;  a.concat(b)
来源：http://vvq.nwbrower.top

C#:   a.Concat(b).ToList()
来源：http://qlr.jqgufenzy.top

[D09] 排序（升序）
来源：http://mtj.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://ham.dianchejie.cn

PHP:  sort($arr);
来源：http://dgr.0kj1m.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bwp.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gmm.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qjp.yvedp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://uys.shangyingyoupin.top

Ruby: arr.sort
来源：http://cgc.c1oappe.top

C#:   list.Sort();
来源：http://eci.aibaodan.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cds.jinyuanbaomall.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://dex.jqgufenzy.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ssr.jlsjyb.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ajg.redwolf501.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://qjx.haohaochexian.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://adq.hysaishi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eyx.svipenyu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://crk.ywan-chungtsiang.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aor.jqgfzy.top

[D11] 反转数组
来源：http://xjh.jqgufenzy.top

Py:   arr[::-1];  arr.reverse()
来源：http://foh.hywenlv.cn

PHP:  array_reverse($arr);
来源：http://ada.ydzc1.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://suw.nwbrower.top

TS:   [...arr].reverse();
来源：http://iay.yj202588.top

Java: Collections.reverse(list);
来源：http://kha.ydjk.org.cn

Go:   slices.Reverse(arr)
来源：http://giq.chenlongwang.top

Ruby: arr.reverse
来源：http://ers.cqqwz.cn

C#:   list.Reverse();
来源：http://kro.sjlbkw.cn

[D12] 查找元素下标
来源：http://ylx.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://oof.nanxinkj.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nrt.hammf.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://izs.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gmo.jinghuilouyu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cug.guowangkeji.top

Go:   slices.Index(arr, x)
来源：http://dst.hfpthk.cn

Ruby: arr.index(x)
来源：http://ukc.xylfe.cn

C#:   list.IndexOf(x);
来源：http://azz.havefunace.top

[D13] 过滤（保留满足条件的）
来源：http://gug.aibaodan.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://nan.zhoulong.xyz

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://pmo.daxiang520.top

JS:   arr.filter(x => x > 3)
来源：http://qrd.xziqi.cn

TS:   arr.filter(x => x > 3)
来源：http://ndb.fanxiaobao.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://yox.yonumen.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://emy.shuidangran.top

Ruby: arr.select { |x| x > 3 }
来源：http://dns.feifeiyinyue.top

C#:   list.Where(x => x > 3).ToList()
来源：http://qyn.uphjek.com

[D14] 映射转换（每个元素变形）
来源：http://tab.xylfe.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qov.hongshengwenyu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://aqu.birdmap.top

JS:   arr.map(x => x * 2)
来源：http://rhm.jinyuanbaomall.cn

TS:   arr.map(x => x * 2)
来源：http://yyk.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ixv.shzxlz.cn

Go:   // 手写循环
来源：http://vwt.gogol.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gnf.chenlongwang.top

C#:   list.Select(x => x * 2).ToList()
来源：http://ela.epnwcf.com

[D15] 去重
来源：http://kdg.sysykeji.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pac.fktsv.cn

PHP:  array_unique($arr);
来源：http://spx.andypj.xyz

JS:   [...new Set(arr)]
来源：http://scz.quarkkingdee.top

TS:   [...new Set(arr)]
来源：http://her.yonumen.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qve.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://sqw.yj20258.top

Ruby: arr.uniq
来源：http://bdv.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://kpn.hcnkem.com

[D16] 求和与平均值
来源：http://bor.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sat.andypj.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://stx.ybcxt.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgx.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bgv.wangshuangyany.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tsb.vqdsnc.cn

Go:   // 手写循环累加
来源：http://avh.bjfxy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cbz.wangdashe.top

C#:   list.Sum();  list.Average()
来源：http://dyc.nwbrower.top

[D17] 最大值与最小值
来源：http://fdb.yuanzhike.top

Py:   max(arr);  min(arr)
来源：http://syr.pengpengdd.cyou

PHP:  max($arr);  min($arr);
来源：http://zbc.jinqigufen.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qef.sjlbkw.cn

TS:   Math.max(...arr);
来源：http://bcr.fehbvm.com

Java: Collections.max(list);  Collections.min(list);
来源：http://twm.xylfe.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://diq.sjlbkw.cn

Ruby: arr.max;  arr.min
来源：http://kuc.haohaochexian.top

C#:   list.Max();  list.Min()
来源：http://hka.jinyuanbaomall.cn

[D18] 扁平化嵌套数组
来源：http://vnf.xuetiantiany.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dam.gotoacloud.top

PHP:  array_merge(...$nested);
来源：http://whc.yj20258888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tjr.chenzaomai.com

TS:   nested.flat();
来源：http://omk.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lph.xuanzx.com

Go:   // 手写双层循环
来源：http://lmk.wangshuangyany.cn

Ruby: nested.flatten
来源：http://loq.9152youxi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uep.fktsv.cn

[D19] 按字段分组
来源：http://igw.shangyingyoupin.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://czm.fzhhl.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://djx.jyoumei.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dpe.zhongyouzk.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://vaq.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wni.birdmap.top

Go:   // 手写 map[string][]T
来源：http://ipn.yfazqb.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://ota.chenjidiqi.icu

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mlr.yj20258888.top

[D20] 统计每个元素出现次数
来源：http://cmi.jiagoushi.top

Py:   Counter(arr)
来源：http://cvq.xziqi.cn

PHP:  array_count_values($arr);
来源：http://cvx.bbcook.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pux.jlsjyb.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rli.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iom.gotoacloud.top

Go:   // 手写 map[T]int
来源：http://qej.shuidangran.top

Ruby: arr.tally
来源：http://ktd.dashuyun.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dow.jqgfzy.top

[D21] 判断是否包含某元素
来源：http://sut.zhoulong.xyz

Py:   x in arr
来源：http://nwg.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://wbb.zhixingplan.top

JS:   arr.includes(x)
来源：http://vbq.jianghu66.top

TS:   arr.includes(x)
来源：http://gjn.xylfe.cn

Java: list.contains(x)
来源：http://rcf.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://oie.ehwqpu.com

Ruby: arr.include?(x)
来源：http://naq.hfpthk.cn

C#:   list.Contains(x)
来源：http://nqi.shuidangran.top

[D22] 复制数组（避免共享引用）
来源：http://uai.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tiy.birdmap.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zla.52xcode.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jko.yj20258.top

TS:   [...arr];
来源：http://msc.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://ytz.zdbjq.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zyf.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://cxr.smart0.xyz

C#:   new List<int>(list);
来源：http://yfs.fehbvm.com

[D23] reduce 累积计算
来源：http://sxi.wangdashe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lzm.yfazqb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dqk.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ljs.hongshengwenyu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hvg.shangyingyoupin.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://wis.guowangkeji.top

Go:   // 手写循环
来源：http://pdc.snrcjt.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vhq.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://izt.9152youxi.cn

[D24] 字典 / Map 基本操作
来源：http://npv.yueranfly.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aay.yanxiufei.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nlx.sjlbkw.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qye.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dca.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zys.quarkkingdee.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oun.52xcode.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://epu.xuanzx.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vsy.shuidangran.top

[D25] Set 集合去重与交并差
来源：http://gpq.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wie.vqdsnc.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pxy.iojbl.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sky.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ifp.fzhhl.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yuj.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgr.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyb.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xht.jlsjyb.cn

[D26] 数组转字符串
来源：http://pim.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://oew.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://azm.cashguo.top

JS:   arr.join(", ")
来源：http://iym.yangfankeji.com

TS:   arr.join(", ")
来源：http://due.cashguo.top

Java: String.join(", ", list)
来源：http://nyg.shangyingyoupin.top

Go:   strings.Join(strs, ", ")
来源：http://vrr.yj20258.top

Ruby: arr.join(", ")
来源：http://smq.sjlbkw.cn

C#:   string.Join(", ", list)
来源：http://qol.yj20258.top

================================================================================
来源：http://uoq.nanxinkj.top

E. 字符串处理
来源：http://pum.hcnkem.com

================================================================================
来源：http://wxe.gzhubu.top

[E01] 拼接字符串
来源：http://eny.iojbl.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pmg.iojbl.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dju.9152youxi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mum.shzxlz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qbz.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nsd.hammf.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zqk.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vci.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uyv.yfazqb.com

[E02] 重复字符串
来源：http://zks.xingfuxueyuan.xyz

Py:   "ab" * 3
来源：http://ums.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://jht.xuanzx.com

JS:   "ab".repeat(3)
来源：http://cxw.52xcode.cn

TS:   "ab".repeat(3)
来源：http://fxs.shuidangran.top

Java: "ab".repeat(3)
来源：http://ggb.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://fyt.0kj1m.cn

Ruby: "ab" * 3
来源：http://cfq.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jvn.uphjek.com

[E03] 截取子串
来源：http://stl.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lfg.wangdashe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gmr.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmi.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://vkz.yvedp.cn

Java: s.substring(1, 4)
来源：http://ujt.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ztc.hysaishi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://evd.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://iiq.vehdjk.com

[E04] 查找子串位置
来源：http://tqd.daxiang520.top

Py:   s.find("x");  s.index("x")
来源：http://kew.c1oappe.top

PHP:  strpos($s, "x");
来源：http://twh.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xct.dianchejie.cn

TS:   s.indexOf("x")
来源：http://ddk.yj20258888.top

Java: s.indexOf("x")
来源：http://yha.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://mdu.shangyingyoupin.top

Ruby: s.index("x")
来源：http://ewc.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://avo.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wgo.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ykm.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://unm.fanxiaobao.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ayh.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qdf.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xzn.jlsjyb.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://svc.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://azx.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://etn.shangyingyoupin.top

[E06] 替换子串
来源：http://vqp.yuxming.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bfh.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://utj.xuetiantiany.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sxe.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://nxz.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wpy.zdbjq.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eew.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gfv.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://lld.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://ycg.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://agy.cashguo.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qcd.xuanzx.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://otl.yuanzhike.top

TS:   s.split(",")
来源：http://pvn.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://thl.sweek.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lxj.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://wwe.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ety.52xcode.cn

[E08] 数组按分隔符合并
来源：http://toq.zhongyouzk.top

Py:   ",".join(items)
来源：http://evu.mhx1999.top

PHP:  implode(",", $items);
来源：http://vbb.tian-w.cn

JS:   items.join(",")
来源：http://cef.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://guz.yanxiufei.cn

Java: String.join(",", items)
来源：http://hti.yvedp.cn

Go:   strings.Join(items, ",")
来源：http://cvk.daxiang520.top

Ruby: items.join(",")
来源：http://vwq.zdbjq.cn

C#:   string.Join(",", items)
来源：http://ymn.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://sjo.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zyn.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ajw.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://hhy.ywan-chungtsiang.top

TS:   s.replace(/\s+/g, "")
来源：http://vkn.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://qlo.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eep.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://tzo.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oid.aibaodan.cn

[E10] 左侧补零 / 定长填充
来源：http://gcd.c1oappe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cxm.hfpthk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ssc.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://wgz.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://kch.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://xwi.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lbf.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgg.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ixu.cashguo.top

[E11] 反转字符串
来源：http://pgx.shanyushiyangkeji.top

Py:   s[::-1]
来源：http://oyo.xuetiantiany.cn

PHP:  strrev($s);
来源：http://lfx.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://peo.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://mgs.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ctu.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nla.shangyingyoupin.top

Ruby: s.reverse
来源：http://eit.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://pug.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://ytj.zdbjq.cn

Py:   s.count("a")
来源：http://yzz.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://jui.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://jqc.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://psg.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dzr.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://yif.shzxlz.cn

Ruby: s.count("a")
来源：http://ywg.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://dky.birdmap.top

[E13] 逐字符遍历
来源：http://ygq.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://omo.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ufs.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hkt.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://thf.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pcq.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vki.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gpb.tarul.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jym.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://bcj.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ykj.yfazqb.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://gti.chenzaomai.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dti.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kpm.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rfw.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hmu.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cqc.hcnkem.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ztt.ydzc1.top

[E15] HTML 转义 / 反转义
来源：http://trw.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ppx.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mfw.birdmap.top


<!-- 参考信息 -->