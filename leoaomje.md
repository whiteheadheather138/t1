代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ump.tianlin.xyz

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jiu.jlsjyb.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gvb.zhiwuduotai.top

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cjv.tianlin.xyz

[D11] 反转数组
来源：http://gfg.zhongyouzk.top

Py:   arr[::-1];  arr.reverse()
来源：http://ucl.zycfv.cn

PHP:  array_reverse($arr);
来源：http://dct.52xcode.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gxb.zdqjudy.top

TS:   [...arr].reverse();
来源：http://gng.zhixingplan.top

Java: Collections.reverse(list);
来源：http://vsx.birdmap.top

Go:   slices.Reverse(arr)
来源：http://nxt.tanke756.top

Ruby: arr.reverse
来源：http://maf.fehbvm.com

C#:   list.Reverse();
来源：http://wea.xziqi.cn

[D12] 查找元素下标
来源：http://tto.zhengqikj.top

Py:   arr.index(x);  x in arr
来源：http://yko.xinyue.icu

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bef.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ulf.shanyushiyangtech.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gce.aibaodan.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cju.zhengqikj.top

Go:   slices.Index(arr, x)
来源：http://xwa.cdnleiting.top

Ruby: arr.index(x)
来源：http://vno.xinyue.icu

C#:   list.IndexOf(x);
来源：http://izr.316326.xyz

[D13] 过滤（保留满足条件的）
来源：http://fwv.jinghuilouyu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://eim.zhijiandao.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gde.zycfv.cn

JS:   arr.filter(x => x > 3)
来源：http://cok.fktsv.cn

TS:   arr.filter(x => x > 3)
来源：http://koz.meibo888.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://khx.hesvh.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://btn.fanxiaobao.xyz

Ruby: arr.select { |x| x > 3 }
来源：http://qpo.xylfe.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://eqd.xziqi.cn

[D14] 映射转换（每个元素变形）
来源：http://yuf.zhongyouzk.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://owx.aizwys.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ngt.sweek.top

JS:   arr.map(x => x * 2)
来源：http://srw.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://hyv.ctjpmb.com

Java: list.stream().map(x -> x * 2).toList()
来源：http://njo.jqgufenzy.top

Go:   // 手写循环
来源：http://kyi.jianghu66.top

Ruby: arr.map { |x| x * 2 }
来源：http://gdh.zdqjudy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://pfb.tian-w.cn

[D15] 去重
来源：http://ejf.ydjk.org.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vwu.tian-w.cn

PHP:  array_unique($arr);
来源：http://wdk.52xcode.cn

JS:   [...new Set(arr)]
来源：http://vlf.fehbvm.com

TS:   [...new Set(arr)]
来源：http://mfe.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zxm.zdqjudy.top

Go:   // 用 map[T]struct{} 手写
来源：http://jly.52xcode.cn

Ruby: arr.uniq
来源：http://imj.sjlbkw.cn

C#:   list.Distinct().ToList()
来源：http://oxl.pycfn.com

[D16] 求和与平均值
来源：http://pii.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://efr.chenlongwang.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fkc.ehwqpu.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ttz.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nfg.birdmap.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mfd.ppjwa.cn

Go:   // 手写循环累加
来源：http://mbm.birdmap.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qdb.jinghuilouyu.cn

C#:   list.Sum();  list.Average()
来源：http://evx.jlsjyb.cn

[D17] 最大值与最小值
来源：http://hcq.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://cxi.kuanghao11.cn

PHP:  max($arr);  min($arr);
来源：http://tzf.ivvv.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fnu.meibo888.top

TS:   Math.max(...arr);
来源：http://yjc.cqqwz.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ing.xuetiantiany.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ake.ctjpmb.com

Ruby: arr.max;  arr.min
来源：http://apd.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://giy.ivvv.top

[D18] 扁平化嵌套数组
来源：http://xfv.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fvi.dashuyun.cn

PHP:  array_merge(...$nested);
来源：http://jol.zhixingplan.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://etb.cdnleiting.top

TS:   nested.flat();
来源：http://kas.gogol.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://rdd.zycfv.cn

Go:   // 手写双层循环
来源：http://fpm.pycfn.com

Ruby: nested.flatten
来源：http://hkt.xinyue.icu

C#:   nested.SelectMany(x => x).ToList()
来源：http://tqh.fanxiaobao.xyz

[D19] 按字段分组
来源：http://cfk.zdqjudy.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hap.mhx1999.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eni.dashuyun.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gjm.shzxlz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qvz.jlsjyb.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xak.sufxvd.cn

Go:   // 手写 map[string][]T
来源：http://med.gotoacloud.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://mux.hnqzz.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://grb.yonumen.top

[D20] 统计每个元素出现次数
来源：http://szp.uphjek.com

Py:   Counter(arr)
来源：http://oqu.nwbrower.top

PHP:  array_count_values($arr);
来源：http://fuc.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cfu.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nql.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ros.birdmap.top

Go:   // 手写 map[T]int
来源：http://vjx.hcnkem.com

Ruby: arr.tally
来源：http://oyg.jqgufenzy.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qht.sysykeji.top

[D21] 判断是否包含某元素
来源：http://ndc.daria6918.cn

Py:   x in arr
来源：http://kqb.hesvh.cn

PHP:  in_array($x, $arr, true);
来源：http://jql.fehbvm.com

JS:   arr.includes(x)
来源：http://nzi.tarul.cn

TS:   arr.includes(x)
来源：http://fve.nanxinkj.top

Java: list.contains(x)
来源：http://ntm.zycfv.cn

Go:   slices.Contains(arr, x)
来源：http://cqv.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://tno.hnxiangtu.top

C#:   list.Contains(x)
来源：http://esr.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://dqx.redwolf501.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fia.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://our.dashuyun.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zgt.xinyue.icu

TS:   [...arr];
来源：http://nmb.kuanghao11.cn

Java: new ArrayList<>(list);
来源：http://xll.xuetiantiany.cn

Go:   copied := append([]int(nil), arr...)
来源：http://usd.cheryme.top

Ruby: arr.dup;  arr.clone
来源：http://gsn.havefunace.top

C#:   new List<int>(list);
来源：http://szp.ybcxt.top

[D23] reduce 累积计算
来源：http://bcp.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wti.9152youxi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pbh.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oav.hnxiangtu.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jyj.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://meo.gotoacloud.top

Go:   // 手写循环
来源：http://zcl.epnwcf.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://oup.yangfankeji.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yxm.xinyue.icu

[D24] 字典 / Map 基本操作
来源：http://pls.redwolf501.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rff.zhiwuduotai.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://duk.shuidangran.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rle.sweek.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cta.ydzc1.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jhb.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ycr.kuanghao11.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://joh.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://srs.xylfe.cn

[D25] Set 集合去重与交并差
来源：http://teg.tanke756.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rlb.nwbrower.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hhg.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mfe.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qmi.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://etp.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sld.ctjpmb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yds.ydzc1.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zbq.jiagoushi.top

[D26] 数组转字符串
来源：http://myh.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://fgf.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://pwk.guannengcc.top

JS:   arr.join(", ")
来源：http://wph.zhoulong.xyz

TS:   arr.join(", ")
来源：http://laf.xylfe.cn

Java: String.join(", ", list)
来源：http://gol.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://rcd.jyoumei.cn

Ruby: arr.join(", ")
来源：http://gcr.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://wnw.gotoacloud.top

================================================================================
来源：http://kov.shanyushiyangkeji.top

E. 字符串处理
来源：http://chk.feifeiyinyue.top

================================================================================
来源：http://oiu.iojbl.cn

[E01] 拼接字符串
来源：http://lei.yangfankeji.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gur.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dck.daria6918.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://chi.redwolf501.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qna.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yku.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://onj.dianchejie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xye.ivvv.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qko.smart0.xyz

[E02] 重复字符串
来源：http://czz.c1oappe.top

Py:   "ab" * 3
来源：http://xji.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://ofz.ydjk.org.cn

JS:   "ab".repeat(3)
来源：http://pkj.jianghu66.top

TS:   "ab".repeat(3)
来源：http://ssr.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://dai.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://pyq.jinqigfzy.top

Ruby: "ab" * 3
来源：http://mpd.xziqi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tkh.shuidangran.top

[E03] 截取子串
来源：http://wzr.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jzo.hammf.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oqb.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xaq.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://mky.xylfe.cn

Java: s.substring(1, 4)
来源：http://tjp.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kly.jqgufenzy.top

Ruby: s[1, 3];  s[1..3]
来源：http://mhj.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://isq.yj20258.top

[E04] 查找子串位置
来源：http://ltz.xylfe.cn

Py:   s.find("x");  s.index("x")
来源：http://vlc.cdnleiting.top

PHP:  strpos($s, "x");
来源：http://baz.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zny.cucudq.cn

TS:   s.indexOf("x")
来源：http://bia.chenlongwang.top

Java: s.indexOf("x")
来源：http://pxn.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://iss.aibaodan.cn

Ruby: s.index("x")
来源：http://krd.epnwcf.com

C#:   s.IndexOf("x")
来源：http://ibt.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://uqd.tarul.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fuj.yonumen.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axl.sxryk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yfk.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://fsh.jinqigufen.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rgd.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pvq.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://naa.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qbo.zhoulong.xyz

[E06] 替换子串
来源：http://hay.hfpthk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ckc.birdmap.top

PHP:  str_replace("a", "b", $s);
来源：http://cgp.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://iev.dashuyun.cn

TS:   s.replaceAll("a", "b")
来源：http://lhl.pycfn.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vvd.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hzb.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mtk.birdmap.top

C#:   s.Replace("a", "b")
来源：http://shx.xziqi.cn

[E07] 按分隔符拆分
来源：http://jah.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ehy.hnqzz.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uvn.vehdjk.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kjg.shanyushiyangtech.top

TS:   s.split(",")
来源：http://znc.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oyx.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://evv.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://rhn.ywan-chungtsiang.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ikx.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://qxh.hnxiangtu.top

Py:   ",".join(items)
来源：http://bwd.daxiang520.top

PHP:  implode(",", $items);
来源：http://gyc.jqgfzy.top

JS:   items.join(",")
来源：http://hly.daria6918.cn

TS:   items.join(",")
来源：http://gge.cucudq.cn

Java: String.join(",", items)
来源：http://hvd.yonumen.top

Go:   strings.Join(items, ",")
来源：http://tkb.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://xex.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://svz.sysykeji.top

[E09] 去除所有空白字符
来源：http://xoj.zhixingplan.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xos.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ame.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://lxc.smart0.xyz

TS:   s.replace(/\s+/g, "")
来源：http://zqm.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://fvr.shuidangran.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pjj.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xjj.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ocw.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://hdb.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ror.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dre.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://ikm.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://fra.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://lbx.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://olm.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uqy.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qsz.dianchejie.cn

[E11] 反转字符串
来源：http://cqp.iojbl.cn

Py:   s[::-1]
来源：http://lrc.chenzaomai.com

PHP:  strrev($s);
来源：http://kpc.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://uls.havefunace.top

TS:   [...s].reverse().join("")
来源：http://cdt.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sfz.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uih.jinghuilouyu.cn

Ruby: s.reverse
来源：http://ybu.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://ufi.yanxiufei.cn

[E12] 统计某字符出现次数
来源：http://uor.hesvh.cn

Py:   s.count("a")
来源：http://giz.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://exh.zhiwuduotai.top

JS:   s.split("a").length - 1
来源：http://idn.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://ocp.hysaishi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://plo.yvedp.cn

Go:   strings.Count(s, "a")
来源：http://dag.yj20258888.top

Ruby: s.count("a")
来源：http://jte.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://fnb.hysaishi.cn

[E13] 逐字符遍历
来源：http://xdy.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://xzf.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qff.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hix.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zds.jinghuilouyu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fjs.sufxvd.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wdu.birdmap.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jkz.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hbq.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://rdg.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://imu.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mff.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dkt.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tbu.fehbvm.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vjd.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cfu.tarul.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lor.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ywy.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://sig.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kyv.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://geq.gotoacloud.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pug.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://rhw.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pgd.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://moz.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jnl.haohaochexian.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bhu.ehwqpu.com

[E16] 数字千分位
来源：http://ogu.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://fdh.yj20258888.top

PHP:  number_format(1234567);
来源：http://xha.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vqm.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ujv.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gub.xziqi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kxj.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pxp.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://ith.kuanghao11.cn

[E17] 首字母大写
来源：http://icw.ctjpmb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zhm.zhengqikj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mbd.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mqw.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uby.gaohongyu789.top


<!-- 参考信息 -->