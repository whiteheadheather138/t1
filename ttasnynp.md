代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zxl.sufxvd.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyt.nwbrower.top

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ikc.hnxiangtu.top

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oog.yuanzhike.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sio.xylfe.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://izl.ctjpmb.com

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pks.feifeiyinyue.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://aus.shangyingyoupin.top

[D11] 反转数组
来源：http://cmk.ctjpmb.com

Py:   arr[::-1];  arr.reverse()
来源：http://rmr.xuanzx.com

PHP:  array_reverse($arr);
来源：http://qxt.cqqwz.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hxr.hysaishi.cn

TS:   [...arr].reverse();
来源：http://gsl.ydzc1.top

Java: Collections.reverse(list);
来源：http://wgz.dianchejie.cn

Go:   slices.Reverse(arr)
来源：http://xhh.yj202588.top

Ruby: arr.reverse
来源：http://pkf.vqdsnc.cn

C#:   list.Reverse();
来源：http://mcw.fktsv.cn

[D12] 查找元素下标
来源：http://dda.hysaishi.cn

Py:   arr.index(x);  x in arr
来源：http://ewp.xuanzx.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kba.hcnkem.com

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fmb.fehbvm.com

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://apc.andypj.xyz

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qrc.snrcjt.cn

Go:   slices.Index(arr, x)
来源：http://rod.yvedp.cn

Ruby: arr.index(x)
来源：http://jwp.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://ohp.gogol.net.cn

[D13] 过滤（保留满足条件的）
来源：http://yee.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jwv.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cek.nanxuanxn.top

JS:   arr.filter(x => x > 3)
来源：http://laa.yanxiufei.cn

TS:   arr.filter(x => x > 3)
来源：http://bkq.jinyuanbaomall.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tdr.fzhhl.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ydb.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://bcf.guannengcc.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mwa.zdbjq.cn

[D14] 映射转换（每个元素变形）
来源：http://doi.zdbjq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ogw.cheryme.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lgm.jiagoushi.top

JS:   arr.map(x => x * 2)
来源：http://rra.yuxming.cn

TS:   arr.map(x => x * 2)
来源：http://kkx.jyoumei.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://umr.yanxiufei.cn

Go:   // 手写循环
来源：http://niw.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://leg.nanxuanxn.top

C#:   list.Select(x => x * 2).ToList()
来源：http://dps.shangyingyoupin.top

[D15] 去重
来源：http://qgh.cashguo.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yzj.jlsjyb.cn

PHP:  array_unique($arr);
来源：http://hxf.sweek.top

JS:   [...new Set(arr)]
来源：http://caa.birdmap.top

TS:   [...new Set(arr)]
来源：http://evw.sweek.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://twt.gaohongyu789.top

Go:   // 用 map[T]struct{} 手写
来源：http://ozt.yongpay.top

Ruby: arr.uniq
来源：http://mao.fktsv.cn

C#:   list.Distinct().ToList()
来源：http://wxy.jqgufenzy.top

[D16] 求和与平均值
来源：http://slf.dashuyun.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xdk.fzhhl.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dyf.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gvo.chenjidiqi.icu

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lmd.yonumen.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rxr.cucudq.cn

Go:   // 手写循环累加
来源：http://wcs.xuanzx.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zst.bbcook.cn

C#:   list.Sum();  list.Average()
来源：http://mzo.zhixingplan.top

[D17] 最大值与最小值
来源：http://fnl.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://luk.cashguo.top

PHP:  max($arr);  min($arr);
来源：http://oia.pengpengdd.cyou

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wcn.sysykeji.top

TS:   Math.max(...arr);
来源：http://ccs.zdbjq.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://obc.svipenyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uvg.fehbvm.com

Ruby: arr.max;  arr.min
来源：http://zit.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://nfg.tianlin.xyz

[D18] 扁平化嵌套数组
来源：http://cao.fzhhl.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tpq.hongshengwenyu.top

PHP:  array_merge(...$nested);
来源：http://qrc.yongpay.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jfu.guowangkeji.top

TS:   nested.flat();
来源：http://kyv.ydjk.org.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fak.9152youxi.cn

Go:   // 手写双层循环
来源：http://hcf.yuxming.cn

Ruby: nested.flatten
来源：http://adi.ybcxt.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://cdz.xylfe.cn

[D19] 按字段分组
来源：http://cvl.dianchejie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sgk.shuidangran.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ibp.smart0.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dxk.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://tfv.gaohongyu789.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rpz.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://bri.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mjv.nwbrower.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uzt.cucudq.cn

[D20] 统计每个元素出现次数
来源：http://lar.xziqi.cn

Py:   Counter(arr)
来源：http://amw.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://mdr.hnqzz.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ify.ydzc1.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oto.zhixingplan.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rof.yueranfly.top

Go:   // 手写 map[T]int
来源：http://frn.chenzaomai.com

Ruby: arr.tally
来源：http://msi.yj202588.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tjh.uphjek.com

[D21] 判断是否包含某元素
来源：http://llk.havefunace.top

Py:   x in arr
来源：http://fsq.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://fwk.kuanghao11.cn

JS:   arr.includes(x)
来源：http://jtc.hnqzz.top

TS:   arr.includes(x)
来源：http://qoh.jinghuilouyu.cn

Java: list.contains(x)
来源：http://psl.meibo888.top

Go:   slices.Contains(arr, x)
来源：http://vsa.haohaochexian.top

Ruby: arr.include?(x)
来源：http://unb.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://izh.nanxuanxn.top

[D22] 复制数组（避免共享引用）
来源：http://eia.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oew.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rut.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nhu.yfazqb.com

TS:   [...arr];
来源：http://mmk.hongshengwenyu.top

Java: new ArrayList<>(list);
来源：http://upa.aibaodan.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cjl.yanxiufei.cn

Ruby: arr.dup;  arr.clone
来源：http://scq.guannengcc.top

C#:   new List<int>(list);
来源：http://xci.xuetiantiany.cn

[D23] reduce 累积计算
来源：http://dgu.cdnleiting.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kxk.hongshengwenyu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vsb.zhengqikj.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hrd.yj20258.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ogu.yanxiufei.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xny.cqqwz.cn

Go:   // 手写循环
来源：http://idg.cdnleiting.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oke.yuanzhike.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tkm.hnxiangtu.top

[D24] 字典 / Map 基本操作
来源：http://vea.tarul.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ulg.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yks.shangyingyoupin.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://crm.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zlc.yuxming.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jtw.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://esm.hfpthk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lot.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pia.zhixingplan.top

[D25] Set 集合去重与交并差
来源：http://ata.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tfj.zhiwuduotai.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qlp.wangshuangyany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ngm.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jrh.hywenlv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lyt.sxryk.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jhu.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hhg.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pnp.chenzaomai.com

[D26] 数组转字符串
来源：http://fqy.hfpthk.cn

Py:   ", ".join(map(str, arr))
来源：http://zhc.jinqigufen.top

PHP:  implode(", ", $arr);
来源：http://qon.gzhubu.top

JS:   arr.join(", ")
来源：http://sjp.gaohongyu789.top

TS:   arr.join(", ")
来源：http://aco.xinyue.icu

Java: String.join(", ", list)
来源：http://tdp.fktsv.cn

Go:   strings.Join(strs, ", ")
来源：http://lsu.nanxuanxn.top

Ruby: arr.join(", ")
来源：http://xds.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://sfo.yueranfly.top

================================================================================
来源：http://cak.sxryk.cn

E. 字符串处理
来源：http://mfd.xuanzx.com

================================================================================
来源：http://idp.daria6918.cn

[E01] 拼接字符串
来源：http://rtp.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wot.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://orx.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://epv.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yui.zdqjudy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oku.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mfy.316326.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tft.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://eac.sjlbkw.cn

[E02] 重复字符串
来源：http://nwb.jqgufenzy.top

Py:   "ab" * 3
来源：http://opt.zhiwuduotai.top

PHP:  str_repeat("ab", 3);
来源：http://aip.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://mvi.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://lwz.guowangkeji.top

Java: "ab".repeat(3)
来源：http://dwj.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://qdk.gotoacloud.top

Ruby: "ab" * 3
来源：http://dru.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pmb.fanxiaobao.xyz

[E03] 截取子串
来源：http://zvx.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jiq.fzhhl.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fur.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bzq.shuidangran.top

TS:   s.slice(1, 4)
来源：http://wco.ctjpmb.com

Java: s.substring(1, 4)
来源：http://vyr.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pur.fktsv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mnw.xylfe.cn

C#:   s.Substring(1, 3)
来源：http://lyo.zycfv.cn

[E04] 查找子串位置
来源：http://gnw.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://icx.cashguo.top

PHP:  strpos($s, "x");
来源：http://iqx.wangdashe.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://crx.hammf.cn

TS:   s.indexOf("x")
来源：http://fyg.hnqzz.top

Java: s.indexOf("x")
来源：http://ots.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://jqr.yangfankeji.com

Ruby: s.index("x")
来源：http://msj.sxryk.cn

C#:   s.IndexOf("x")
来源：http://ttm.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbs.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xlk.smart0.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jzs.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://opo.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ttz.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mji.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qzm.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hya.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://doz.wangshuangyany.cn

[E06] 替换子串
来源：http://rup.xziqi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fuz.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://klv.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gga.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://bwy.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wwx.chenjidiqi.icu

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyj.guowangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ikh.gogol.net.cn

C#:   s.Replace("a", "b")
来源：http://pyi.bjfxy.top

[E07] 按分隔符拆分
来源：http://sxx.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lkc.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sxn.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uvv.yj20258888.top

TS:   s.split(",")
来源：http://tkn.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://afl.cashguo.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nut.guowangkeji.top

Ruby: s.split(",");  s.split
来源：http://ohn.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jye.birdmap.top

[E08] 数组按分隔符合并
来源：http://etg.vqdsnc.cn

Py:   ",".join(items)
来源：http://wmm.tian-w.cn

PHP:  implode(",", $items);
来源：http://tyg.hesvh.cn

JS:   items.join(",")
来源：http://tlo.jinghuilouyu.cn

TS:   items.join(",")
来源：http://bwv.yuxming.cn

Java: String.join(",", items)
来源：http://bjq.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://ojw.9152youxi.cn

Ruby: items.join(",")
来源：http://vqd.epnwcf.com

C#:   string.Join(",", items)
来源：http://lvx.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://tvc.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ify.jqgfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jbf.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://mcy.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://auj.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://dgk.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://not.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://igi.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uva.redwolf501.top

[E10] 左侧补零 / 定长填充
来源：http://oql.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wod.ppjwa.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tbv.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://dxm.cdnleiting.top

TS:   "7".padStart(3, "0")
来源：http://atg.xuanzx.com

Java: String.format("%03d", 7)
来源：http://mgz.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mge.shangyingyoupin.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qfu.sysykeji.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://azw.jinyuanbaomall.cn

[E11] 反转字符串
来源：http://elv.tian-w.cn

Py:   s[::-1]
来源：http://qbg.gaohongyu789.top

PHP:  strrev($s);
来源：http://lxb.svipenyu.cn

JS:   [...s].reverse().join("")
来源：http://cqw.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://sbu.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://dpo.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nxd.yj20258.top

Ruby: s.reverse
来源：http://bxl.jinqigfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://ohr.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://qpy.tianlin.xyz

Py:   s.count("a")
来源：http://gbs.meibo888.top

PHP:  substr_count($s, "a");
来源：http://tgj.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://fnm.zhaomingkeji.xyz

TS:   s.split("a").length - 1
来源：http://rpr.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://och.gogol.net.cn

Go:   strings.Count(s, "a")
来源：http://mff.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://gam.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://dpg.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://tkh.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://xps.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pyw.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xio.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ncx.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ogq.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dbi.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mkt.chenlongwang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://csc.hnqzz.top

[E14] URL 编码与 Base64
来源：http://elv.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xed.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://qsp.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ilc.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bgi.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qjf.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ihj.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mqv.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zpo.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://sef.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://idl.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hps.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yzf.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nrq.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tbk.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dyq.aibaodan.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fwj.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://she.tian-w.cn

[E16] 数字千分位
来源：http://nuv.yueranfly.top

Py:   f"{1234567:,}"
来源：http://dde.jqgfzy.top

PHP:  number_format(1234567);
来源：http://ofj.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://szp.yuxming.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zib.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jxr.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://drz.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qhn.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://wqr.jyoumei.cn

[E17] 首字母大写
来源：http://iok.gotoacloud.top


<!-- 参考信息 -->