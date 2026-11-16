代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://fqu.wangdashe.top

TS:   [...a, ...b];
来源：http://muc.guowangkeji.top

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zes.sysykeji.top

Go:   append(a, b...)
来源：http://bko.52xcode.cn

Ruby: a + b;  a.concat(b)
来源：http://vdd.zdbjq.cn

C#:   a.Concat(b).ToList()
来源：http://gjw.nanxinkj.top

[D09] 排序（升序）
来源：http://rmb.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://uzq.tanke756.top

PHP:  sort($arr);
来源：http://rbq.ppjwa.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qgb.yanxiufei.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dhs.jqgufenzy.top

Java: Collections.sort(list);  list.sort(null);
来源：http://asb.gzhubu.top

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qbb.mhx1999.top

Ruby: arr.sort
来源：http://eqe.sweek.top

C#:   list.Sort();
来源：http://qbp.daxiang520.top

[D10] 自定义排序（按字段 / 多条件）
来源：http://jlg.sjlbkw.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://led.ehwqpu.com

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ljv.yfazqb.com

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zvy.sxryk.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wyq.aibaodan.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bzh.xuanzx.com

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nqx.yonumen.top

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dvp.ppjwa.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ouy.tian-w.cn

[D11] 反转数组
来源：http://zwi.shangyingyoupin.top

Py:   arr[::-1];  arr.reverse()
来源：http://ckv.zhengqikj.top

PHP:  array_reverse($arr);
来源：http://tob.zhongyouzk.top

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cye.nanxinkj.top

TS:   [...arr].reverse();
来源：http://knh.ppjwa.cn

Java: Collections.reverse(list);
来源：http://oql.zdbjq.cn

Go:   slices.Reverse(arr)
来源：http://ahi.hnqzz.top

Ruby: arr.reverse
来源：http://xhs.hnxiangtu.top

C#:   list.Reverse();
来源：http://dia.kuanghao11.cn

[D12] 查找元素下标
来源：http://sgn.xuetiantiany.cn

Py:   arr.index(x);  x in arr
来源：http://enn.ehwqpu.com

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://maf.yongpay.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mvd.cashguo.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vtf.zhijiandao.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://rgc.ybcxt.top

Go:   slices.Index(arr, x)
来源：http://vck.redwolf501.top

Ruby: arr.index(x)
来源：http://uen.nanxinkj.top

C#:   list.IndexOf(x);
来源：http://ywp.cashguo.top

[D13] 过滤（保留满足条件的）
来源：http://gsk.andypj.xyz

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://xuo.gaohongyu789.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nur.yfazqb.com

JS:   arr.filter(x => x > 3)
来源：http://dsy.zhengqikj.top

TS:   arr.filter(x => x > 3)
来源：http://mxo.yongpay.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://kck.ydzc1.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sqp.mhx1999.top

Ruby: arr.select { |x| x > 3 }
来源：http://kbk.andypj.xyz

C#:   list.Where(x => x > 3).ToList()
来源：http://ywv.iojbl.cn

[D14] 映射转换（每个元素变形）
来源：http://sfz.cheryme.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://goj.gzhubu.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://efq.jinqigufen.top

JS:   arr.map(x => x * 2)
来源：http://hca.sxryk.cn

TS:   arr.map(x => x * 2)
来源：http://qth.9152youxi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cie.xuanzx.com

Go:   // 手写循环
来源：http://usg.shzxlz.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aub.hywenlv.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ert.hesvh.cn

[D15] 去重
来源：http://pzk.aizwys.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://okg.hywenlv.cn

PHP:  array_unique($arr);
来源：http://zad.jinqigfzy.top

JS:   [...new Set(arr)]
来源：http://uia.hammf.cn

TS:   [...new Set(arr)]
来源：http://cvw.jiagoushi.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://olc.0kj1m.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kob.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://raj.hongshengwenyu.top

C#:   list.Distinct().ToList()
来源：http://vwk.vehdjk.com

[D16] 求和与平均值
来源：http://uua.yanxiufei.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wek.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qdf.smart0.xyz

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ywi.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jiz.fengsongda.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gnp.jqgfzy.top

Go:   // 手写循环累加
来源：http://cmg.ppjwa.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jkl.gogol.net.cn

C#:   list.Sum();  list.Average()
来源：http://wvt.zhixingplan.top

[D17] 最大值与最小值
来源：http://xoe.havefunace.top

Py:   max(arr);  min(arr)
来源：http://ipr.jinghuilouyu.cn

PHP:  max($arr);  min($arr);
来源：http://dwi.yangfankeji.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yii.guannengcc.top

TS:   Math.max(...arr);
来源：http://fnt.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://enx.pycfn.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ggh.ivvv.top

Ruby: arr.max;  arr.min
来源：http://tvu.sxryk.cn

C#:   list.Max();  list.Min()
来源：http://kcx.xingfuxueyuan.xyz

[D18] 扁平化嵌套数组
来源：http://ypt.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eqc.hywenlv.cn

PHP:  array_merge(...$nested);
来源：http://zno.nwbrower.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zae.cqqwz.cn

TS:   nested.flat();
来源：http://cgi.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cqy.jyoumei.cn

Go:   // 手写双层循环
来源：http://dks.nanxuanxn.top

Ruby: nested.flatten
来源：http://kdv.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://chs.yanxiufei.cn

[D19] 按字段分组
来源：http://dkx.sufxvd.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yoe.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fki.bjfxy.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nzr.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://xeb.fzhhl.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yva.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://dun.tanke756.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://zhd.aizwys.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://niw.c1oappe.top

[D20] 统计每个元素出现次数
来源：http://ynk.hysaishi.cn

Py:   Counter(arr)
来源：http://sji.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://giu.yfazqb.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://buv.andypj.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uis.c1oappe.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wbz.shangyingyoupin.top

Go:   // 手写 map[T]int
来源：http://ysh.sjlbkw.cn

Ruby: arr.tally
来源：http://yby.jianghu66.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vuh.bbcook.cn

[D21] 判断是否包含某元素
来源：http://imc.yueranfly.top

Py:   x in arr
来源：http://rau.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://ows.aizwys.cn

JS:   arr.includes(x)
来源：http://nfg.yanxiufei.cn

TS:   arr.includes(x)
来源：http://rga.cheryme.top

Java: list.contains(x)
来源：http://tac.pycfn.com

Go:   slices.Contains(arr, x)
来源：http://umr.ehwqpu.com

Ruby: arr.include?(x)
来源：http://bzb.bjfxy.top

C#:   list.Contains(x)
来源：http://ojv.bjfxy.top

[D22] 复制数组（避免共享引用）
来源：http://upb.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fdw.fengsongda.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zpw.ivvv.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://arx.jqgfzy.top

TS:   [...arr];
来源：http://wev.pycfn.com

Java: new ArrayList<>(list);
来源：http://ost.hywenlv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nay.hfpthk.cn

Ruby: arr.dup;  arr.clone
来源：http://bpk.meibo888.top

C#:   new List<int>(list);
来源：http://eaw.sweek.top

[D23] reduce 累积计算
来源：http://ean.gaohongyu789.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kzk.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tzw.jlsjyb.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gmk.dashuyun.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ply.jlsjyb.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dzx.andypj.xyz

Go:   // 手写循环
来源：http://mpa.zhongyouzk.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vjf.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qet.ywan-chungtsiang.top

[D24] 字典 / Map 基本操作
来源：http://kqr.vehdjk.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://puv.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://myj.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zwq.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dqz.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ycy.jinqigufen.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gre.gaohongyu789.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://piy.xingfuxueyuan.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sbn.zhijiandao.cn

[D25] Set 集合去重与交并差
来源：http://dwx.jqgufenzy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xbr.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fxq.andypj.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lkh.tarul.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dyh.xuetiantiany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xdj.yj20258.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://typ.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://swo.shangyingyoupin.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wnt.cheryme.top

[D26] 数组转字符串
来源：http://mwj.daria6918.cn

Py:   ", ".join(map(str, arr))
来源：http://hnn.yj20258888.top

PHP:  implode(", ", $arr);
来源：http://fgn.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://hvr.hnqzz.top

TS:   arr.join(", ")
来源：http://lqs.ctjpmb.com

Java: String.join(", ", list)
来源：http://iya.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://lyn.shuidangran.top

Ruby: arr.join(", ")
来源：http://eka.zycfv.cn

C#:   string.Join(", ", list)
来源：http://wou.svipenyu.cn

================================================================================
来源：http://jdz.yueranfly.top

E. 字符串处理
来源：http://grz.havefunace.top

================================================================================
来源：http://sjy.jianghu66.top

[E01] 拼接字符串
来源：http://dlc.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fev.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fph.hnqzz.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://exk.xylfe.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxx.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dfo.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xoa.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nla.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jvn.fengsongda.top

[E02] 重复字符串
来源：http://ztw.jiagoushi.top

Py:   "ab" * 3
来源：http://aju.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://deo.52xcode.cn

JS:   "ab".repeat(3)
来源：http://zpy.jinyuanbaomall.cn

TS:   "ab".repeat(3)
来源：http://tfy.yj202588.top

Java: "ab".repeat(3)
来源：http://okp.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://riy.hysaishi.cn

Ruby: "ab" * 3
来源：http://bbg.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ucv.fktsv.cn

[E03] 截取子串
来源：http://nzh.feifeiyinyue.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qqc.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iuy.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qfl.ivvv.top

TS:   s.slice(1, 4)
来源：http://hfk.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://vlv.guannengcc.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://omw.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gkf.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://tdz.yongpay.top

[E04] 查找子串位置
来源：http://kwe.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://mrg.c1oappe.top

PHP:  strpos($s, "x");
来源：http://epi.gogol.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bdy.ehwqpu.com

TS:   s.indexOf("x")
来源：http://ook.hammf.cn

Java: s.indexOf("x")
来源：http://egl.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://chl.haohaochexian.top

Ruby: s.index("x")
来源：http://lzl.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://bnd.wangshuangyany.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vsn.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ykj.ydzc1.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kms.shanyushiyangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ovu.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bkx.wangdashe.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iut.gogol.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tjy.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wji.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tho.svipenyu.cn

[E06] 替换子串
来源：http://hhi.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lqm.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://djy.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://stv.yj20258.top

TS:   s.replaceAll("a", "b")
来源：http://wpa.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujo.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iuq.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://usv.hammf.cn

C#:   s.Replace("a", "b")
来源：http://anf.xuanzx.com

[E07] 按分隔符拆分
来源：http://iou.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ubg.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ifo.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kjn.jlsjyb.cn

TS:   s.split(",")
来源：http://azf.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://qbn.zhaomingkeji.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://typ.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://pfm.gzhubu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sfa.dashuyun.cn

[E08] 数组按分隔符合并
来源：http://ukm.cucudq.cn

Py:   ",".join(items)
来源：http://gox.jqgfzy.top

PHP:  implode(",", $items);
来源：http://puj.feifeiyinyue.top

JS:   items.join(",")
来源：http://nab.tianlin.xyz

TS:   items.join(",")
来源：http://npi.jinqigufen.top

Java: String.join(",", items)
来源：http://tcu.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://glh.ctjpmb.com

Ruby: items.join(",")
来源：http://ynt.chenlongwang.top

C#:   string.Join(",", items)
来源：http://mhf.fzhhl.top

[E09] 去除所有空白字符
来源：http://vzm.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ebf.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cdn.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://txs.hywenlv.cn

TS:   s.replace(/\s+/g, "")
来源：http://sgc.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://ldy.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://mrn.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://nyj.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ucr.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://krp.dashuyun.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ssq.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://slp.hcnkem.com

JS:   "7".padStart(3, "0")
来源：http://aat.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://igt.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://hig.zdbjq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pch.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qhh.quarkkingdee.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lxf.havefunace.top

[E11] 反转字符串
来源：http://qpn.yj20258888.top

Py:   s[::-1]
来源：http://kdx.yangfankeji.com

PHP:  strrev($s);
来源：http://qjy.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://npr.yonumen.top

TS:   [...s].reverse().join("")
来源：http://adb.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://puc.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zpy.cqqwz.cn

Ruby: s.reverse
来源：http://xsl.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://zdw.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://wch.smart0.xyz

Py:   s.count("a")
来源：http://ykz.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://dar.hfpthk.cn

JS:   s.split("a").length - 1
来源：http://gxh.yanxiufei.cn

TS:   s.split("a").length - 1
来源：http://rev.shanyushiyangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oid.cheryme.top

Go:   strings.Count(s, "a")
来源：http://phb.c1oappe.top

Ruby: s.count("a")
来源：http://ohh.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://sez.yuxming.cn

[E13] 逐字符遍历
来源：http://oyr.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://coc.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gjj.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vxi.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qde.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bwr.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zju.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nlw.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://urf.guannengcc.top

[E14] URL 编码与 Base64
来源：http://wtr.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aag.shanyushiyangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://irk.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fto.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hxo.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebf.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://brt.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hnc.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ujx.vqdsnc.cn

[E15] HTML 转义 / 反转义
来源：http://kox.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gxd.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bmk.nanxinkj.top


<!-- 参考信息 -->