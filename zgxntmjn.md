代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dsw.fengsongda.top

Ruby: arr.sort
来源：http://mdr.havefunace.top

C#:   list.Sort();
来源：http://ras.jinqigfzy.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://gjm.dianchejie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cjv.jianghu66.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cws.yanxiufei.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://qfd.316326.xyz

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://apk.xuanzx.com

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gkk.wangshuangyany.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gbr.bjfxy.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kjp.ydzc1.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dfu.zdqjudy.top

[D11] 反转数组
来源：http://ugy.sufxvd.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wpc.xylfe.cn

PHP:  array_reverse($arr);
来源：http://vhe.xuanzx.com

JS:   [...arr].reverse();  arr.toReversed()
来源：http://brc.shanyushiyangkeji.top

TS:   [...arr].reverse();
来源：http://ibn.ehwqpu.com

Java: Collections.reverse(list);
来源：http://osd.ivvv.top

Go:   slices.Reverse(arr)
来源：http://maf.yj202588.top

Ruby: arr.reverse
来源：http://acy.jyoumei.cn

C#:   list.Reverse();
来源：http://zgj.aibaodan.cn

[D12] 查找元素下标
来源：http://xny.yj20258.top

Py:   arr.index(x);  x in arr
来源：http://jdw.yj20258.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ohb.guannengcc.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fum.xziqi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ggp.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oub.xuetiantiany.cn

Go:   slices.Index(arr, x)
来源：http://bww.xylfe.cn

Ruby: arr.index(x)
来源：http://qrq.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://biy.xuetiantiany.cn

[D13] 过滤（保留满足条件的）
来源：http://koy.xziqi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mgp.jqgfzy.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cvi.jqgfzy.top

JS:   arr.filter(x => x > 3)
来源：http://zcy.bjfxy.top

TS:   arr.filter(x => x > 3)
来源：http://gtq.ybcxt.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wxk.nanxinkj.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lax.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://djm.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://nze.jinghuilouyu.cn

[D14] 映射转换（每个元素变形）
来源：http://obd.iojbl.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kuj.hcnkem.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rsy.ybcxt.top

JS:   arr.map(x => x * 2)
来源：http://kxr.jqgfzy.top

TS:   arr.map(x => x * 2)
来源：http://dxp.nwbrower.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://pfb.zhengqikj.top

Go:   // 手写循环
来源：http://ucq.yj202588.top

Ruby: arr.map { |x| x * 2 }
来源：http://reo.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://bbq.shangyingyoupin.top

[D15] 去重
来源：http://lhb.daxiang520.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gtg.fengsongda.top

PHP:  array_unique($arr);
来源：http://ztb.tianlin.xyz

JS:   [...new Set(arr)]
来源：http://azw.cucudq.cn

TS:   [...new Set(arr)]
来源：http://pcf.svipenyu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://glk.zhongyouzk.top

Go:   // 用 map[T]struct{} 手写
来源：http://kuk.smart0.xyz

Ruby: arr.uniq
来源：http://bnx.xinyue.icu

C#:   list.Distinct().ToList()
来源：http://szt.sxryk.cn

[D16] 求和与平均值
来源：http://rhi.hnxiangtu.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eze.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://air.dianchejie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xol.epnwcf.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://aga.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bzs.cashguo.top

Go:   // 手写循环累加
来源：http://qdx.uphjek.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ijn.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://isz.hongshengwenyu.top

[D17] 最大值与最小值
来源：http://yyn.epnwcf.com

Py:   max(arr);  min(arr)
来源：http://njk.xinyue.icu

PHP:  max($arr);  min($arr);
来源：http://djn.dianchejie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://csj.zhijiandao.cn

TS:   Math.max(...arr);
来源：http://gys.c1oappe.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pnm.nwbrower.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wka.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://mks.yueranfly.top

C#:   list.Max();  list.Min()
来源：http://ukz.epnwcf.com

[D18] 扁平化嵌套数组
来源：http://skr.jinqigfzy.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdo.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://fnx.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://svu.jyoumei.cn

TS:   nested.flat();
来源：http://thl.yvedp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mod.sufxvd.cn

Go:   // 手写双层循环
来源：http://civ.fzhhl.top

Ruby: nested.flatten
来源：http://fnw.yj20258.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://apx.meibo888.top

[D19] 按字段分组
来源：http://tle.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gad.ywan-chungtsiang.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yzg.316326.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wat.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tff.sysykeji.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ygi.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://tqh.sysykeji.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://amd.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tcy.fehbvm.com

[D20] 统计每个元素出现次数
来源：http://yfv.zhiwuduotai.top

Py:   Counter(arr)
来源：http://soy.316326.xyz

PHP:  array_count_values($arr);
来源：http://ort.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vzw.jinyuanbaomall.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lyo.redwolf501.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bxf.cheryme.top

Go:   // 手写 map[T]int
来源：http://vrf.jlsjyb.cn

Ruby: arr.tally
来源：http://cyp.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ugh.ydzc1.top

[D21] 判断是否包含某元素
来源：http://tbs.cqqwz.cn

Py:   x in arr
来源：http://udl.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://mjs.tian-w.cn

JS:   arr.includes(x)
来源：http://hdg.xinyue.icu

TS:   arr.includes(x)
来源：http://chw.wangdashe.top

Java: list.contains(x)
来源：http://kxq.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://ziz.tianlin.xyz

Ruby: arr.include?(x)
来源：http://okm.jiagoushi.top

C#:   list.Contains(x)
来源：http://esc.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://lzr.pycfn.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vos.0kj1m.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kib.tarul.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://iwk.jianghu66.top

TS:   [...arr];
来源：http://hmj.fzhhl.top

Java: new ArrayList<>(list);
来源：http://rlw.shzxlz.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ibl.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://lay.ivvv.top

C#:   new List<int>(list);
来源：http://zmw.haohaochexian.top

[D23] reduce 累积计算
来源：http://kdr.uphjek.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zrk.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qfy.vqdsnc.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cai.xziqi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qzn.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xkn.nwbrower.top

Go:   // 手写循环
来源：http://axs.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rpf.feifeiyinyue.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lnb.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://unt.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pcy.epnwcf.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rlz.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gao.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://efx.quarkkingdee.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ufu.sjlbkw.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xzv.yj20258888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ejo.gzhubu.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nwm.tarul.cn

[D25] Set 集合去重与交并差
来源：http://phr.hysaishi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://txm.shangyingyoupin.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xef.xingfuxueyuan.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://snq.feifeiyinyue.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vkv.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://fiu.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://raq.shangyingyoupin.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ryl.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wri.hywenlv.cn

[D26] 数组转字符串
来源：http://wqz.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://fec.yueranfly.top

PHP:  implode(", ", $arr);
来源：http://lde.cucudq.cn

JS:   arr.join(", ")
来源：http://gji.zhongyouzk.top

TS:   arr.join(", ")
来源：http://iln.bbcook.cn

Java: String.join(", ", list)
来源：http://vof.yongpay.top

Go:   strings.Join(strs, ", ")
来源：http://ynm.jiagoushi.top

Ruby: arr.join(", ")
来源：http://wyj.wangshuangyany.cn

C#:   string.Join(", ", list)
来源：http://omx.yanxiufei.cn

================================================================================
来源：http://ulz.0kj1m.cn

E. 字符串处理
来源：http://fsi.guannengcc.top

================================================================================
来源：http://iuj.chenzaomai.com

[E01] 拼接字符串
来源：http://ufv.hfpthk.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dyy.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lzp.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lnp.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fyr.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ylg.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gdu.sweek.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xma.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kal.daria6918.cn

[E02] 重复字符串
来源：http://ayj.xinyue.icu

Py:   "ab" * 3
来源：http://aje.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://arm.gzhubu.top

JS:   "ab".repeat(3)
来源：http://blm.nanxinkj.top

TS:   "ab".repeat(3)
来源：http://etd.iojbl.cn

Java: "ab".repeat(3)
来源：http://yud.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://qkn.sjlbkw.cn

Ruby: "ab" * 3
来源：http://qnn.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xbn.ehwqpu.com

[E03] 截取子串
来源：http://fas.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bwy.xylfe.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sta.jyoumei.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ebw.zhoulong.xyz

TS:   s.slice(1, 4)
来源：http://ydb.yanxiufei.cn

Java: s.substring(1, 4)
来源：http://ary.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yaj.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://kow.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://lzd.dianchejie.cn

[E04] 查找子串位置
来源：http://oqz.jinqigfzy.top

Py:   s.find("x");  s.index("x")
来源：http://rok.tarul.cn

PHP:  strpos($s, "x");
来源：http://sse.uphjek.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://eqo.bbcook.cn

TS:   s.indexOf("x")
来源：http://tqv.wangshuangyany.cn

Java: s.indexOf("x")
来源：http://obf.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://veu.nwbrower.top

Ruby: s.index("x")
来源：http://hxt.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://wef.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://cuk.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vkz.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pfi.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://syy.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vqy.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ozk.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bwb.sufxvd.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tiy.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vca.tanke756.top

[E06] 替换子串
来源：http://koc.jinqigfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fwi.snrcjt.cn

PHP:  str_replace("a", "b", $s);
来源：http://qog.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://miw.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://moc.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xng.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tzs.nanxuanxn.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eez.jinyuanbaomall.cn

C#:   s.Replace("a", "b")
来源：http://tlo.gogol.net.cn

[E07] 按分隔符拆分
来源：http://sgo.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hiu.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aat.svipenyu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bby.yueranfly.top

TS:   s.split(",")
来源：http://jre.jlsjyb.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gqz.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rwd.zhoulong.xyz

Ruby: s.split(",");  s.split
来源：http://pdf.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pek.hnxiangtu.top

[E08] 数组按分隔符合并
来源：http://wlz.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://yfo.xziqi.cn

PHP:  implode(",", $items);
来源：http://lvy.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://gpb.yangfankeji.com

TS:   items.join(",")
来源：http://efi.yj20258888.top

Java: String.join(",", items)
来源：http://sjh.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://sxw.dianchejie.cn

Ruby: items.join(",")
来源：http://pnl.zhixingplan.top

C#:   string.Join(",", items)
来源：http://wcd.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://wgv.gaohongyu789.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mzf.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jrh.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://lyv.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://fxw.52xcode.cn

Java: s.replaceAll("\\s+", "")
来源：http://wtz.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fac.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wcg.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tqc.andypj.xyz

[E10] 左侧补零 / 定长填充
来源：http://gzh.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wtg.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lyt.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://xzk.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://hzk.cheryme.top

Java: String.format("%03d", 7)
来源：http://ktn.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nse.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kta.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bbs.ybcxt.top

[E11] 反转字符串
来源：http://cge.hammf.cn

Py:   s[::-1]
来源：http://wnr.hammf.cn

PHP:  strrev($s);
来源：http://itg.nanxinkj.top

JS:   [...s].reverse().join("")
来源：http://tah.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://ora.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aio.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://efd.zycfv.cn

Ruby: s.reverse
来源：http://osg.yuanzhike.top

C#:   new string(s.Reverse().ToArray())
来源：http://kcr.ydzc1.top

[E12] 统计某字符出现次数
来源：http://lvi.svipenyu.cn

Py:   s.count("a")
来源：http://ogu.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://cvc.guannengcc.top

JS:   s.split("a").length - 1
来源：http://nck.guannengcc.top

TS:   s.split("a").length - 1
来源：http://fqb.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vgz.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://vsa.epnwcf.com

Ruby: s.count("a")
来源：http://ujx.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://bkb.cqqwz.cn

[E13] 逐字符遍历
来源：http://znx.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://lvf.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tbr.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://aav.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fxc.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cyo.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dqt.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xab.sjlbkw.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xly.yj20258.top

[E14] URL 编码与 Base64
来源：http://qvx.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xui.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dlk.316326.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jej.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ygk.aizwys.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xae.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://did.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lbb.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vte.yonumen.top

[E15] HTML 转义 / 反转义
来源：http://ozg.zhiwuduotai.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vrf.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uyv.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wpc.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qzb.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://roc.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oke.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://waw.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ypg.zhengqikj.top

[E16] 数字千分位
来源：http://daa.sysykeji.top

Py:   f"{1234567:,}"
来源：http://eie.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://pdx.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://efx.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zhz.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ouj.mhx1999.top


<!-- 参考信息 -->