代发 wailian999

Ruby: arr.index(x)
来源：http://nog.wangdashe.top

C#:   list.IndexOf(x);
来源：http://pga.jiagoushi.top

[D13] 过滤（保留满足条件的）
来源：http://nhm.guannengcc.top

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vgk.zhengqikj.top

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dqb.sweek.top

JS:   arr.filter(x => x > 3)
来源：http://izr.tarul.cn

TS:   arr.filter(x => x > 3)
来源：http://tdc.shanyushiyangtech.top

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ztk.yvedp.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dbd.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://pbn.cqqwz.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mfi.nanxinkj.top

[D14] 映射转换（每个元素变形）
来源：http://qds.cucudq.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qiu.xingfuxueyuan.xyz

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lqs.0kj1m.cn

JS:   arr.map(x => x * 2)
来源：http://djj.nanxuanxn.top

TS:   arr.map(x => x * 2)
来源：http://set.sjlbkw.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lyz.epnwcf.com

Go:   // 手写循环
来源：http://fvo.cashguo.top

Ruby: arr.map { |x| x * 2 }
来源：http://lko.jqgfzy.top

C#:   list.Select(x => x * 2).ToList()
来源：http://oxl.hnxiangtu.top

[D15] 去重
来源：http://gbg.jiagoushi.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ptt.havefunace.top

PHP:  array_unique($arr);
来源：http://usx.birdmap.top

JS:   [...new Set(arr)]
来源：http://jtp.redwolf501.top

TS:   [...new Set(arr)]
来源：http://sxp.fzhhl.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wws.xuetiantiany.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wug.jqgfzy.top

Ruby: arr.uniq
来源：http://aae.yvedp.cn

C#:   list.Distinct().ToList()
来源：http://zvo.ydjk.org.cn

[D16] 求和与平均值
来源：http://ggf.yvedp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yyq.xziqi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tok.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://los.sweek.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sns.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ojy.guowangkeji.top

Go:   // 手写循环累加
来源：http://lnr.meibo888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gxi.hammf.cn

C#:   list.Sum();  list.Average()
来源：http://oby.aibaodan.cn

[D17] 最大值与最小值
来源：http://hug.yj20258888.top

Py:   max(arr);  min(arr)
来源：http://leo.uphjek.com

PHP:  max($arr);  min($arr);
来源：http://eku.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xlc.daxiang520.top

TS:   Math.max(...arr);
来源：http://gfk.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xfx.sweek.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vcm.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://yri.c1oappe.top

C#:   list.Max();  list.Min()
来源：http://jxv.gzhubu.top

[D18] 扁平化嵌套数组
来源：http://zcf.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ohs.wangshuangyany.cn

PHP:  array_merge(...$nested);
来源：http://mat.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iwb.vehdjk.com

TS:   nested.flat();
来源：http://vfc.ehwqpu.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kaq.svipenyu.cn

Go:   // 手写双层循环
来源：http://fbr.mhx1999.top

Ruby: nested.flatten
来源：http://jfn.andypj.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://wcv.0kj1m.cn

[D19] 按字段分组
来源：http://dgz.pycfn.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jcf.vehdjk.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yhf.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqi.andypj.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://bwx.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kgi.zhengqikj.top

Go:   // 手写 map[string][]T
来源：http://ior.chenzaomai.com

Ruby: arr.group_by { |x| x[:type] }
来源：http://wxl.zhengqikj.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://man.shanyushiyangtech.top

[D20] 统计每个元素出现次数
来源：http://pec.hesvh.cn

Py:   Counter(arr)
来源：http://kbw.yueranfly.top

PHP:  array_count_values($arr);
来源：http://gix.nanxinkj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tio.52xcode.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nxz.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://och.sxryk.cn

Go:   // 手写 map[T]int
来源：http://yqy.52xcode.cn

Ruby: arr.tally
来源：http://xws.ctjpmb.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wnt.gaohongyu789.top

[D21] 判断是否包含某元素
来源：http://hzl.dianchejie.cn

Py:   x in arr
来源：http://jxp.xylfe.cn

PHP:  in_array($x, $arr, true);
来源：http://biv.epnwcf.com

JS:   arr.includes(x)
来源：http://kaz.hywenlv.cn

TS:   arr.includes(x)
来源：http://vut.yvedp.cn

Java: list.contains(x)
来源：http://smd.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://xcj.bjfxy.top

Ruby: arr.include?(x)
来源：http://tov.tian-w.cn

C#:   list.Contains(x)
来源：http://lej.yj202588.top

[D22] 复制数组（避免共享引用）
来源：http://rez.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cin.yangfankeji.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://emd.yvedp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hev.sweek.top

TS:   [...arr];
来源：http://iby.ybcxt.top

Java: new ArrayList<>(list);
来源：http://eho.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ohi.iojbl.cn

Ruby: arr.dup;  arr.clone
来源：http://ebo.shanyushiyangkeji.top

C#:   new List<int>(list);
来源：http://juz.jlsjyb.cn

[D23] reduce 累积计算
来源：http://kwa.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://etu.feifeiyinyue.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aua.yuxming.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ims.nwbrower.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvq.daria6918.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pva.jqgufenzy.top

Go:   // 手写循环
来源：http://aqy.cucudq.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vro.guannengcc.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dlw.fktsv.cn

[D24] 字典 / Map 基本操作
来源：http://bxk.jinyuanbaomall.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wcj.316326.xyz

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cmm.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cte.jianghu66.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://krl.jianghu66.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qsh.chenzaomai.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bss.hongshengwenyu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ayv.zhengqikj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nzk.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://fec.birdmap.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://woc.vehdjk.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nnp.aizwys.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qss.birdmap.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vhy.hammf.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wns.zdbjq.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://omh.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ysl.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ldq.ydjk.org.cn

[D26] 数组转字符串
来源：http://waz.feifeiyinyue.top

Py:   ", ".join(map(str, arr))
来源：http://tdl.cqqwz.cn

PHP:  implode(", ", $arr);
来源：http://dpv.zdbjq.cn

JS:   arr.join(", ")
来源：http://gxv.zdqjudy.top

TS:   arr.join(", ")
来源：http://zuv.pycfn.com

Java: String.join(", ", list)
来源：http://rgs.yvedp.cn

Go:   strings.Join(strs, ", ")
来源：http://kte.aibaodan.cn

Ruby: arr.join(", ")
来源：http://pjt.hfpthk.cn

C#:   string.Join(", ", list)
来源：http://idi.fzhhl.top

================================================================================
来源：http://zmc.shanyushiyangkeji.top

E. 字符串处理
来源：http://mol.xingfuxueyuan.xyz

================================================================================
来源：http://kra.aizwys.cn

[E01] 拼接字符串
来源：http://rep.andypj.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jse.sxryk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rkb.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ihz.birdmap.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hbo.yj20258888.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qyo.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xrs.snrcjt.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://abr.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kxr.xuanzx.com

[E02] 重复字符串
来源：http://wyl.chenzaomai.com

Py:   "ab" * 3
来源：http://aif.redwolf501.top

PHP:  str_repeat("ab", 3);
来源：http://xtx.sysykeji.top

JS:   "ab".repeat(3)
来源：http://jgi.chenjidiqi.icu

TS:   "ab".repeat(3)
来源：http://gwv.316326.xyz

Java: "ab".repeat(3)
来源：http://uuj.fktsv.cn

Go:   strings.Repeat("ab", 3)
来源：http://gds.zhoulong.xyz

Ruby: "ab" * 3
来源：http://uda.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qoe.bbcook.cn

[E03] 截取子串
来源：http://ims.jqgfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rlm.quarkkingdee.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vgm.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ndv.jqgfzy.top

TS:   s.slice(1, 4)
来源：http://ssd.mhx1999.top

Java: s.substring(1, 4)
来源：http://wpn.hnxiangtu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hxy.xingfuxueyuan.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://acp.ehwqpu.com

C#:   s.Substring(1, 3)
来源：http://qvu.xylfe.cn

[E04] 查找子串位置
来源：http://zue.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://lnv.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://ndq.bjfxy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nam.sjlbkw.cn

TS:   s.indexOf("x")
来源：http://kjy.feifeiyinyue.top

Java: s.indexOf("x")
来源：http://xqb.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://zwc.ctjpmb.com

Ruby: s.index("x")
来源：http://has.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://swp.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qbq.wangdashe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oax.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qwr.gaohongyu789.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kjf.sysykeji.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://eml.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ene.yanxiufei.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wmn.hnqzz.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hpr.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yif.zhengqikj.top

[E06] 替换子串
来源：http://ash.shanyushiyangtech.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zxf.nanxinkj.top

PHP:  str_replace("a", "b", $s);
来源：http://jrh.daria6918.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zri.0kj1m.cn

TS:   s.replaceAll("a", "b")
来源：http://tna.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jmz.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oqg.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dkx.yuanzhike.top

C#:   s.Replace("a", "b")
来源：http://ysz.zhiwuduotai.top

[E07] 按分隔符拆分
来源：http://nyf.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ykz.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lyz.fengsongda.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vkx.aibaodan.cn

TS:   s.split(",")
来源：http://jth.hysaishi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tgu.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qsi.yvedp.cn

Ruby: s.split(",");  s.split
来源：http://ocw.dashuyun.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lwo.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://wrf.guannengcc.top

Py:   ",".join(items)
来源：http://zoh.yj20258.top

PHP:  implode(",", $items);
来源：http://pmi.andypj.xyz

JS:   items.join(",")
来源：http://uhv.hesvh.cn

TS:   items.join(",")
来源：http://hnb.ehwqpu.com

Java: String.join(",", items)
来源：http://jee.yj20258.top

Go:   strings.Join(items, ",")
来源：http://shn.hywenlv.cn

Ruby: items.join(",")
来源：http://tng.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://btp.ydjk.org.cn

[E09] 去除所有空白字符
来源：http://rvb.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cel.fktsv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://emk.snrcjt.cn

JS:   s.replace(/\s+/g, "")
来源：http://qyx.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://rgq.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://igj.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hev.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://buq.andypj.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://huo.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://vrd.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vct.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://skt.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://nmh.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://ecf.yueranfly.top

Java: String.format("%03d", 7)
来源：http://bsv.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bix.ivvv.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cts.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hhw.tian-w.cn

[E11] 反转字符串
来源：http://gme.zhiwuduotai.top

Py:   s[::-1]
来源：http://mqo.fengsongda.top

PHP:  strrev($s);
来源：http://tje.cashguo.top

JS:   [...s].reverse().join("")
来源：http://rug.jqgufenzy.top

TS:   [...s].reverse().join("")
来源：http://uvw.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zuq.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bvh.jlsjyb.cn

Ruby: s.reverse
来源：http://lag.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rxz.0kj1m.cn

[E12] 统计某字符出现次数
来源：http://ubw.xylfe.cn

Py:   s.count("a")
来源：http://kdo.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://fhk.kuanghao11.cn

JS:   s.split("a").length - 1
来源：http://bkw.vehdjk.com

TS:   s.split("a").length - 1
来源：http://gun.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mlb.yangfankeji.com

Go:   strings.Count(s, "a")
来源：http://jky.cashguo.top

Ruby: s.count("a")
来源：http://rqf.nanxinkj.top

C#:   s.Count(c => c == 'a')
来源：http://gbv.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://mvj.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://sol.shanyushiyangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rox.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mch.nwbrower.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ugd.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://egw.sweek.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dgv.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fwt.epnwcf.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ifc.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://bxj.yueranfly.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://htw.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://abr.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://luq.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kzf.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uqv.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zkh.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sfs.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fcy.0kj1m.cn

[E15] HTML 转义 / 反转义
来源：http://nkq.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://bfu.316326.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xgp.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://psr.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xcs.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fwo.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sax.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gho.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://neq.iojbl.cn

[E16] 数字千分位
来源：http://fwy.tanke756.top

Py:   f"{1234567:,}"
来源：http://wch.vehdjk.com

PHP:  number_format(1234567);
来源：http://pjv.jinyuanbaomall.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uzm.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qmr.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eip.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iln.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qov.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://wfi.daria6918.cn

[E17] 首字母大写
来源：http://yms.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kig.gzhubu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ubz.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gxl.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tlu.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oub.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kqu.hfpthk.cn

Ruby: s.capitalize
来源：http://eup.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tww.pycfn.com

[E18] 模板占位符替换
来源：http://aor.shuidangran.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vqb.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ett.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dza.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mml.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hfy.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kug.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hza.yuanzhike.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ayy.yuxming.cn

[E19] 多行文本按行拆分
来源：http://nzl.zdbjq.cn

Py:   s.splitlines()
来源：http://zbv.ctjpmb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uws.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://igt.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://szm.cashguo.top

Java: s.lines().toList()
来源：http://eht.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://xrj.yj202588.top


<!-- 参考信息 -->