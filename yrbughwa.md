代发 wailian999

TS:   [...arr].reverse();
来源：http://gjh.gogol.net.cn

Java: Collections.reverse(list);
来源：http://ibr.hnxiangtu.top

Go:   slices.Reverse(arr)
来源：http://iyn.shzxlz.cn

Ruby: arr.reverse
来源：http://ugl.cheryme.top

C#:   list.Reverse();
来源：http://wwg.52xcode.cn

[D12] 查找元素下标
来源：http://mol.chenzaomai.com

Py:   arr.index(x);  x in arr
来源：http://jjo.xylfe.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wta.fengsongda.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mpp.kuanghao11.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://twi.daxiang520.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://seh.chenzaomai.com

Go:   slices.Index(arr, x)
来源：http://fgl.zhijiandao.cn

Ruby: arr.index(x)
来源：http://ntm.andypj.xyz

C#:   list.IndexOf(x);
来源：http://lrb.yangfankeji.com

[D13] 过滤（保留满足条件的）
来源：http://cdy.jianghu66.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yyj.ydjk.org.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mzy.xuetiantiany.cn

JS:   arr.filter(x => x > 3)
来源：http://ajj.ehwqpu.com

TS:   arr.filter(x => x > 3)
来源：http://htd.shanyushiyangkeji.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xcr.zhixingplan.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bjz.zhongyouzk.top

Ruby: arr.select { |x| x > 3 }
来源：http://wvj.bjfxy.top

C#:   list.Where(x => x > 3).ToList()
来源：http://sii.daxiang520.top

[D14] 映射转换（每个元素变形）
来源：http://hgw.yvedp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sgy.yuxming.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sne.fanxiaobao.xyz

JS:   arr.map(x => x * 2)
来源：http://saj.xziqi.cn

TS:   arr.map(x => x * 2)
来源：http://rim.ivvv.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://jbr.chenjidiqi.icu

Go:   // 手写循环
来源：http://bcu.hesvh.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ifj.sufxvd.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qid.gotoacloud.top

[D15] 去重
来源：http://nup.yueranfly.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://icf.shzxlz.cn

PHP:  array_unique($arr);
来源：http://asb.cqqwz.cn

JS:   [...new Set(arr)]
来源：http://qyf.yuanzhike.top

TS:   [...new Set(arr)]
来源：http://awq.feifeiyinyue.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dhb.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://dgm.sjlbkw.cn

Ruby: arr.uniq
来源：http://met.hfpthk.cn

C#:   list.Distinct().ToList()
来源：http://bco.hywenlv.cn

[D16] 求和与平均值
来源：http://gko.ppjwa.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ajc.chenzaomai.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wkz.shanyushiyangkeji.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kbu.pengpengdd.cyou

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wuh.yj202588.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://awn.cashguo.top

Go:   // 手写循环累加
来源：http://baz.yanxiufei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uhd.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://ube.daxiang520.top

[D17] 最大值与最小值
来源：http://eho.xinyue.icu

Py:   max(arr);  min(arr)
来源：http://wie.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://vbm.shanyushiyangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hwi.hesvh.cn

TS:   Math.max(...arr);
来源：http://ixb.shanyushiyangkeji.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rkb.fengsongda.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://aie.quarkkingdee.top

Ruby: arr.max;  arr.min
来源：http://kqy.svipenyu.cn

C#:   list.Max();  list.Min()
来源：http://zks.316326.xyz

[D18] 扁平化嵌套数组
来源：http://drd.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pit.birdmap.top

PHP:  array_merge(...$nested);
来源：http://gar.jqgufenzy.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dpv.yvedp.cn

TS:   nested.flat();
来源：http://zmw.dashuyun.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://his.feifeiyinyue.top

Go:   // 手写双层循环
来源：http://urq.jianghu66.top

Ruby: nested.flatten
来源：http://lqg.guannengcc.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://iqe.quarkkingdee.top

[D19] 按字段分组
来源：http://kbb.daxiang520.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sbz.sweek.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://soh.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mrb.uphjek.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://ugm.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hcr.fzhhl.top

Go:   // 手写 map[string][]T
来源：http://pfd.ywan-chungtsiang.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kpq.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://exp.tianlin.xyz

[D20] 统计每个元素出现次数
来源：http://csv.hywenlv.cn

Py:   Counter(arr)
来源：http://tmy.zycfv.cn

PHP:  array_count_values($arr);
来源：http://yxv.zhijiandao.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ggi.316326.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://awh.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mub.ehwqpu.com

Go:   // 手写 map[T]int
来源：http://txl.jqgufenzy.top

Ruby: arr.tally
来源：http://lcy.hcnkem.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hag.redwolf501.top

[D21] 判断是否包含某元素
来源：http://xfn.havefunace.top

Py:   x in arr
来源：http://osb.vqdsnc.cn

PHP:  in_array($x, $arr, true);
来源：http://xxk.cucudq.cn

JS:   arr.includes(x)
来源：http://wex.jinqigfzy.top

TS:   arr.includes(x)
来源：http://qbp.yonumen.top

Java: list.contains(x)
来源：http://jzv.yj20258888.top

Go:   slices.Contains(arr, x)
来源：http://qvn.smart0.xyz

Ruby: arr.include?(x)
来源：http://fkm.gzhubu.top

C#:   list.Contains(x)
来源：http://qxx.jqgfzy.top

[D22] 复制数组（避免共享引用）
来源：http://swe.sufxvd.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fwk.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zfl.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tls.ehwqpu.com

TS:   [...arr];
来源：http://wds.cqqwz.cn

Java: new ArrayList<>(list);
来源：http://jww.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qnl.ybcxt.top

Ruby: arr.dup;  arr.clone
来源：http://llv.shanyushiyangtech.top

C#:   new List<int>(list);
来源：http://qgb.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://ugy.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dhf.yueranfly.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://szp.xylfe.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jtg.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://taa.zycfv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://srf.jiagoushi.top

Go:   // 手写循环
来源：http://ito.uphjek.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gxg.ybcxt.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zcz.wangshuangyany.cn

[D24] 字典 / Map 基本操作
来源：http://fyh.yangfankeji.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qgr.hcnkem.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zdx.jyoumei.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qio.sysykeji.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fwp.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ofj.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zcm.shangyingyoupin.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rcl.meibo888.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jde.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://jmd.andypj.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hph.yangfankeji.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lzf.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dmq.yj20258.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lpp.yuxming.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ofu.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qof.tian-w.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kpo.shuidangran.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mzl.svipenyu.cn

[D26] 数组转字符串
来源：http://tbc.yongpay.top

Py:   ", ".join(map(str, arr))
来源：http://hkr.chenzaomai.com

PHP:  implode(", ", $arr);
来源：http://dyd.vqdsnc.cn

JS:   arr.join(", ")
来源：http://bdl.yanxiufei.cn

TS:   arr.join(", ")
来源：http://rdf.ywan-chungtsiang.top

Java: String.join(", ", list)
来源：http://bik.zhiwuduotai.top

Go:   strings.Join(strs, ", ")
来源：http://ihk.uphjek.com

Ruby: arr.join(", ")
来源：http://nqz.xziqi.cn

C#:   string.Join(", ", list)
来源：http://elp.daxiang520.top

================================================================================
来源：http://okz.nanxuanxn.top

E. 字符串处理
来源：http://scv.zhaomingkeji.xyz

================================================================================
来源：http://dqv.fengsongda.top

[E01] 拼接字符串
来源：http://bdx.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uej.pengpengdd.cyou

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wxc.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rpa.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoc.zdbjq.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ish.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aze.yj20258.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fem.zhongyouzk.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tma.nanxinkj.top

[E02] 重复字符串
来源：http://uyi.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://hhy.hammf.cn

PHP:  str_repeat("ab", 3);
来源：http://xdd.hfpthk.cn

JS:   "ab".repeat(3)
来源：http://llq.xziqi.cn

TS:   "ab".repeat(3)
来源：http://rni.wangshuangyany.cn

Java: "ab".repeat(3)
来源：http://qyq.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://mwf.havefunace.top

Ruby: "ab" * 3
来源：http://jxg.feifeiyinyue.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nip.quarkkingdee.top

[E03] 截取子串
来源：http://nfn.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://waa.hysaishi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lqc.0kj1m.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lnh.xziqi.cn

TS:   s.slice(1, 4)
来源：http://hiy.aizwys.cn

Java: s.substring(1, 4)
来源：http://iim.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jnz.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://tkb.sxryk.cn

C#:   s.Substring(1, 3)
来源：http://dao.hammf.cn

[E04] 查找子串位置
来源：http://zhk.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://xwi.zhiwuduotai.top

PHP:  strpos($s, "x");
来源：http://zub.9152youxi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ajh.zhixingplan.top

TS:   s.indexOf("x")
来源：http://gwr.9152youxi.cn

Java: s.indexOf("x")
来源：http://hnf.hfpthk.cn

Go:   strings.Index(s, "x")
来源：http://cdk.yj20258.top

Ruby: s.index("x")
来源：http://agv.bbcook.cn

C#:   s.IndexOf("x")
来源：http://fdh.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://opt.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://isl.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zig.zdqjudy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fko.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mqg.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edj.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uru.hammf.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://htp.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cpz.feifeiyinyue.top

[E06] 替换子串
来源：http://dux.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://won.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://kgk.zhijiandao.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pxj.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://tqd.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pit.yuxming.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://beg.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ral.svipenyu.cn

C#:   s.Replace("a", "b")
来源：http://gor.zhixingplan.top

[E07] 按分隔符拆分
来源：http://tym.ybcxt.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eof.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://niz.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://fpr.shanyushiyangtech.top

TS:   s.split(",")
来源：http://nzo.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://pxo.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://aui.ehwqpu.com

Ruby: s.split(",");  s.split
来源：http://zza.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oou.iojbl.cn

[E08] 数组按分隔符合并
来源：http://ouh.chenlongwang.top

Py:   ",".join(items)
来源：http://rab.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://ghb.cashguo.top

JS:   items.join(",")
来源：http://kex.vqdsnc.cn

TS:   items.join(",")
来源：http://gcw.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://rgp.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://wxz.shzxlz.cn

Ruby: items.join(",")
来源：http://rzt.xylfe.cn

C#:   string.Join(",", items)
来源：http://ydw.xuetiantiany.cn

[E09] 去除所有空白字符
来源：http://vru.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mzx.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qlm.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://xsk.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://pzo.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://teb.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://drl.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gze.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vrn.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://hnq.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zrn.yj202588.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ioa.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://yyj.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://eyn.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://nty.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mdp.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eao.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zyz.shanyushiyangtech.top

[E11] 反转字符串
来源：http://ayk.haohaochexian.top

Py:   s[::-1]
来源：http://fxs.zhijiandao.cn

PHP:  strrev($s);
来源：http://cjh.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://yux.svipenyu.cn

TS:   [...s].reverse().join("")
来源：http://hzq.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tuc.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ggu.hesvh.cn

Ruby: s.reverse
来源：http://ndl.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://zvj.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://aoi.ydzc1.top

Py:   s.count("a")
来源：http://xol.ppjwa.cn

PHP:  substr_count($s, "a");
来源：http://lgb.uphjek.com

JS:   s.split("a").length - 1
来源：http://lzq.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://ovg.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://omg.c1oappe.top

Go:   strings.Count(s, "a")
来源：http://xsx.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://qhk.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://lvj.zycfv.cn

[E13] 逐字符遍历
来源：http://vbg.hfpthk.cn

Py:   for ch in s: print(ch)
来源：http://pdq.bjfxy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ydy.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fso.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://prz.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sdm.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://una.ehwqpu.com

Ruby: s.each_char { |ch| puts ch }
来源：http://cuw.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://quw.xylfe.cn

[E14] URL 编码与 Base64
来源：http://mab.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://joh.ydjk.org.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://urp.svipenyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xyp.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bit.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xps.fanxiaobao.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hdk.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zld.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wiy.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://uqo.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uym.hysaishi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ggv.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://poq.yongpay.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qeg.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tzn.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lib.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wkh.vqdsnc.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tmn.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://dto.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://imf.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://dql.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rno.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ggn.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://whn.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fgz.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tbf.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://dxw.ydjk.org.cn

[E17] 首字母大写
来源：http://ktm.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://osg.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fha.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rov.xuanzx.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://imq.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lcb.yj20258.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dde.yanxiufei.cn

Ruby: s.capitalize
来源：http://acv.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ibz.cashguo.top

[E18] 模板占位符替换
来源：http://jcw.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qtl.ppjwa.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wau.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://yjr.xylfe.cn


<!-- 参考信息 -->