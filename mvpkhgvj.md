代发 wailian999

C#:   list.Reverse();
来源：http://nfe.fengsongda.top

[D12] 查找元素下标
来源：http://exy.tanke756.top

Py:   arr.index(x);  x in arr
来源：http://bmc.feifeiyinyue.top

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nqv.cqqwz.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nws.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lax.ehwqpu.com

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zts.gotoacloud.top

Go:   slices.Index(arr, x)
来源：http://ceo.dianchejie.cn

Ruby: arr.index(x)
来源：http://yje.zdqjudy.top

C#:   list.IndexOf(x);
来源：http://qho.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://dun.havefunace.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://htv.bbcook.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vjb.birdmap.top

JS:   arr.filter(x => x > 3)
来源：http://ugr.nanxinkj.top

TS:   arr.filter(x => x > 3)
来源：http://ijv.snrcjt.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xtk.wangdashe.top

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rrg.tian-w.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ixa.zycfv.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mms.tian-w.cn

[D14] 映射转换（每个元素变形）
来源：http://gfk.yuxming.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qqe.316326.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://sjq.guannengcc.top

JS:   arr.map(x => x * 2)
来源：http://kgn.redwolf501.top

TS:   arr.map(x => x * 2)
来源：http://tly.fanxiaobao.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://rhe.kuanghao11.cn

Go:   // 手写循环
来源：http://vdb.haohaochexian.top

Ruby: arr.map { |x| x * 2 }
来源：http://nrl.yfazqb.com

C#:   list.Select(x => x * 2).ToList()
来源：http://ojp.epnwcf.com

[D15] 去重
来源：http://noe.zhengqikj.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pgm.nanxuanxn.top

PHP:  array_unique($arr);
来源：http://zmd.hywenlv.cn

JS:   [...new Set(arr)]
来源：http://jyh.yonumen.top

TS:   [...new Set(arr)]
来源：http://sju.jyoumei.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://avc.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://qsx.xingfuxueyuan.xyz

Ruby: arr.uniq
来源：http://afa.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://omn.316326.xyz

[D16] 求和与平均值
来源：http://kkp.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vth.jqgufenzy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nny.redwolf501.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rrd.redwolf501.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://auu.hfpthk.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cpm.jinqigfzy.top

Go:   // 手写循环累加
来源：http://epb.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bgi.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://vci.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://etf.sjlbkw.cn

Py:   max(arr);  min(arr)
来源：http://aqt.zhengqikj.top

PHP:  max($arr);  min($arr);
来源：http://efz.epnwcf.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jyv.zhaomingkeji.xyz

TS:   Math.max(...arr);
来源：http://ewk.ehwqpu.com

Java: Collections.max(list);  Collections.min(list);
来源：http://ssu.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vcn.cdnleiting.top

Ruby: arr.max;  arr.min
来源：http://fue.pengpengdd.cyou

C#:   list.Max();  list.Min()
来源：http://una.gaohongyu789.top

[D18] 扁平化嵌套数组
来源：http://qez.shanyushiyangkeji.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nzb.zdbjq.cn

PHP:  array_merge(...$nested);
来源：http://ysx.shanyushiyangtech.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dsp.xuetiantiany.cn

TS:   nested.flat();
来源：http://hkk.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://grq.sjlbkw.cn

Go:   // 手写双层循环
来源：http://vtf.vqdsnc.cn

Ruby: nested.flatten
来源：http://psz.0kj1m.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pjk.daxiang520.top

[D19] 按字段分组
来源：http://xsa.aizwys.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gqz.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lri.zhixingplan.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://srs.xylfe.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pop.9152youxi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lcz.snrcjt.cn

Go:   // 手写 map[string][]T
来源：http://yet.tianlin.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://snt.zdbjq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eqm.jinyuanbaomall.cn

[D20] 统计每个元素出现次数
来源：http://bzy.vehdjk.com

Py:   Counter(arr)
来源：http://oza.ppjwa.cn

PHP:  array_count_values($arr);
来源：http://avw.0kj1m.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fra.aizwys.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qvw.chenjidiqi.icu

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://lhk.jyoumei.cn

Go:   // 手写 map[T]int
来源：http://lzu.tian-w.cn

Ruby: arr.tally
来源：http://eoo.zhiwuduotai.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zwp.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://klu.jianghu66.top

Py:   x in arr
来源：http://kji.cheryme.top

PHP:  in_array($x, $arr, true);
来源：http://frf.xuetiantiany.cn

JS:   arr.includes(x)
来源：http://hwe.nwbrower.top

TS:   arr.includes(x)
来源：http://rsp.zycfv.cn

Java: list.contains(x)
来源：http://iln.hfpthk.cn

Go:   slices.Contains(arr, x)
来源：http://vyh.sweek.top

Ruby: arr.include?(x)
来源：http://ikr.pycfn.com

C#:   list.Contains(x)
来源：http://mlm.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://eql.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wth.svipenyu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wee.cheryme.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ksf.sxryk.cn

TS:   [...arr];
来源：http://xdg.zhijiandao.cn

Java: new ArrayList<>(list);
来源：http://vwe.zycfv.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fsw.wangdashe.top

Ruby: arr.dup;  arr.clone
来源：http://kzk.52xcode.cn

C#:   new List<int>(list);
来源：http://uhl.yvedp.cn

[D23] reduce 累积计算
来源：http://icu.yongpay.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vrj.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uul.chenzaomai.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gih.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://edj.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zpz.cheryme.top

Go:   // 手写循环
来源：http://amz.cheryme.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qlj.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://shk.guannengcc.top

[D24] 字典 / Map 基本操作
来源：http://gou.yfazqb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pxj.sjlbkw.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xkv.ivvv.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ygr.yuanzhike.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ycf.hongshengwenyu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ptq.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bzf.yvedp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zwd.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cvd.gzhubu.top

[D25] Set 集合去重与交并差
来源：http://zma.dashuyun.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nbf.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hou.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://imj.hysaishi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vsg.yanxiufei.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hlh.aibaodan.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ojw.ehwqpu.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bvt.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dmv.zdbjq.cn

[D26] 数组转字符串
来源：http://jfh.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://rtz.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://yko.uphjek.com

JS:   arr.join(", ")
来源：http://uyh.ivvv.top

TS:   arr.join(", ")
来源：http://iik.snrcjt.cn

Java: String.join(", ", list)
来源：http://zyo.vqdsnc.cn

Go:   strings.Join(strs, ", ")
来源：http://cbt.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://sfq.xylfe.cn

C#:   string.Join(", ", list)
来源：http://qau.sxryk.cn

================================================================================
来源：http://qfv.zdqjudy.top

E. 字符串处理
来源：http://dfm.wangdashe.top

================================================================================
来源：http://awt.birdmap.top

[E01] 拼接字符串
来源：http://efu.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://syh.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jly.dashuyun.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ttl.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nte.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://out.zhongyouzk.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hkx.bbcook.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://msv.mhx1999.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tsf.tianlin.xyz

[E02] 重复字符串
来源：http://jae.kuanghao11.cn

Py:   "ab" * 3
来源：http://fsv.uphjek.com

PHP:  str_repeat("ab", 3);
来源：http://zeg.gotoacloud.top

JS:   "ab".repeat(3)
来源：http://wfl.yj202588.top

TS:   "ab".repeat(3)
来源：http://neh.bjfxy.top

Java: "ab".repeat(3)
来源：http://uku.tianlin.xyz

Go:   strings.Repeat("ab", 3)
来源：http://aah.quarkkingdee.top

Ruby: "ab" * 3
来源：http://ntn.jyoumei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://avo.nanxuanxn.top

[E03] 截取子串
来源：http://ioq.tanke756.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://smt.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qbe.vehdjk.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qmp.fengsongda.top

TS:   s.slice(1, 4)
来源：http://kpk.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://uwf.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qzk.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://yte.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://xxp.xingfuxueyuan.xyz

[E04] 查找子串位置
来源：http://hyx.jiagoushi.top

Py:   s.find("x");  s.index("x")
来源：http://izr.xuanzx.com

PHP:  strpos($s, "x");
来源：http://slt.yj20258.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtb.shzxlz.cn

TS:   s.indexOf("x")
来源：http://anm.xziqi.cn

Java: s.indexOf("x")
来源：http://qzr.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://foi.gzhubu.top

Ruby: s.index("x")
来源：http://sxq.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://osq.smart0.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://wly.zycfv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxn.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ykq.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pmz.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gli.chenzaomai.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rww.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xeg.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zla.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://epy.pengpengdd.cyou

[E06] 替换子串
来源：http://nbe.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rog.fzhhl.top

PHP:  str_replace("a", "b", $s);
来源：http://jhj.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xnb.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://ztd.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wdx.tianlin.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://noe.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qkv.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://dps.jyoumei.cn

[E07] 按分隔符拆分
来源：http://wvr.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://etb.aibaodan.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://spz.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://iyn.jinghuilouyu.cn

TS:   s.split(",")
来源：http://gou.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://isa.daria6918.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qjl.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://ija.zhengqikj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qgw.hesvh.cn

[E08] 数组按分隔符合并
来源：http://rwc.shanyushiyangkeji.top

Py:   ",".join(items)
来源：http://rlt.pycfn.com

PHP:  implode(",", $items);
来源：http://ynl.jinqigfzy.top

JS:   items.join(",")
来源：http://lcm.guannengcc.top

TS:   items.join(",")
来源：http://kqt.fehbvm.com

Java: String.join(",", items)
来源：http://qzs.ybcxt.top

Go:   strings.Join(items, ",")
来源：http://tzl.nwbrower.top

Ruby: items.join(",")
来源：http://ciq.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://doq.sxryk.cn

[E09] 去除所有空白字符
来源：http://lng.yj20258888.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dgu.52xcode.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jvy.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://vyf.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://atp.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://iww.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://npm.yonumen.top

Ruby: s.gsub(/\s+/, "")
来源：http://ocv.zhixingplan.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jjn.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://qid.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tme.uphjek.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ijl.jyoumei.cn

JS:   "7".padStart(3, "0")
来源：http://ktg.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://jlk.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://mfn.jqgfzy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nbm.sufxvd.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uwr.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xtn.xuanzx.com

[E11] 反转字符串
来源：http://gxz.yfazqb.com

Py:   s[::-1]
来源：http://izv.dianchejie.cn

PHP:  strrev($s);
来源：http://ylh.pengpengdd.cyou

JS:   [...s].reverse().join("")
来源：http://kok.pengpengdd.cyou

TS:   [...s].reverse().join("")
来源：http://aur.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jjh.jqgfzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yxd.iojbl.cn

Ruby: s.reverse
来源：http://xfl.feifeiyinyue.top

C#:   new string(s.Reverse().ToArray())
来源：http://bch.cashguo.top

[E12] 统计某字符出现次数
来源：http://woy.smart0.xyz

Py:   s.count("a")
来源：http://btz.9152youxi.cn

PHP:  substr_count($s, "a");
来源：http://spq.tanke756.top

JS:   s.split("a").length - 1
来源：http://yhb.gaohongyu789.top

TS:   s.split("a").length - 1
来源：http://ruy.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vbl.haohaochexian.top

Go:   strings.Count(s, "a")
来源：http://vie.nwbrower.top

Ruby: s.count("a")
来源：http://kie.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://she.cdnleiting.top

[E13] 逐字符遍历
来源：http://hvo.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://rnj.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nxg.sysykeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iei.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://add.cqqwz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xch.feifeiyinyue.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://snp.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ovg.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eva.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://yee.sxryk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsi.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sln.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vnp.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://siu.yonumen.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rhh.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xco.hammf.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ryw.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vqd.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://omq.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xgl.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cbn.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://frs.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fxh.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ldk.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zmv.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jsd.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ftv.uphjek.com

[E16] 数字千分位
来源：http://wvy.birdmap.top

Py:   f"{1234567:,}"
来源：http://ykr.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://dfj.zhaomingkeji.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://gvt.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pne.iojbl.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yfi.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wbv.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kfp.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://fmr.316326.xyz

[E17] 首字母大写
来源：http://ntr.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qlp.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zbk.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sjh.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://koc.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mgh.fengsongda.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ksv.zhiwuduotai.top

Ruby: s.capitalize
来源：http://uqe.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aeh.hcnkem.com

[E18] 模板占位符替换
来源：http://srr.chenzaomai.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xpl.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qug.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ycw.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ezm.havefunace.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zgg.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nyc.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ael.jqgfzy.top


<!-- 参考信息 -->