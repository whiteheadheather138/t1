代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hcr.hcnkem.com

Ruby: arr.select { |x| x > 3 }
来源：http://qck.yj20258888.top

C#:   list.Where(x => x > 3).ToList()
来源：http://mip.shanyushiyangkeji.top

[D14] 映射转换（每个元素变形）
来源：http://spo.xuetiantiany.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qge.meibo888.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ggw.tian-w.cn

JS:   arr.map(x => x * 2)
来源：http://jqa.tanke756.top

TS:   arr.map(x => x * 2)
来源：http://zej.0kj1m.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pzy.sufxvd.cn

Go:   // 手写循环
来源：http://olm.hongshengwenyu.top

Ruby: arr.map { |x| x * 2 }
来源：http://ngb.yuanzhike.top

C#:   list.Select(x => x * 2).ToList()
来源：http://exp.sufxvd.cn

[D15] 去重
来源：http://cae.ywan-chungtsiang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ojw.shanyushiyangtech.top

PHP:  array_unique($arr);
来源：http://upk.xuetiantiany.cn

JS:   [...new Set(arr)]
来源：http://jgh.cdnleiting.top

TS:   [...new Set(arr)]
来源：http://hno.daria6918.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bya.yj20258.top

Go:   // 用 map[T]struct{} 手写
来源：http://brs.ywan-chungtsiang.top

Ruby: arr.uniq
来源：http://syz.birdmap.top

C#:   list.Distinct().ToList()
来源：http://dsw.redwolf501.top

[D16] 求和与平均值
来源：http://khm.hammf.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qyx.ppjwa.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vrm.sxryk.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fjj.jinghuilouyu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tmg.ybcxt.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rqx.shuidangran.top

Go:   // 手写循环累加
来源：http://mpy.zhiwuduotai.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bje.fanxiaobao.xyz

C#:   list.Sum();  list.Average()
来源：http://feu.redwolf501.top

[D17] 最大值与最小值
来源：http://rpk.jianghu66.top

Py:   max(arr);  min(arr)
来源：http://slf.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://cqt.jinghuilouyu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://llq.hysaishi.cn

TS:   Math.max(...arr);
来源：http://fys.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ysl.zdbjq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dxd.cheryme.top

Ruby: arr.max;  arr.min
来源：http://huu.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://eui.cucudq.cn

[D18] 扁平化嵌套数组
来源：http://zjt.tarul.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://thv.svipenyu.cn

PHP:  array_merge(...$nested);
来源：http://ysb.daxiang520.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://glg.birdmap.top

TS:   nested.flat();
来源：http://wjb.hesvh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://xwb.jqgufenzy.top

Go:   // 手写双层循环
来源：http://nci.feifeiyinyue.top

Ruby: nested.flatten
来源：http://ksg.quarkkingdee.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://nka.tarul.cn

[D19] 按字段分组
来源：http://myt.hnxiangtu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wfb.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ltt.0kj1m.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iau.dianchejie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nja.hongshengwenyu.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lro.havefunace.top

Go:   // 手写 map[string][]T
来源：http://set.hywenlv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://agt.hongshengwenyu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tsz.uphjek.com

[D20] 统计每个元素出现次数
来源：http://plv.mhx1999.top

Py:   Counter(arr)
来源：http://tih.tarul.cn

PHP:  array_count_values($arr);
来源：http://jce.yonumen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ysp.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sgi.hesvh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ufn.fktsv.cn

Go:   // 手写 map[T]int
来源：http://ihq.yanxiufei.cn

Ruby: arr.tally
来源：http://uof.yj20258.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mff.c1oappe.top

[D21] 判断是否包含某元素
来源：http://kza.jinqigfzy.top

Py:   x in arr
来源：http://dox.yongpay.top

PHP:  in_array($x, $arr, true);
来源：http://uuf.pengpengdd.cyou

JS:   arr.includes(x)
来源：http://leq.feifeiyinyue.top

TS:   arr.includes(x)
来源：http://zxa.jianghu66.top

Java: list.contains(x)
来源：http://rhg.yongpay.top

Go:   slices.Contains(arr, x)
来源：http://dot.yfazqb.com

Ruby: arr.include?(x)
来源：http://qlb.ywan-chungtsiang.top

C#:   list.Contains(x)
来源：http://vbh.52xcode.cn

[D22] 复制数组（避免共享引用）
来源：http://vge.yj20258888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ugq.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vpq.tanke756.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ryi.hnxiangtu.top

TS:   [...arr];
来源：http://lcv.hywenlv.cn

Java: new ArrayList<>(list);
来源：http://esx.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://faj.nanxinkj.top

Ruby: arr.dup;  arr.clone
来源：http://ftf.jianghu66.top

C#:   new List<int>(list);
来源：http://auv.yuxming.cn

[D23] reduce 累积计算
来源：http://nbw.shzxlz.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://vah.zhiwuduotai.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iie.ywan-chungtsiang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://thh.jianghu66.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pjv.xylfe.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgh.chenlongwang.top

Go:   // 手写循环
来源：http://qpq.sysykeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cls.9152youxi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tft.sjlbkw.cn

[D24] 字典 / Map 基本操作
来源：http://mnm.bbcook.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ybi.zhixingplan.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qng.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://huh.guannengcc.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iff.9152youxi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cxi.dianchejie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://oqt.vqdsnc.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ggh.zhixingplan.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://els.fehbvm.com

[D25] Set 集合去重与交并差
来源：http://ubd.yfazqb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kud.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aas.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vfc.zhaomingkeji.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ynq.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rfi.nanxinkj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://amw.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kun.c1oappe.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dqs.9152youxi.cn

[D26] 数组转字符串
来源：http://pyf.cashguo.top

Py:   ", ".join(map(str, arr))
来源：http://tme.fehbvm.com

PHP:  implode(", ", $arr);
来源：http://bux.zdqjudy.top

JS:   arr.join(", ")
来源：http://rtx.tarul.cn

TS:   arr.join(", ")
来源：http://iyd.nwbrower.top

Java: String.join(", ", list)
来源：http://yjg.meibo888.top

Go:   strings.Join(strs, ", ")
来源：http://jlv.ydzc1.top

Ruby: arr.join(", ")
来源：http://due.yonumen.top

C#:   string.Join(", ", list)
来源：http://aqi.9152youxi.cn

================================================================================
来源：http://zsu.chenlongwang.top

E. 字符串处理
来源：http://zvy.svipenyu.cn

================================================================================
来源：http://ssb.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://hig.xuanzx.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dbe.havefunace.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sya.epnwcf.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oxw.guannengcc.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tsp.shanyushiyangkeji.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xjl.chenjidiqi.icu

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://djv.gzhubu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rql.zhijiandao.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxl.bbcook.cn

[E02] 重复字符串
来源：http://spy.yangfankeji.com

Py:   "ab" * 3
来源：http://ttt.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://kxh.gogol.net.cn

JS:   "ab".repeat(3)
来源：http://rii.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://kqw.xuetiantiany.cn

Java: "ab".repeat(3)
来源：http://zpj.c1oappe.top

Go:   strings.Repeat("ab", 3)
来源：http://wky.shanyushiyangkeji.top

Ruby: "ab" * 3
来源：http://cwt.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xek.hnxiangtu.top

[E03] 截取子串
来源：http://una.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qzh.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://krb.cqqwz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://slv.yj20258888.top

TS:   s.slice(1, 4)
来源：http://okp.yj20258888.top

Java: s.substring(1, 4)
来源：http://qig.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://aoc.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://lmn.jqgfzy.top

C#:   s.Substring(1, 3)
来源：http://mrv.chenzaomai.com

[E04] 查找子串位置
来源：http://ywh.tianlin.xyz

Py:   s.find("x");  s.index("x")
来源：http://anr.gotoacloud.top

PHP:  strpos($s, "x");
来源：http://hvr.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qlk.bjfxy.top

TS:   s.indexOf("x")
来源：http://cip.cqqwz.cn

Java: s.indexOf("x")
来源：http://jio.hnxiangtu.top

Go:   strings.Index(s, "x")
来源：http://fik.cucudq.cn

Ruby: s.index("x")
来源：http://hnm.jyoumei.cn

C#:   s.IndexOf("x")
来源：http://gtu.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ncm.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://txk.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bzp.ctjpmb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yra.cucudq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oos.nanxuanxn.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://evf.haohaochexian.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xsc.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qqf.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ymz.hammf.cn

[E06] 替换子串
来源：http://mbf.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wvr.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://qya.yvedp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://srm.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://jvv.kuanghao11.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgk.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xde.zhiwuduotai.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yis.sweek.top

C#:   s.Replace("a", "b")
来源：http://kak.shzxlz.cn

[E07] 按分隔符拆分
来源：http://yvd.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bam.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hqd.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ytt.bjfxy.top

TS:   s.split(",")
来源：http://utt.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://sic.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yqs.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://rkg.xuetiantiany.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mcm.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://xfi.sweek.top

Py:   ",".join(items)
来源：http://wai.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://wxq.pengpengdd.cyou

JS:   items.join(",")
来源：http://asy.hammf.cn

TS:   items.join(",")
来源：http://cad.uphjek.com

Java: String.join(",", items)
来源：http://lsn.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://msc.9152youxi.cn

Ruby: items.join(",")
来源：http://stx.yongpay.top

C#:   string.Join(",", items)
来源：http://gnx.guannengcc.top

[E09] 去除所有空白字符
来源：http://czl.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gki.shangyingyoupin.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jal.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://fcy.9152youxi.cn

TS:   s.replace(/\s+/g, "")
来源：http://mvo.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://yow.shangyingyoupin.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nrk.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://lvr.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cvh.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://zbj.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dpp.shanyushiyangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sqi.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://mof.gzhubu.top

TS:   "7".padStart(3, "0")
来源：http://jbw.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://uql.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tlz.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://reh.yueranfly.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fus.c1oappe.top

[E11] 反转字符串
来源：http://wiq.epnwcf.com

Py:   s[::-1]
来源：http://plv.aibaodan.cn

PHP:  strrev($s);
来源：http://ciz.yanxiufei.cn

JS:   [...s].reverse().join("")
来源：http://pwv.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://biv.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wrk.wangshuangyany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rhb.guowangkeji.top

Ruby: s.reverse
来源：http://tik.guannengcc.top

C#:   new string(s.Reverse().ToArray())
来源：http://nza.fktsv.cn

[E12] 统计某字符出现次数
来源：http://thu.kuanghao11.cn

Py:   s.count("a")
来源：http://iug.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://txh.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://wtq.jinqigfzy.top

TS:   s.split("a").length - 1
来源：http://tof.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jwn.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://edx.0kj1m.cn

Ruby: s.count("a")
来源：http://pal.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://iqp.sufxvd.cn

[E13] 逐字符遍历
来源：http://hyr.xylfe.cn

Py:   for ch in s: print(ch)
来源：http://kgi.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gwn.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hww.iojbl.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nzx.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ncp.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://itt.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zdn.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xis.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://cdu.zhongyouzk.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tqn.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xwt.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vjv.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vlh.jlsjyb.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qba.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zfj.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qop.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lty.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://mlu.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rup.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hic.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mew.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gvg.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bog.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ypo.sysykeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sgj.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mky.yuxming.cn

[E16] 数字千分位
来源：http://ctt.jiagoushi.top

Py:   f"{1234567:,}"
来源：http://tpr.redwolf501.top

PHP:  number_format(1234567);
来源：http://uir.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jrq.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ujl.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iiv.yangfankeji.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tst.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pug.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://cqd.ydjk.org.cn

[E17] 首字母大写
来源：http://pbv.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xyp.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aot.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pzg.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qvm.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qlw.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ihl.nanxinkj.top

Ruby: s.capitalize
来源：http://xok.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bud.gotoacloud.top

[E18] 模板占位符替换
来源：http://sir.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eyu.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bfo.chenlongwang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dmo.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dgq.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://amv.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ihq.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://epb.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gte.mhx1999.top

[E19] 多行文本按行拆分
来源：http://opt.tian-w.cn

Py:   s.splitlines()
来源：http://sfe.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://anz.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://gvu.sweek.top

TS:   s.split(/\r?\n/)
来源：http://toi.epnwcf.com

Java: s.lines().toList()
来源：http://irk.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://rko.xylfe.cn

Ruby: s.lines
来源：http://ufz.yangfankeji.com

C#:   s.Split('\n')
来源：http://gvg.yvedp.cn

[E20] 判断字符串是否为空
来源：http://uga.iojbl.cn

Py:   if not s:
来源：http://ouw.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lhd.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nwb.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://tus.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://ojs.dianchejie.cn


<!-- 参考信息 -->