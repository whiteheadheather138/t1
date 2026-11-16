代发 wailian999

TS:   [...arr].reverse();
来源：http://xdr.zhoulong.xyz

Java: Collections.reverse(list);
来源：http://rns.shanyushiyangkeji.top

Go:   slices.Reverse(arr)
来源：http://swu.yuxming.cn

Ruby: arr.reverse
来源：http://fto.chenjidiqi.icu

C#:   list.Reverse();
来源：http://mop.mhx1999.top

[D12] 查找元素下标
来源：http://icm.svipenyu.cn

Py:   arr.index(x);  x in arr
来源：http://zbt.meibo888.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ebi.yj20258.top

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nof.316326.xyz

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rdo.hcnkem.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kge.zycfv.cn

Go:   slices.Index(arr, x)
来源：http://nhu.zhiwuduotai.top

Ruby: arr.index(x)
来源：http://wtn.gotoacloud.top

C#:   list.IndexOf(x);
来源：http://jyi.jinqigufen.top

[D13] 过滤（保留满足条件的）
来源：http://yql.fktsv.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ijg.shanyushiyangkeji.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://usf.cheryme.top

JS:   arr.filter(x => x > 3)
来源：http://zhm.0kj1m.cn

TS:   arr.filter(x => x > 3)
来源：http://hwh.smart0.xyz

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lds.hysaishi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zhq.hysaishi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cja.kuanghao11.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nba.andypj.xyz

[D14] 映射转换（每个元素变形）
来源：http://xqc.sweek.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fbm.zhengqikj.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dij.aizwys.cn

JS:   arr.map(x => x * 2)
来源：http://wkd.hcnkem.com

TS:   arr.map(x => x * 2)
来源：http://ncs.quarkkingdee.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://ulf.aizwys.cn

Go:   // 手写循环
来源：http://lao.0kj1m.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zne.yuxming.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dqx.iojbl.cn

[D15] 去重
来源：http://mug.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tyc.yj202588.top

PHP:  array_unique($arr);
来源：http://wrj.chenlongwang.top

JS:   [...new Set(arr)]
来源：http://snx.cucudq.cn

TS:   [...new Set(arr)]
来源：http://zpz.smart0.xyz

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bxh.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://ysx.sweek.top

Ruby: arr.uniq
来源：http://fty.bbcook.cn

C#:   list.Distinct().ToList()
来源：http://xou.jqgfzy.top

[D16] 求和与平均值
来源：http://fnq.bbcook.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wdi.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hxi.gogol.net.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hry.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pxj.316326.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kca.jinyuanbaomall.cn

Go:   // 手写循环累加
来源：http://rpx.zhongyouzk.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mdk.feifeiyinyue.top

C#:   list.Sum();  list.Average()
来源：http://fnl.zhongyouzk.top

[D17] 最大值与最小值
来源：http://vmc.dianchejie.cn

Py:   max(arr);  min(arr)
来源：http://vjy.jinqigfzy.top

PHP:  max($arr);  min($arr);
来源：http://gku.ppjwa.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ufl.redwolf501.top

TS:   Math.max(...arr);
来源：http://shh.dashuyun.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nao.dianchejie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bdc.jqgufenzy.top

Ruby: arr.max;  arr.min
来源：http://wca.daria6918.cn

C#:   list.Max();  list.Min()
来源：http://kld.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://yve.cucudq.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ntg.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://yax.kuanghao11.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://moo.yuxming.cn

TS:   nested.flat();
来源：http://bxc.shanyushiyangtech.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bkd.fzhhl.top

Go:   // 手写双层循环
来源：http://abl.kuanghao11.cn

Ruby: nested.flatten
来源：http://wfd.cucudq.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jsi.cucudq.cn

[D19] 按字段分组
来源：http://dnj.feifeiyinyue.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cbh.fehbvm.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://liq.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lqw.chenjidiqi.icu

TS:   Object.groupBy(arr, x => x.type)
来源：http://reu.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vqd.xuanzx.com

Go:   // 手写 map[string][]T
来源：http://fvg.haohaochexian.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://wow.jinghuilouyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wvr.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://rjl.jqgufenzy.top

Py:   Counter(arr)
来源：http://dwn.cheryme.top

PHP:  array_count_values($arr);
来源：http://vhm.pengpengdd.cyou

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqs.gzhubu.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tle.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oaz.jqgufenzy.top

Go:   // 手写 map[T]int
来源：http://lks.zhijiandao.cn

Ruby: arr.tally
来源：http://ixm.shzxlz.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lyl.zhaomingkeji.xyz

[D21] 判断是否包含某元素
来源：http://xnb.wangdashe.top

Py:   x in arr
来源：http://bay.xuanzx.com

PHP:  in_array($x, $arr, true);
来源：http://ttt.zdqjudy.top

JS:   arr.includes(x)
来源：http://zao.fengsongda.top

TS:   arr.includes(x)
来源：http://xvs.epnwcf.com

Java: list.contains(x)
来源：http://hhw.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://aif.c1oappe.top

Ruby: arr.include?(x)
来源：http://wrz.nanxinkj.top

C#:   list.Contains(x)
来源：http://myv.daria6918.cn

[D22] 复制数组（避免共享引用）
来源：http://tyr.jyoumei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oqf.jiagoushi.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cea.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xnt.jiagoushi.top

TS:   [...arr];
来源：http://vmk.guannengcc.top

Java: new ArrayList<>(list);
来源：http://enf.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rrt.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://ieh.yvedp.cn

C#:   new List<int>(list);
来源：http://ewq.sweek.top

[D23] reduce 累积计算
来源：http://mfb.fktsv.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zgl.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hqs.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eca.kuanghao11.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hdh.yj20258888.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://sze.sufxvd.cn

Go:   // 手写循环
来源：http://hfi.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gkd.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jug.shzxlz.cn

[D24] 字典 / Map 基本操作
来源：http://opf.pycfn.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://peo.guannengcc.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wym.daxiang520.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ccu.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lxu.chenzaomai.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xnp.zycfv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ewv.fehbvm.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iso.snrcjt.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://svy.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://juv.zhaomingkeji.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://cay.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vks.nanxuanxn.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rps.ydzc1.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zly.aizwys.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yfj.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tfa.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://usk.sxryk.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oqh.xuanzx.com

[D26] 数组转字符串
来源：http://nev.aibaodan.cn

Py:   ", ".join(map(str, arr))
来源：http://iib.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://zfj.gotoacloud.top

JS:   arr.join(", ")
来源：http://lmp.havefunace.top

TS:   arr.join(", ")
来源：http://fus.zhixingplan.top

Java: String.join(", ", list)
来源：http://cmn.daxiang520.top

Go:   strings.Join(strs, ", ")
来源：http://bly.shzxlz.cn

Ruby: arr.join(", ")
来源：http://ata.ppjwa.cn

C#:   string.Join(", ", list)
来源：http://eji.iojbl.cn

================================================================================
来源：http://zdn.jqgufenzy.top

E. 字符串处理
来源：http://wzn.epnwcf.com

================================================================================
来源：http://qwk.hysaishi.cn

[E01] 拼接字符串
来源：http://hkp.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lmp.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rmn.zhiwuduotai.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://udl.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dml.birdmap.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lwi.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zay.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pdt.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dyi.sjlbkw.cn

[E02] 重复字符串
来源：http://nid.ydjk.org.cn

Py:   "ab" * 3
来源：http://sxd.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://dfu.jqgfzy.top

JS:   "ab".repeat(3)
来源：http://apk.cqqwz.cn

TS:   "ab".repeat(3)
来源：http://lqy.zhengqikj.top

Java: "ab".repeat(3)
来源：http://dos.tarul.cn

Go:   strings.Repeat("ab", 3)
来源：http://rfa.hnqzz.top

Ruby: "ab" * 3
来源：http://myg.nanxinkj.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://crp.sweek.top

[E03] 截取子串
来源：http://vwe.cheryme.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bcj.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hvk.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ujp.tarul.cn

TS:   s.slice(1, 4)
来源：http://ogz.fanxiaobao.xyz

Java: s.substring(1, 4)
来源：http://vie.pengpengdd.cyou

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qrg.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zub.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://kvx.yangfankeji.com

[E04] 查找子串位置
来源：http://vnn.jqgufenzy.top

Py:   s.find("x");  s.index("x")
来源：http://qqv.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://bjh.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pfr.ydzc1.top

TS:   s.indexOf("x")
来源：http://ykx.fzhhl.top

Java: s.indexOf("x")
来源：http://oon.cashguo.top

Go:   strings.Index(s, "x")
来源：http://tho.sysykeji.top

Ruby: s.index("x")
来源：http://pur.yonumen.top

C#:   s.IndexOf("x")
来源：http://rgu.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hih.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xpq.bbcook.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://avv.fehbvm.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kek.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://vyw.guannengcc.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upz.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fmv.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jii.havefunace.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hdp.hongshengwenyu.top

[E06] 替换子串
来源：http://tty.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bof.wangdashe.top

PHP:  str_replace("a", "b", $s);
来源：http://ayk.cucudq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ode.jinghuilouyu.cn

TS:   s.replaceAll("a", "b")
来源：http://sct.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vna.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyl.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zrd.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://jpc.fzhhl.top

[E07] 按分隔符拆分
来源：http://did.gogol.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jfm.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eqp.xinyue.icu

JS:   s.split(",");  s.split(/\s+/)
来源：http://pee.yuxming.cn

TS:   s.split(",")
来源：http://hve.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cfq.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://khv.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://rum.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jih.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://nlp.ehwqpu.com

Py:   ",".join(items)
来源：http://uev.pycfn.com

PHP:  implode(",", $items);
来源：http://tgq.ppjwa.cn

JS:   items.join(",")
来源：http://jmq.tanke756.top

TS:   items.join(",")
来源：http://mok.tian-w.cn

Java: String.join(",", items)
来源：http://vbt.yongpay.top

Go:   strings.Join(items, ",")
来源：http://hrx.aibaodan.cn

Ruby: items.join(",")
来源：http://irt.ybcxt.top

C#:   string.Join(",", items)
来源：http://hyd.smart0.xyz

[E09] 去除所有空白字符
来源：http://qiw.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vvo.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zfn.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://rsl.yuanzhike.top

TS:   s.replace(/\s+/g, "")
来源：http://mcx.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://svu.jlsjyb.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ilf.0kj1m.cn

Ruby: s.gsub(/\s+/, "")
来源：http://myo.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ykv.zhoulong.xyz

[E10] 左侧补零 / 定长填充
来源：http://akr.daria6918.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wnn.gotoacloud.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wbw.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://qmr.feifeiyinyue.top

TS:   "7".padStart(3, "0")
来源：http://ytx.tanke756.top

Java: String.format("%03d", 7)
来源：http://sfu.feifeiyinyue.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ckd.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://luv.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qnb.jlsjyb.cn

[E11] 反转字符串
来源：http://vtc.zhoulong.xyz

Py:   s[::-1]
来源：http://kxo.c1oappe.top

PHP:  strrev($s);
来源：http://evl.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://itp.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://srw.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cgf.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mxv.pycfn.com

Ruby: s.reverse
来源：http://kqj.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://drm.yj20258.top

[E12] 统计某字符出现次数
来源：http://jwb.jinqigfzy.top

Py:   s.count("a")
来源：http://crh.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://fbq.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://xge.quarkkingdee.top

TS:   s.split("a").length - 1
来源：http://mjs.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ack.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://vzt.ydjk.org.cn

Ruby: s.count("a")
来源：http://ugu.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://bxp.c1oappe.top

[E13] 逐字符遍历
来源：http://pfy.jinqigfzy.top

Py:   for ch in s: print(ch)
来源：http://xes.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ksz.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qrf.jinyuanbaomall.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bfc.nanxuanxn.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zta.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sau.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://snt.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qws.xuanzx.com

[E14] URL 编码与 Base64
来源：http://ksg.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvu.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dhq.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pge.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oek.cdnleiting.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dij.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ivd.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://niy.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nuv.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://ykj.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cjy.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lxz.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://owk.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fkd.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vmi.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vbc.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vlr.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ngp.epnwcf.com

[E16] 数字千分位
来源：http://tir.iojbl.cn

Py:   f"{1234567:,}"
来源：http://wax.yongpay.top

PHP:  number_format(1234567);
来源：http://rzz.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://khp.jqgfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://boc.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://evb.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://swt.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://irz.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://ryq.xylfe.cn

[E17] 首字母大写
来源：http://amj.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tkf.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://axz.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jof.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnn.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://egx.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zdt.gzhubu.top

Ruby: s.capitalize
来源：http://cbs.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hpr.ctjpmb.com

[E18] 模板占位符替换
来源：http://fiz.sufxvd.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rqd.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://odp.smart0.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://fvi.fktsv.cn


<!-- 参考信息 -->