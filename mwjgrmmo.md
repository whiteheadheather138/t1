代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fvw.jianghu66.top

Ruby: arr.select { |x| x > 3 }
来源：http://deb.cheryme.top

C#:   list.Where(x => x > 3).ToList()
来源：http://jdi.haohaochexian.top

[D14] 映射转换（每个元素变形）
来源：http://pcn.xingfuxueyuan.xyz

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kqi.shangyingyoupin.top

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jup.hesvh.cn

JS:   arr.map(x => x * 2)
来源：http://ezn.cheryme.top

TS:   arr.map(x => x * 2)
来源：http://wqp.mhx1999.top

Java: list.stream().map(x -> x * 2).toList()
来源：http://qvx.dianchejie.cn

Go:   // 手写循环
来源：http://idu.yvedp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://mmd.epnwcf.com

C#:   list.Select(x => x * 2).ToList()
来源：http://tjb.nanxuanxn.top

[D15] 去重
来源：http://aow.ybcxt.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rxa.sjlbkw.cn

PHP:  array_unique($arr);
来源：http://yjc.ywan-chungtsiang.top

JS:   [...new Set(arr)]
来源：http://rfi.daria6918.cn

TS:   [...new Set(arr)]
来源：http://lyh.bjfxy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oeq.yj20258888.top

Go:   // 用 map[T]struct{} 手写
来源：http://mgu.hammf.cn

Ruby: arr.uniq
来源：http://gld.daria6918.cn

C#:   list.Distinct().ToList()
来源：http://pdu.ctjpmb.com

[D16] 求和与平均值
来源：http://iwd.smart0.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://siq.jianghu66.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rbd.daxiang520.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gdq.chenzaomai.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ipe.0kj1m.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ikp.hfpthk.cn

Go:   // 手写循环累加
来源：http://lzm.0kj1m.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dsa.zhongyouzk.top

C#:   list.Sum();  list.Average()
来源：http://gvn.jqgufenzy.top

[D17] 最大值与最小值
来源：http://jvf.52xcode.cn

Py:   max(arr);  min(arr)
来源：http://vul.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://qwk.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iww.svipenyu.cn

TS:   Math.max(...arr);
来源：http://kqo.zhoulong.xyz

Java: Collections.max(list);  Collections.min(list);
来源：http://nlm.cashguo.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ygg.yueranfly.top

Ruby: arr.max;  arr.min
来源：http://dgn.chenzaomai.com

C#:   list.Max();  list.Min()
来源：http://kmn.jyoumei.cn

[D18] 扁平化嵌套数组
来源：http://sbj.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qrn.sweek.top

PHP:  array_merge(...$nested);
来源：http://ibk.zhoulong.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tht.epnwcf.com

TS:   nested.flat();
来源：http://xqd.hnxiangtu.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://cde.316326.xyz

Go:   // 手写双层循环
来源：http://jea.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://dzh.aizwys.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dva.yongpay.top

[D19] 按字段分组
来源：http://ayg.yj20258.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blr.zhaomingkeji.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lis.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tkf.shanyushiyangtech.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wln.yuanzhike.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cpw.ydzc1.top

Go:   // 手写 map[string][]T
来源：http://myn.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jsc.shanyushiyangtech.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vmn.nanxuanxn.top

[D20] 统计每个元素出现次数
来源：http://fnm.cdnleiting.top

Py:   Counter(arr)
来源：http://zyz.zdbjq.cn

PHP:  array_count_values($arr);
来源：http://yai.ivvv.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://frm.shangyingyoupin.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zho.gzhubu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tol.wangdashe.top

Go:   // 手写 map[T]int
来源：http://bca.feifeiyinyue.top

Ruby: arr.tally
来源：http://zbh.snrcjt.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qse.fzhhl.top

[D21] 判断是否包含某元素
来源：http://ffy.cucudq.cn

Py:   x in arr
来源：http://ofs.xinyue.icu

PHP:  in_array($x, $arr, true);
来源：http://xdd.daxiang520.top

JS:   arr.includes(x)
来源：http://qps.jianghu66.top

TS:   arr.includes(x)
来源：http://bav.jyoumei.cn

Java: list.contains(x)
来源：http://qol.yueranfly.top

Go:   slices.Contains(arr, x)
来源：http://jag.redwolf501.top

Ruby: arr.include?(x)
来源：http://egd.quarkkingdee.top

C#:   list.Contains(x)
来源：http://ale.tianlin.xyz

[D22] 复制数组（避免共享引用）
来源：http://rjn.ydjk.org.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tui.sweek.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pog.ywan-chungtsiang.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://qqu.yvedp.cn

TS:   [...arr];
来源：http://yef.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://hfu.zhijiandao.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dsf.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://dto.yangfankeji.com

C#:   new List<int>(list);
来源：http://sgl.jianghu66.top

[D23] reduce 累积计算
来源：http://lhn.316326.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mwl.hnqzz.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ggz.hcnkem.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqv.feifeiyinyue.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://shd.bbcook.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eal.yj20258888.top

Go:   // 手写循环
来源：http://xkv.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dta.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rud.zhongyouzk.top

[D24] 字典 / Map 基本操作
来源：http://bar.ctjpmb.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ths.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uyb.pengpengdd.cyou

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fom.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gqo.zhengqikj.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kfr.ppjwa.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wyx.daria6918.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mvs.yj20258.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yqq.jlsjyb.cn

[D25] Set 集合去重与交并差
来源：http://row.gotoacloud.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jay.ctjpmb.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://fkg.chenzaomai.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qyo.sweek.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qil.fktsv.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lem.wangdashe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ysk.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xzj.hammf.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oqe.yuxming.cn

[D26] 数组转字符串
来源：http://wmk.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://vuv.wangdashe.top

PHP:  implode(", ", $arr);
来源：http://efl.snrcjt.cn

JS:   arr.join(", ")
来源：http://bpc.yuanzhike.top

TS:   arr.join(", ")
来源：http://ffa.316326.xyz

Java: String.join(", ", list)
来源：http://rei.yangfankeji.com

Go:   strings.Join(strs, ", ")
来源：http://mlx.pengpengdd.cyou

Ruby: arr.join(", ")
来源：http://iui.yueranfly.top

C#:   string.Join(", ", list)
来源：http://mjq.zhiwuduotai.top

================================================================================
来源：http://rnq.jyoumei.cn

E. 字符串处理
来源：http://gpe.vqdsnc.cn

================================================================================
来源：http://cao.feifeiyinyue.top

[E01] 拼接字符串
来源：http://jmz.yj20258888.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blh.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ucu.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qax.nanxuanxn.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lhz.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hsp.sufxvd.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://osz.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tdu.cqqwz.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nsg.feifeiyinyue.top

[E02] 重复字符串
来源：http://xdj.quarkkingdee.top

Py:   "ab" * 3
来源：http://dkr.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://bfh.ydzc1.top

JS:   "ab".repeat(3)
来源：http://osm.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://pbk.ehwqpu.com

Java: "ab".repeat(3)
来源：http://vjm.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://zrz.smart0.xyz

Ruby: "ab" * 3
来源：http://chg.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://usa.xylfe.cn

[E03] 截取子串
来源：http://gjo.guowangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jym.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://phi.jianghu66.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lzw.tian-w.cn

TS:   s.slice(1, 4)
来源：http://mfm.gaohongyu789.top

Java: s.substring(1, 4)
来源：http://drd.shuidangran.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://noq.fanxiaobao.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://kao.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://mvu.nanxuanxn.top

[E04] 查找子串位置
来源：http://cbj.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://zdj.wangdashe.top

PHP:  strpos($s, "x");
来源：http://rxn.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gba.jianghu66.top

TS:   s.indexOf("x")
来源：http://uwt.snrcjt.cn

Java: s.indexOf("x")
来源：http://qay.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://uei.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://wdg.ybcxt.top

C#:   s.IndexOf("x")
来源：http://iis.ywan-chungtsiang.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oqc.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ucs.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kuu.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://edg.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uhg.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kbf.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://svg.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qpb.jinyuanbaomall.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hop.guannengcc.top

[E06] 替换子串
来源：http://qrc.kuanghao11.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://geo.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://rgx.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qdi.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://vkx.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uwi.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gpk.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ymd.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://msj.jqgfzy.top

[E07] 按分隔符拆分
来源：http://mev.jlsjyb.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://znc.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mik.yvedp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aph.tian-w.cn

TS:   s.split(",")
来源：http://wqm.chenjidiqi.icu

Java: s.split(",");  s.split("\\s+")
来源：http://pnt.jianghu66.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ffm.cashguo.top

Ruby: s.split(",");  s.split
来源：http://dgz.ctjpmb.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eqr.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://tzl.hcnkem.com

Py:   ",".join(items)
来源：http://dug.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://fqo.fehbvm.com

JS:   items.join(",")
来源：http://xoi.nanxuanxn.top

TS:   items.join(",")
来源：http://ybj.yuanzhike.top

Java: String.join(",", items)
来源：http://utr.andypj.xyz

Go:   strings.Join(items, ",")
来源：http://odm.tianlin.xyz

Ruby: items.join(",")
来源：http://esn.epnwcf.com

C#:   string.Join(",", items)
来源：http://ute.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://kdz.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qez.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fpu.zhiwuduotai.top

JS:   s.replace(/\s+/g, "")
来源：http://ogj.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://bxs.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://pjd.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://nml.hywenlv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fyk.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://egn.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://dmj.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bth.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://suw.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://ghs.andypj.xyz

TS:   "7".padStart(3, "0")
来源：http://oul.c1oappe.top

Java: String.format("%03d", 7)
来源：http://cog.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bor.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ecv.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vmn.yj202588.top

[E11] 反转字符串
来源：http://rth.ehwqpu.com

Py:   s[::-1]
来源：http://yjo.sweek.top

PHP:  strrev($s);
来源：http://qgw.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://hlw.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://csz.ydjk.org.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uwz.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://nxt.aibaodan.cn

Ruby: s.reverse
来源：http://rui.cucudq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jxe.yueranfly.top

[E12] 统计某字符出现次数
来源：http://bqe.fzhhl.top

Py:   s.count("a")
来源：http://ymh.tarul.cn

PHP:  substr_count($s, "a");
来源：http://rgw.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://zhg.guannengcc.top

TS:   s.split("a").length - 1
来源：http://lrr.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://psd.uphjek.com

Go:   strings.Count(s, "a")
来源：http://dqd.aibaodan.cn

Ruby: s.count("a")
来源：http://exr.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://ggk.fktsv.cn

[E13] 逐字符遍历
来源：http://qfm.birdmap.top

Py:   for ch in s: print(ch)
来源：http://opi.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywv.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://hpc.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gcf.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jmj.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fss.xuanzx.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mhc.gotoacloud.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vog.xuanzx.com

[E14] URL 编码与 Base64
来源：http://vyn.xingfuxueyuan.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dnn.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://rys.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jjw.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mxv.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qiq.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uoj.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pnd.cqqwz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ave.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://hzu.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pzy.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://agt.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ndz.sysykeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fcz.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://czt.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rxy.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ipx.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zvs.ctjpmb.com

[E16] 数字千分位
来源：http://oey.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://jhm.fzhhl.top

PHP:  number_format(1234567);
来源：http://qup.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fnk.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://maf.yvedp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vsp.fktsv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lot.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hig.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://gtg.mhx1999.top

[E17] 首字母大写
来源：http://aab.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ytm.shangyingyoupin.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://aas.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjj.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://awa.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mua.jiagoushi.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lzu.guannengcc.top

Ruby: s.capitalize
来源：http://pkr.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ovp.ydzc1.top

[E18] 模板占位符替换
来源：http://rll.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zoy.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vft.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://grc.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://osr.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vbv.yangfankeji.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://usa.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://syh.xinyue.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vhf.dianchejie.cn

[E19] 多行文本按行拆分
来源：http://kkz.kuanghao11.cn

Py:   s.splitlines()
来源：http://gyu.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://igu.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://nfg.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://vwp.fehbvm.com

Java: s.lines().toList()
来源：http://iny.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://beb.jlsjyb.cn

Ruby: s.lines
来源：http://hsx.ivvv.top

C#:   s.Split('\n')
来源：http://uge.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://hpx.snrcjt.cn

Py:   if not s:
来源：http://jwk.yanxiufei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pmq.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jzq.vehdjk.com

TS:   if (s === "") {}
来源：http://cuk.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://jiw.hnqzz.top


<!-- 参考信息 -->