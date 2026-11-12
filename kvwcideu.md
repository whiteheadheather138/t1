代发 wailian999

Py:   len(arr)
来源：http://naw.smart0.xyz

PHP:  count($arr);
来源：http://boy.sufxvd.cn

JS:   arr.length
来源：http://afw.bbcook.cn

TS:   arr.length
来源：http://yzw.gotoacloud.top

Java: list.size();
来源：http://tcv.kuanghao11.cn

Go:   len(arr)
来源：http://jpe.wangdashe.top

Ruby: arr.length; arr.size
来源：http://wgp.snrcjt.cn

C#:   list.Count;
来源：http://wut.jianghu66.top

[D07] 切片 / 取子数组
来源：http://ioq.dianchejie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gpd.zhoulong.xyz

PHP:  array_slice($arr, 1, 3);
来源：http://rov.feifeiyinyue.top

JS:   arr.slice(1, 4);
来源：http://sfr.cqqwz.cn

TS:   arr.slice(1, 4);
来源：http://byb.guannengcc.top

Java: list.subList(1, 4);
来源：http://mly.316326.xyz

Go:   arr[1:4]
来源：http://uyu.tian-w.cn

Ruby: arr[1, 3]
来源：http://ajz.bjfxy.top

C#:   list.GetRange(1, 3);
来源：http://tfy.yongpay.top

[D08] 合并两个数组
来源：http://sim.svipenyu.cn

Py:   a + b;  a.extend(b)
来源：http://jen.iojbl.cn

PHP:  array_merge($a, $b);
来源：http://xnz.yanxiufei.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rkf.gogol.net.cn

TS:   [...a, ...b];
来源：http://oke.cqqwz.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ask.xziqi.cn

Go:   append(a, b...)
来源：http://uly.iojbl.cn

Ruby: a + b;  a.concat(b)
来源：http://ljq.tanke756.top

C#:   a.Concat(b).ToList()
来源：http://ykc.snrcjt.cn

[D09] 排序（升序）
来源：http://mzs.jianghu66.top

Py:   sorted(arr);  arr.sort()
来源：http://xcw.xuetiantiany.cn

PHP:  sort($arr);
来源：http://uwy.gogol.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ooy.sjlbkw.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fdm.redwolf501.top

Java: Collections.sort(list);  list.sort(null);
来源：http://nmz.cashguo.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tup.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://lao.shangyingyoupin.top

C#:   list.Sort();
来源：http://aiv.316326.xyz

[D10] 自定义排序（按字段 / 多条件）
来源：http://zdz.ydjk.org.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tnh.hammf.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://flt.yj20258888.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://biu.jyoumei.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://njt.ydjk.org.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ikf.guannengcc.top

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uij.xuetiantiany.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hfs.zycfv.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mde.wangdashe.top

[D11] 反转数组
来源：http://sli.gaohongyu789.top

Py:   arr[::-1];  arr.reverse()
来源：http://ymj.hcnkem.com

PHP:  array_reverse($arr);
来源：http://mtv.yj20258888.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://isj.jlsjyb.cn

TS:   [...arr].reverse();
来源：http://mfh.nanxuanxn.top

Java: Collections.reverse(list);
来源：http://djf.mhx1999.top

Go:   slices.Reverse(arr)
来源：http://mak.tanke756.top

Ruby: arr.reverse
来源：http://uwa.zdqjudy.top

C#:   list.Reverse();
来源：http://ktn.aibaodan.cn

[D12] 查找元素下标
来源：http://fwh.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://zod.chenzaomai.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qrm.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qmr.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jfd.zhiwuduotai.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uwp.quarkkingdee.top

Go:   slices.Index(arr, x)
来源：http://csq.cdnleiting.top

Ruby: arr.index(x)
来源：http://mhi.fehbvm.com

C#:   list.IndexOf(x);
来源：http://ifc.nanxuanxn.top

[D13] 过滤（保留满足条件的）
来源：http://tzh.xylfe.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://feh.birdmap.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wej.jianghu66.top

JS:   arr.filter(x => x > 3)
来源：http://tci.chenlongwang.top

TS:   arr.filter(x => x > 3)
来源：http://ncl.0kj1m.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zei.9152youxi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gbe.birdmap.top

Ruby: arr.select { |x| x > 3 }
来源：http://xvz.9152youxi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vac.vqdsnc.cn

[D14] 映射转换（每个元素变形）
来源：http://twm.shanyushiyangtech.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cve.dianchejie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mnf.pengpengdd.cyou

JS:   arr.map(x => x * 2)
来源：http://ktq.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://afj.shzxlz.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nnf.yvedp.cn

Go:   // 手写循环
来源：http://yku.gzhubu.top

Ruby: arr.map { |x| x * 2 }
来源：http://tfy.birdmap.top

C#:   list.Select(x => x * 2).ToList()
来源：http://vyf.cheryme.top

[D15] 去重
来源：http://yzw.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ibl.yueranfly.top

PHP:  array_unique($arr);
来源：http://pvo.ppjwa.cn

JS:   [...new Set(arr)]
来源：http://hiv.zdbjq.cn

TS:   [...new Set(arr)]
来源：http://xml.meibo888.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ofn.hesvh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ake.hywenlv.cn

Ruby: arr.uniq
来源：http://ukv.bjfxy.top

C#:   list.Distinct().ToList()
来源：http://ipd.pycfn.com

[D16] 求和与平均值
来源：http://qcq.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://psv.jqgfzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yhf.hcnkem.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://sme.wangdashe.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mph.hywenlv.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ctq.nanxuanxn.top

Go:   // 手写循环累加
来源：http://ike.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vrl.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://geq.sxryk.cn

[D17] 最大值与最小值
来源：http://lvt.xuetiantiany.cn

Py:   max(arr);  min(arr)
来源：http://lxf.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://koz.chenlongwang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oen.yvedp.cn

TS:   Math.max(...arr);
来源：http://vwx.hysaishi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ubl.ydzc1.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rjz.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://kya.gogol.net.cn

C#:   list.Max();  list.Min()
来源：http://wcu.ydjk.org.cn

[D18] 扁平化嵌套数组
来源：http://kmr.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wrl.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://xwf.hongshengwenyu.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hbk.sjlbkw.cn

TS:   nested.flat();
来源：http://yoh.fzhhl.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zif.xziqi.cn

Go:   // 手写双层循环
来源：http://vpc.zhaomingkeji.xyz

Ruby: nested.flatten
来源：http://hvi.yfazqb.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://nst.pengpengdd.cyou

[D19] 按字段分组
来源：http://odu.zdbjq.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://omn.hammf.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pxa.hywenlv.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vli.daxiang520.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://aum.cdnleiting.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lan.zhijiandao.cn

Go:   // 手写 map[string][]T
来源：http://mba.jinyuanbaomall.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kda.yuxming.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dow.zhiwuduotai.top

[D20] 统计每个元素出现次数
来源：http://bii.zhoulong.xyz

Py:   Counter(arr)
来源：http://yel.yueranfly.top

PHP:  array_count_values($arr);
来源：http://kqq.hysaishi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gko.yfazqb.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wiy.316326.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sqo.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://edr.zycfv.cn

Ruby: arr.tally
来源：http://bnv.zhaomingkeji.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zsk.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://sii.gotoacloud.top

Py:   x in arr
来源：http://byj.hcnkem.com

PHP:  in_array($x, $arr, true);
来源：http://owx.feifeiyinyue.top

JS:   arr.includes(x)
来源：http://kiw.zhaomingkeji.xyz

TS:   arr.includes(x)
来源：http://xqq.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://ssy.0kj1m.cn

Go:   slices.Contains(arr, x)
来源：http://qyp.ctjpmb.com

Ruby: arr.include?(x)
来源：http://rvd.meibo888.top

C#:   list.Contains(x)
来源：http://dir.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://ftc.xylfe.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dbv.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gvu.yj202588.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zem.hcnkem.com

TS:   [...arr];
来源：http://tzn.nanxuanxn.top

Java: new ArrayList<>(list);
来源：http://fcg.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tga.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://urr.xinyue.icu

C#:   new List<int>(list);
来源：http://utr.sysykeji.top

[D23] reduce 累积计算
来源：http://rzr.quarkkingdee.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vwc.pycfn.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mdy.ybcxt.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sbf.sysykeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lbn.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gmk.kuanghao11.cn

Go:   // 手写循环
来源：http://mpq.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kpj.dashuyun.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ude.ydjk.org.cn

[D24] 字典 / Map 基本操作
来源：http://cmz.jqgfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uwz.svipenyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jhu.dashuyun.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ypk.yfazqb.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yfj.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lhl.tarul.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vub.sufxvd.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jhk.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tde.zdqjudy.top

[D25] Set 集合去重与交并差
来源：http://thd.9152youxi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iiw.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rlw.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://chn.ctjpmb.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iui.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xat.yanxiufei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xut.gzhubu.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xli.ehwqpu.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xib.hammf.cn

[D26] 数组转字符串
来源：http://tdt.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://tjh.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://wpy.chenjidiqi.icu

JS:   arr.join(", ")
来源：http://vzj.ywan-chungtsiang.top

TS:   arr.join(", ")
来源：http://mwr.fehbvm.com

Java: String.join(", ", list)
来源：http://ofg.c1oappe.top

Go:   strings.Join(strs, ", ")
来源：http://wwn.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://nvp.sweek.top

C#:   string.Join(", ", list)
来源：http://nsy.ehwqpu.com

================================================================================
来源：http://hgs.zhoulong.xyz

E. 字符串处理
来源：http://qtx.jqgfzy.top

================================================================================
来源：http://yoy.birdmap.top

[E01] 拼接字符串
来源：http://ztz.nanxuanxn.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rzk.jinqigufen.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gnb.cqqwz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pyg.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kgb.redwolf501.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lzq.xuanzx.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oji.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wex.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://map.fktsv.cn

[E02] 重复字符串
来源：http://tyj.jinqigufen.top

Py:   "ab" * 3
来源：http://ygu.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://gac.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://ejr.hcnkem.com

TS:   "ab".repeat(3)
来源：http://yja.guowangkeji.top

Java: "ab".repeat(3)
来源：http://mll.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://beg.mhx1999.top

Ruby: "ab" * 3
来源：http://agg.shanyushiyangtech.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rsc.yj202588.top

[E03] 截取子串
来源：http://uza.316326.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://iai.vqdsnc.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vsq.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://atx.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://yxg.yuxming.cn

Java: s.substring(1, 4)
来源：http://awq.zhoulong.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dro.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://awq.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://zaq.fktsv.cn

[E04] 查找子串位置
来源：http://tjs.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://ihv.yueranfly.top

PHP:  strpos($s, "x");
来源：http://njv.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aam.xuetiantiany.cn

TS:   s.indexOf("x")
来源：http://xys.mhx1999.top

Java: s.indexOf("x")
来源：http://ilk.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://xjf.jianghu66.top

Ruby: s.index("x")
来源：http://zdt.bjfxy.top

C#:   s.IndexOf("x")
来源：http://mor.yueranfly.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mij.yonumen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vnv.cashguo.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bjz.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://naq.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://hsi.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jso.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://stu.shuidangran.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://frx.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fhg.kuanghao11.cn

[E06] 替换子串
来源：http://idg.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nmb.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://llr.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cjj.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://gwm.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hps.nanxinkj.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rsi.hnqzz.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kvb.daxiang520.top

C#:   s.Replace("a", "b")
来源：http://xlh.haohaochexian.top

[E07] 按分隔符拆分
来源：http://kgz.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hnz.wangshuangyany.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://edb.zhaomingkeji.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://pft.shanyushiyangkeji.top

TS:   s.split(",")
来源：http://itk.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pqo.xuanzx.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://flj.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://rha.zycfv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jhh.zycfv.cn

[E08] 数组按分隔符合并
来源：http://qlc.nwbrower.top

Py:   ",".join(items)
来源：http://plr.yj20258.top

PHP:  implode(",", $items);
来源：http://qfz.zhijiandao.cn

JS:   items.join(",")
来源：http://arp.hfpthk.cn

TS:   items.join(",")
来源：http://jtg.52xcode.cn

Java: String.join(",", items)
来源：http://rre.gotoacloud.top

Go:   strings.Join(items, ",")
来源：http://hml.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://qhj.hysaishi.cn

C#:   string.Join(",", items)
来源：http://phi.hysaishi.cn

[E09] 去除所有空白字符
来源：http://ocw.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://len.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dzd.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://vws.52xcode.cn

TS:   s.replace(/\s+/g, "")
来源：http://dvx.guannengcc.top

Java: s.replaceAll("\\s+", "")
来源：http://dos.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vep.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://uso.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqe.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://tth.zhengqikj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uoj.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jvn.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://tgr.jinghuilouyu.cn

TS:   "7".padStart(3, "0")
来源：http://dhi.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://qyf.jinqigfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tph.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tzp.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://spm.aizwys.cn

[E11] 反转字符串
来源：http://mye.fengsongda.top

Py:   s[::-1]
来源：http://gcz.kuanghao11.cn

PHP:  strrev($s);
来源：http://acx.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://gfg.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://bfj.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bda.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fwo.guannengcc.top

Ruby: s.reverse
来源：http://sfc.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://oob.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://uxz.shzxlz.cn

Py:   s.count("a")
来源：http://lom.c1oappe.top

PHP:  substr_count($s, "a");
来源：http://ecu.nwbrower.top

JS:   s.split("a").length - 1
来源：http://jdc.zycfv.cn

TS:   s.split("a").length - 1
来源：http://erd.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wzp.yj20258.top

Go:   strings.Count(s, "a")
来源：http://uby.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://ypc.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://dth.daria6918.cn

[E13] 逐字符遍历
来源：http://aen.aibaodan.cn


<!-- 参考信息 -->