代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hrd.jqgfzy.top

Java: list.subList(1, 4);
来源：http://qqj.aizwys.cn

Go:   arr[1:4]
来源：http://ngn.c1oappe.top

Ruby: arr[1, 3]
来源：http://zac.hnxiangtu.top

C#:   list.GetRange(1, 3);
来源：http://rtw.shuidangran.top

[D08] 合并两个数组
来源：http://eni.yanxiufei.cn

Py:   a + b;  a.extend(b)
来源：http://xaf.meibo888.top

PHP:  array_merge($a, $b);
来源：http://taf.bbcook.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://obt.chenlongwang.top

TS:   [...a, ...b];
来源：http://mxn.hnqzz.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dyq.yj20258.top

Go:   append(a, b...)
来源：http://bus.cheryme.top

Ruby: a + b;  a.concat(b)
来源：http://job.guannengcc.top

C#:   a.Concat(b).ToList()
来源：http://brq.guowangkeji.top

[D09] 排序（升序）
来源：http://bnp.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://sbn.xuanzx.com

PHP:  sort($arr);
来源：http://omz.aibaodan.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pku.jinghuilouyu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://exc.aizwys.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://frs.ivvv.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://riu.mhx1999.top

Ruby: arr.sort
来源：http://itw.fehbvm.com

C#:   list.Sort();
来源：http://dru.zdbjq.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jdu.aibaodan.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cmo.zhiwuduotai.top

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://owa.iojbl.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://jpe.snrcjt.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://txw.yj202588.top

Java: list.sort(Comparator.comparing(Person::age));
来源：http://txv.uphjek.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vux.daxiang520.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://jsx.fzhhl.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gqa.smart0.xyz

[D11] 反转数组
来源：http://zei.bbcook.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lyz.fehbvm.com

PHP:  array_reverse($arr);
来源：http://mwe.yj202588.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dbl.dashuyun.cn

TS:   [...arr].reverse();
来源：http://ygu.zdbjq.cn

Java: Collections.reverse(list);
来源：http://vvn.zhiwuduotai.top

Go:   slices.Reverse(arr)
来源：http://wah.hnxiangtu.top

Ruby: arr.reverse
来源：http://tai.snrcjt.cn

C#:   list.Reverse();
来源：http://upt.xingfuxueyuan.xyz

[D12] 查找元素下标
来源：http://crc.cashguo.top

Py:   arr.index(x);  x in arr
来源：http://twc.guowangkeji.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://myj.ybcxt.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pmo.yanxiufei.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bui.haohaochexian.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wyi.xingfuxueyuan.xyz

Go:   slices.Index(arr, x)
来源：http://fud.guannengcc.top

Ruby: arr.index(x)
来源：http://typ.tian-w.cn

C#:   list.IndexOf(x);
来源：http://kgk.cdnleiting.top

[D13] 过滤（保留满足条件的）
来源：http://tpj.jinyuanbaomall.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pai.tian-w.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tsr.daria6918.cn

JS:   arr.filter(x => x > 3)
来源：http://hfn.mhx1999.top

TS:   arr.filter(x => x > 3)
来源：http://rpr.xuanzx.com

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jsh.kuanghao11.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qhc.yuanzhike.top

Ruby: arr.select { |x| x > 3 }
来源：http://vnw.yueranfly.top

C#:   list.Where(x => x > 3).ToList()
来源：http://iix.hysaishi.cn

[D14] 映射转换（每个元素变形）
来源：http://wtu.yangfankeji.com

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://edg.gotoacloud.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lsg.yj20258.top

JS:   arr.map(x => x * 2)
来源：http://gei.iojbl.cn

TS:   arr.map(x => x * 2)
来源：http://yud.shuidangran.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://vum.hnqzz.top

Go:   // 手写循环
来源：http://dqz.hywenlv.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jde.tianlin.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://zwt.fzhhl.top

[D15] 去重
来源：http://ztr.mhx1999.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qnl.zhixingplan.top

PHP:  array_unique($arr);
来源：http://tem.nwbrower.top

JS:   [...new Set(arr)]
来源：http://hlg.xziqi.cn

TS:   [...new Set(arr)]
来源：http://omj.birdmap.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://nay.shanyushiyangkeji.top

Go:   // 用 map[T]struct{} 手写
来源：http://iun.gogol.net.cn

Ruby: arr.uniq
来源：http://ikz.yj20258.top

C#:   list.Distinct().ToList()
来源：http://kdc.nanxuanxn.top

[D16] 求和与平均值
来源：http://ktf.sysykeji.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nxh.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ozj.tian-w.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yvi.vehdjk.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://shh.havefunace.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hbf.fanxiaobao.xyz

Go:   // 手写循环累加
来源：http://imo.ydzc1.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vvb.jyoumei.cn

C#:   list.Sum();  list.Average()
来源：http://ydg.zycfv.cn

[D17] 最大值与最小值
来源：http://qgv.gzhubu.top

Py:   max(arr);  min(arr)
来源：http://ddy.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://tha.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jbf.0kj1m.cn

TS:   Math.max(...arr);
来源：http://zer.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://upx.ybcxt.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mnm.redwolf501.top

Ruby: arr.max;  arr.min
来源：http://rri.iojbl.cn

C#:   list.Max();  list.Min()
来源：http://igy.chenzaomai.com

[D18] 扁平化嵌套数组
来源：http://lpo.xziqi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pxi.pengpengdd.cyou

PHP:  array_merge(...$nested);
来源：http://bvq.jlsjyb.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wgk.zhaomingkeji.xyz

TS:   nested.flat();
来源：http://axp.jqgfzy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vas.cucudq.cn

Go:   // 手写双层循环
来源：http://zrz.9152youxi.cn

Ruby: nested.flatten
来源：http://mli.uphjek.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://mow.ppjwa.cn

[D19] 按字段分组
来源：http://qwn.shuidangran.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zba.cqqwz.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wze.snrcjt.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dep.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ppk.52xcode.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yhg.iojbl.cn

Go:   // 手写 map[string][]T
来源：http://ygs.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://did.andypj.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://isf.yj20258.top

[D20] 统计每个元素出现次数
来源：http://qye.feifeiyinyue.top

Py:   Counter(arr)
来源：http://vny.fengsongda.top

PHP:  array_count_values($arr);
来源：http://xqb.aizwys.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kui.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyo.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iza.yongpay.top

Go:   // 手写 map[T]int
来源：http://oah.xuanzx.com

Ruby: arr.tally
来源：http://bak.haohaochexian.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://smg.zhixingplan.top

[D21] 判断是否包含某元素
来源：http://gfd.zdbjq.cn

Py:   x in arr
来源：http://cwb.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://row.tarul.cn

JS:   arr.includes(x)
来源：http://hri.yvedp.cn

TS:   arr.includes(x)
来源：http://vox.cqqwz.cn

Java: list.contains(x)
来源：http://mss.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://rpb.hongshengwenyu.top

Ruby: arr.include?(x)
来源：http://mbz.jyoumei.cn

C#:   list.Contains(x)
来源：http://hut.tian-w.cn

[D22] 复制数组（避免共享引用）
来源：http://biy.pengpengdd.cyou

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rdj.zhiwuduotai.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nxb.ehwqpu.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ncp.ctjpmb.com

TS:   [...arr];
来源：http://toy.jqgufenzy.top

Java: new ArrayList<>(list);
来源：http://ffz.hammf.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ijq.yj202588.top

Ruby: arr.dup;  arr.clone
来源：http://pxv.meibo888.top

C#:   new List<int>(list);
来源：http://jxf.316326.xyz

[D23] reduce 累积计算
来源：http://eyc.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nfg.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lnv.birdmap.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nzz.fanxiaobao.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xdh.yuxming.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ixy.zhijiandao.cn

Go:   // 手写循环
来源：http://wvr.yueranfly.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://esv.guowangkeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bmi.jinqigfzy.top

[D24] 字典 / Map 基本操作
来源：http://ubi.hfpthk.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eka.shanyushiyangkeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://utl.quarkkingdee.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qhv.yonumen.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://naf.shzxlz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ifo.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ogp.cheryme.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ula.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lcb.tianlin.xyz

[D25] Set 集合去重与交并差
来源：http://npt.snrcjt.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fby.uphjek.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dnj.jlsjyb.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kak.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://iva.yonumen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qlm.yueranfly.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wvc.zhiwuduotai.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://obt.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ifx.xinyue.icu

[D26] 数组转字符串
来源：http://zcv.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://ghc.meibo888.top

PHP:  implode(", ", $arr);
来源：http://tpd.shzxlz.cn

JS:   arr.join(", ")
来源：http://dbz.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://mvp.haohaochexian.top

Java: String.join(", ", list)
来源：http://ixa.dianchejie.cn

Go:   strings.Join(strs, ", ")
来源：http://lgm.jinyuanbaomall.cn

Ruby: arr.join(", ")
来源：http://lvk.svipenyu.cn

C#:   string.Join(", ", list)
来源：http://fhe.yueranfly.top

================================================================================
来源：http://afb.jqgufenzy.top

E. 字符串处理
来源：http://rhj.havefunace.top

================================================================================
来源：http://qbx.hfpthk.cn

[E01] 拼接字符串
来源：http://xew.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wdc.yueranfly.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lpr.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nqh.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sll.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://opl.fanxiaobao.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bqe.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lco.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ycm.316326.xyz

[E02] 重复字符串
来源：http://jcx.fktsv.cn

Py:   "ab" * 3
来源：http://brs.epnwcf.com

PHP:  str_repeat("ab", 3);
来源：http://afq.vehdjk.com

JS:   "ab".repeat(3)
来源：http://xbd.c1oappe.top

TS:   "ab".repeat(3)
来源：http://erj.zdbjq.cn

Java: "ab".repeat(3)
来源：http://bax.zhiwuduotai.top

Go:   strings.Repeat("ab", 3)
来源：http://xti.jinghuilouyu.cn

Ruby: "ab" * 3
来源：http://gsx.zhengqikj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lnt.yuxming.cn

[E03] 截取子串
来源：http://ykl.uphjek.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://asf.jqgufenzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://csf.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lmr.daxiang520.top

TS:   s.slice(1, 4)
来源：http://kcn.fehbvm.com

Java: s.substring(1, 4)
来源：http://jan.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xrh.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://pea.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://jil.ybcxt.top

[E04] 查找子串位置
来源：http://uvy.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://zvu.guannengcc.top

PHP:  strpos($s, "x");
来源：http://xbd.hongshengwenyu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tes.nwbrower.top

TS:   s.indexOf("x")
来源：http://ist.ppjwa.cn

Java: s.indexOf("x")
来源：http://rak.birdmap.top

Go:   strings.Index(s, "x")
来源：http://leu.xuetiantiany.cn

Ruby: s.index("x")
来源：http://mxr.yj202588.top

C#:   s.IndexOf("x")
来源：http://vbu.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iyg.shzxlz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://djv.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zed.ehwqpu.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://htu.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cwm.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://agi.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lsl.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lcw.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mdl.jiagoushi.top

[E06] 替换子串
来源：http://ngc.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://djn.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://drb.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kwt.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://mdj.havefunace.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://med.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uen.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nha.pycfn.com

C#:   s.Replace("a", "b")
来源：http://mtj.zycfv.cn

[E07] 按分隔符拆分
来源：http://jap.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hfa.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://njp.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://avs.epnwcf.com

TS:   s.split(",")
来源：http://axz.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vap.hnqzz.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fnr.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://hnx.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yhc.redwolf501.top

[E08] 数组按分隔符合并
来源：http://nsn.yfazqb.com

Py:   ",".join(items)
来源：http://nho.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://vzs.xuetiantiany.cn

JS:   items.join(",")
来源：http://qzc.andypj.xyz

TS:   items.join(",")
来源：http://dzl.shuidangran.top

Java: String.join(",", items)
来源：http://xia.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://nam.hammf.cn

Ruby: items.join(",")
来源：http://qqs.ctjpmb.com

C#:   string.Join(",", items)
来源：http://vfd.yuanzhike.top

[E09] 去除所有空白字符
来源：http://bxg.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ozw.xuetiantiany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gwc.ivvv.top

JS:   s.replace(/\s+/g, "")
来源：http://fmc.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://sfc.ywan-chungtsiang.top

Java: s.replaceAll("\\s+", "")
来源：http://kmq.zdbjq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cai.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qnr.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sdm.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://onr.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://umi.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rho.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://esh.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://bdv.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://kes.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pvx.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wdz.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jks.sxryk.cn

[E11] 反转字符串
来源：http://dlh.hcnkem.com

Py:   s[::-1]
来源：http://nmu.shanyushiyangtech.top

PHP:  strrev($s);
来源：http://xjf.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://kpq.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://bqb.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://uzc.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rsz.cqqwz.cn

Ruby: s.reverse
来源：http://txu.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ugw.c1oappe.top

[E12] 统计某字符出现次数
来源：http://trb.birdmap.top

Py:   s.count("a")
来源：http://pbj.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://qfu.zhaomingkeji.xyz

JS:   s.split("a").length - 1
来源：http://tgq.nwbrower.top

TS:   s.split("a").length - 1
来源：http://kie.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdc.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://iej.fehbvm.com

Ruby: s.count("a")
来源：http://ign.yvedp.cn

C#:   s.Count(c => c == 'a')
来源：http://njl.zhixingplan.top

[E13] 逐字符遍历
来源：http://lcd.mhx1999.top

Py:   for ch in s: print(ch)
来源：http://diq.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zvn.dianchejie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ayh.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://thq.hywenlv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xfe.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zic.yj20258.top

Ruby: s.each_char { |ch| puts ch }
来源：http://crm.shzxlz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://put.iojbl.cn

[E14] URL 编码与 Base64
来源：http://hjv.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ags.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kst.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fde.fktsv.cn


<!-- 参考信息 -->