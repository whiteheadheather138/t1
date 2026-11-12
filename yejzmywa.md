代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zmm.gaohongyu789.top

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rhr.cashguo.top

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://izs.c1oappe.top

Go:   slices.Index(arr, x)
来源：http://ebm.meibo888.top

Ruby: arr.index(x)
来源：http://hgn.chenjidiqi.icu

C#:   list.IndexOf(x);
来源：http://nho.snrcjt.cn

[D13] 过滤（保留满足条件的）
来源：http://xwt.redwolf501.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://adq.cdnleiting.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vtj.52xcode.cn

JS:   arr.filter(x => x > 3)
来源：http://suo.dianchejie.cn

TS:   arr.filter(x => x > 3)
来源：http://ufl.birdmap.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qgd.zhoulong.xyz

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dwo.quarkkingdee.top

Ruby: arr.select { |x| x > 3 }
来源：http://sib.cucudq.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://alg.fanxiaobao.xyz

[D14] 映射转换（每个元素变形）
来源：http://voo.shanyushiyangkeji.top

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zps.guowangkeji.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dmf.svipenyu.cn

JS:   arr.map(x => x * 2)
来源：http://upb.daria6918.cn

TS:   arr.map(x => x * 2)
来源：http://idw.zhaomingkeji.xyz

Java: list.stream().map(x -> x * 2).toList()
来源：http://zai.bbcook.cn

Go:   // 手写循环
来源：http://xvi.wangdashe.top

Ruby: arr.map { |x| x * 2 }
来源：http://sin.smart0.xyz

C#:   list.Select(x => x * 2).ToList()
来源：http://xxz.zdbjq.cn

[D15] 去重
来源：http://mul.xylfe.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wss.shangyingyoupin.top

PHP:  array_unique($arr);
来源：http://sxh.316326.xyz

JS:   [...new Set(arr)]
来源：http://ncf.aizwys.cn

TS:   [...new Set(arr)]
来源：http://uoa.uphjek.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eiq.sjlbkw.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vwy.uphjek.com

Ruby: arr.uniq
来源：http://kpq.cheryme.top

C#:   list.Distinct().ToList()
来源：http://orn.meibo888.top

[D16] 求和与平均值
来源：http://zvh.zdbjq.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://stc.yfazqb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ovr.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xxe.zhoulong.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://npg.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kid.aibaodan.cn

Go:   // 手写循环累加
来源：http://xcp.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://eso.cucudq.cn

C#:   list.Sum();  list.Average()
来源：http://zxq.nanxinkj.top

[D17] 最大值与最小值
来源：http://wom.bbcook.cn

Py:   max(arr);  min(arr)
来源：http://lte.havefunace.top

PHP:  max($arr);  min($arr);
来源：http://uxi.fzhhl.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://otf.316326.xyz

TS:   Math.max(...arr);
来源：http://tco.cashguo.top

Java: Collections.max(list);  Collections.min(list);
来源：http://qdm.jinghuilouyu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ixw.nanxuanxn.top

Ruby: arr.max;  arr.min
来源：http://ebj.yvedp.cn

C#:   list.Max();  list.Min()
来源：http://pwu.zhongyouzk.top

[D18] 扁平化嵌套数组
来源：http://uvt.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fjo.cqqwz.cn

PHP:  array_merge(...$nested);
来源：http://lkl.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rxk.jinghuilouyu.cn

TS:   nested.flat();
来源：http://grh.nwbrower.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ywj.shuidangran.top

Go:   // 手写双层循环
来源：http://bzx.ydjk.org.cn

Ruby: nested.flatten
来源：http://bmu.nanxuanxn.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://bmf.yangfankeji.com

[D19] 按字段分组
来源：http://anf.fzhhl.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vkz.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zco.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rqn.xziqi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jok.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://abw.dianchejie.cn

Go:   // 手写 map[string][]T
来源：http://mlm.smart0.xyz

Ruby: arr.group_by { |x| x[:type] }
来源：http://ael.zhaomingkeji.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nnf.xziqi.cn

[D20] 统计每个元素出现次数
来源：http://qsu.xingfuxueyuan.xyz

Py:   Counter(arr)
来源：http://cht.ydzc1.top

PHP:  array_count_values($arr);
来源：http://pfb.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pcn.uphjek.com

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://eow.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rkq.jinqigufen.top

Go:   // 手写 map[T]int
来源：http://vul.xylfe.cn

Ruby: arr.tally
来源：http://msn.zhixingplan.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pkx.cashguo.top

[D21] 判断是否包含某元素
来源：http://ldm.c1oappe.top

Py:   x in arr
来源：http://xgp.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://tpk.iojbl.cn

JS:   arr.includes(x)
来源：http://iuz.mhx1999.top

TS:   arr.includes(x)
来源：http://ime.xylfe.cn

Java: list.contains(x)
来源：http://lqh.hcnkem.com

Go:   slices.Contains(arr, x)
来源：http://kbr.sysykeji.top

Ruby: arr.include?(x)
来源：http://gpj.316326.xyz

C#:   list.Contains(x)
来源：http://tdn.fehbvm.com

[D22] 复制数组（避免共享引用）
来源：http://vvn.jiagoushi.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ewl.jianghu66.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gan.vqdsnc.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zhe.yj20258888.top

TS:   [...arr];
来源：http://bok.gogol.net.cn

Java: new ArrayList<>(list);
来源：http://dbg.ctjpmb.com

Go:   copied := append([]int(nil), arr...)
来源：http://hiw.tanke756.top

Ruby: arr.dup;  arr.clone
来源：http://oic.jyoumei.cn

C#:   new List<int>(list);
来源：http://bof.zhiwuduotai.top

[D23] reduce 累积计算
来源：http://wcq.fengsongda.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ktm.dianchejie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://itl.tarul.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fjm.cqqwz.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gab.jinqigfzy.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://gsq.svipenyu.cn

Go:   // 手写循环
来源：http://oiw.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aap.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pdf.wangdashe.top

[D24] 字典 / Map 基本操作
来源：http://ntr.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qwg.bjfxy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ogn.hnxiangtu.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dhe.gaohongyu789.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://syi.zhaomingkeji.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gbl.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqw.sxryk.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qbl.ydzc1.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oat.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://cgv.gaohongyu789.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lko.yvedp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cig.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qhn.jyoumei.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aqm.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xdq.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hgp.havefunace.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zyt.wangdashe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgt.nanxuanxn.top

[D26] 数组转字符串
来源：http://sic.316326.xyz

Py:   ", ".join(map(str, arr))
来源：http://gbc.zdqjudy.top

PHP:  implode(", ", $arr);
来源：http://uwn.dianchejie.cn

JS:   arr.join(", ")
来源：http://vjg.cheryme.top

TS:   arr.join(", ")
来源：http://azo.yuxming.cn

Java: String.join(", ", list)
来源：http://wtg.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://iaz.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://ywr.tanke756.top

C#:   string.Join(", ", list)
来源：http://xrg.xylfe.cn

================================================================================
来源：http://uod.fzhhl.top

E. 字符串处理
来源：http://egd.ehwqpu.com

================================================================================
来源：http://csi.zycfv.cn

[E01] 拼接字符串
来源：http://eng.zhixingplan.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pwl.dianchejie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pom.fanxiaobao.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lfy.yuanzhike.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eac.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tjd.redwolf501.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jni.zhiwuduotai.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kez.ppjwa.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://obw.svipenyu.cn

[E02] 重复字符串
来源：http://tnh.yongpay.top

Py:   "ab" * 3
来源：http://nvr.havefunace.top

PHP:  str_repeat("ab", 3);
来源：http://mhp.guowangkeji.top

JS:   "ab".repeat(3)
来源：http://teb.jiagoushi.top

TS:   "ab".repeat(3)
来源：http://agx.nanxinkj.top

Java: "ab".repeat(3)
来源：http://vyf.zdqjudy.top

Go:   strings.Repeat("ab", 3)
来源：http://ztk.birdmap.top

Ruby: "ab" * 3
来源：http://xmg.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://flw.jiagoushi.top

[E03] 截取子串
来源：http://agy.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tkj.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pcc.xinyue.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xlj.daxiang520.top

TS:   s.slice(1, 4)
来源：http://zeu.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://kzy.jlsjyb.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ooj.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://asc.gogol.net.cn

C#:   s.Substring(1, 3)
来源：http://zat.epnwcf.com

[E04] 查找子串位置
来源：http://wzj.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://crn.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://ngu.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kff.jinqigufen.top

TS:   s.indexOf("x")
来源：http://iok.hfpthk.cn

Java: s.indexOf("x")
来源：http://upe.zdqjudy.top

Go:   strings.Index(s, "x")
来源：http://nwo.ydzc1.top

Ruby: s.index("x")
来源：http://oeg.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://foh.jqgufenzy.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://pkl.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iox.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://muo.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tyi.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iyk.andypj.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ofr.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jwf.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zif.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://frt.kuanghao11.cn

[E06] 替换子串
来源：http://ris.yfazqb.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qmu.wangshuangyany.cn

PHP:  str_replace("a", "b", $s);
来源：http://zwb.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tet.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://bfb.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tfh.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ahf.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vmg.hnxiangtu.top

C#:   s.Replace("a", "b")
来源：http://bfz.ivvv.top

[E07] 按分隔符拆分
来源：http://kiv.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tkw.feifeiyinyue.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://khw.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qei.daxiang520.top

TS:   s.split(",")
来源：http://psi.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://kxk.wangshuangyany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bcy.zdqjudy.top

Ruby: s.split(",");  s.split
来源：http://zyv.ydjk.org.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lwt.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://wnp.xziqi.cn

Py:   ",".join(items)
来源：http://arj.redwolf501.top

PHP:  implode(",", $items);
来源：http://rct.kuanghao11.cn

JS:   items.join(",")
来源：http://xze.fzhhl.top

TS:   items.join(",")
来源：http://uqf.birdmap.top

Java: String.join(",", items)
来源：http://yji.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://shg.cdnleiting.top

Ruby: items.join(",")
来源：http://pva.smart0.xyz

C#:   string.Join(",", items)
来源：http://sig.hnxiangtu.top

[E09] 去除所有空白字符
来源：http://yvw.fktsv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qvd.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://atr.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://mgo.uphjek.com

TS:   s.replace(/\s+/g, "")
来源：http://qvz.yongpay.top

Java: s.replaceAll("\\s+", "")
来源：http://vjh.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gcz.hongshengwenyu.top

Ruby: s.gsub(/\s+/, "")
来源：http://jfz.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qex.vehdjk.com

[E10] 左侧补零 / 定长填充
来源：http://kkx.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tmc.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cbz.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://azc.c1oappe.top

TS:   "7".padStart(3, "0")
来源：http://bwu.cheryme.top

Java: String.format("%03d", 7)
来源：http://qaw.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nqp.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nis.svipenyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fvs.52xcode.cn

[E11] 反转字符串
来源：http://akz.hywenlv.cn

Py:   s[::-1]
来源：http://gvh.hfpthk.cn

PHP:  strrev($s);
来源：http://aaz.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://czc.sweek.top

TS:   [...s].reverse().join("")
来源：http://vau.ydzc1.top

Java: new StringBuilder(s).reverse().toString()
来源：http://css.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dgn.wangdashe.top

Ruby: s.reverse
来源：http://mgy.hesvh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wzi.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://uce.hfpthk.cn

Py:   s.count("a")
来源：http://jxj.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://ttt.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://gkd.ppjwa.cn

TS:   s.split("a").length - 1
来源：http://ajb.haohaochexian.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ahj.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://npq.yj20258.top

Ruby: s.count("a")
来源：http://kpd.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://ygy.zdbjq.cn

[E13] 逐字符遍历
来源：http://ehe.hammf.cn

Py:   for ch in s: print(ch)
来源：http://cak.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baf.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://upt.c1oappe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cup.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://svk.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lhd.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rwb.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jmq.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://pzv.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aba.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cdq.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wxt.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zno.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ayl.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://soj.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yhd.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vkv.sweek.top

[E15] HTML 转义 / 反转义
来源：http://bgx.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xho.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zig.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nyc.nanxuanxn.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pef.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rqc.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kjc.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tvl.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://znq.ybcxt.top

[E16] 数字千分位
来源：http://ndy.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://gyu.ctjpmb.com

PHP:  number_format(1234567);
来源：http://qtb.svipenyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uxq.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pqo.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cge.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jdn.gotoacloud.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://thl.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://byw.meibo888.top

[E17] 首字母大写
来源：http://ykx.dianchejie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dcj.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://phq.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xpi.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://usa.ctjpmb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpy.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jfs.hfpthk.cn

Ruby: s.capitalize
来源：http://skc.ppjwa.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dga.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://tde.jqgufenzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ehy.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fux.ybcxt.top

JS:   tpl.replaceAll("{name}", name)
来源：http://haj.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pka.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://izc.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bhe.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zdb.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eka.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://tuj.yangfankeji.com

Py:   s.splitlines()
来源：http://mtw.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xdi.jqgufenzy.top


<!-- 参考信息 -->