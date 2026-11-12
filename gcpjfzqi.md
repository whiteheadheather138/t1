代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://qbp.pengpengdd.cyou

C#:   list.Sum();  list.Average()
来源：http://kbr.meibo888.top

[D17] 最大值与最小值
来源：http://ctd.meibo888.top

Py:   max(arr);  min(arr)
来源：http://aek.gotoacloud.top

PHP:  max($arr);  min($arr);
来源：http://mcc.guannengcc.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zzb.tanke756.top

TS:   Math.max(...arr);
来源：http://wdj.ydzc1.top

Java: Collections.max(list);  Collections.min(list);
来源：http://mwv.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dnt.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://bih.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://gov.daria6918.cn

[D18] 扁平化嵌套数组
来源：http://jls.jinqigufen.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wke.haohaochexian.top

PHP:  array_merge(...$nested);
来源：http://ovu.gaohongyu789.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uuv.xinyue.icu

TS:   nested.flat();
来源：http://laj.guowangkeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wal.ctjpmb.com

Go:   // 手写双层循环
来源：http://rgw.nwbrower.top

Ruby: nested.flatten
来源：http://quq.haohaochexian.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://itw.tian-w.cn

[D19] 按字段分组
来源：http://fqg.9152youxi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zfs.gotoacloud.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kka.jinyuanbaomall.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ykr.shanyushiyangkeji.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nhe.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xhp.jlsjyb.cn

Go:   // 手写 map[string][]T
来源：http://fdc.cheryme.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sem.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://psz.cashguo.top

[D20] 统计每个元素出现次数
来源：http://hti.fehbvm.com

Py:   Counter(arr)
来源：http://arq.daria6918.cn

PHP:  array_count_values($arr);
来源：http://lav.hnxiangtu.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xlo.hnqzz.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lim.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wgr.meibo888.top

Go:   // 手写 map[T]int
来源：http://bhg.vehdjk.com

Ruby: arr.tally
来源：http://mcr.nanxinkj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qcd.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://bsq.xuanzx.com

Py:   x in arr
来源：http://wlq.fengsongda.top

PHP:  in_array($x, $arr, true);
来源：http://bwk.zhoulong.xyz

JS:   arr.includes(x)
来源：http://zut.fengsongda.top

TS:   arr.includes(x)
来源：http://ejw.pycfn.com

Java: list.contains(x)
来源：http://ivl.9152youxi.cn

Go:   slices.Contains(arr, x)
来源：http://eyv.hywenlv.cn

Ruby: arr.include?(x)
来源：http://izi.sxryk.cn

C#:   list.Contains(x)
来源：http://nsk.zhijiandao.cn

[D22] 复制数组（避免共享引用）
来源：http://jxb.sxryk.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dbj.meibo888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xkz.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ngh.meibo888.top

TS:   [...arr];
来源：http://ufz.hnxiangtu.top

Java: new ArrayList<>(list);
来源：http://adz.zhiwuduotai.top

Go:   copied := append([]int(nil), arr...)
来源：http://ykb.ydjk.org.cn

Ruby: arr.dup;  arr.clone
来源：http://dcr.cdnleiting.top

C#:   new List<int>(list);
来源：http://auz.hcnkem.com

[D23] reduce 累积计算
来源：http://rvn.jinghuilouyu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://asn.yj20258888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hfx.xinyue.icu

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wui.nanxinkj.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hdn.ybcxt.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://oxm.chenlongwang.top

Go:   // 手写循环
来源：http://dyv.gotoacloud.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yye.yj20258.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nvu.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://syh.fzhhl.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://srb.wangshuangyany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wqp.ydjk.org.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hdl.jinqigfzy.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gvf.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xpr.pycfn.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ujv.nanxuanxn.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cqc.sxryk.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vob.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://rqw.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://trt.feifeiyinyue.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uso.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hrp.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kcs.xinyue.icu

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vzt.gaohongyu789.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gef.guowangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mwi.dashuyun.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xuo.chenjidiqi.icu

[D26] 数组转字符串
来源：http://mfk.ywan-chungtsiang.top

Py:   ", ".join(map(str, arr))
来源：http://hrv.jianghu66.top

PHP:  implode(", ", $arr);
来源：http://alv.0kj1m.cn

JS:   arr.join(", ")
来源：http://gma.316326.xyz

TS:   arr.join(", ")
来源：http://yqb.xuanzx.com

Java: String.join(", ", list)
来源：http://gbs.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://tyb.yfazqb.com

Ruby: arr.join(", ")
来源：http://sdy.gzhubu.top

C#:   string.Join(", ", list)
来源：http://lpg.yueranfly.top

================================================================================
来源：http://dsm.shangyingyoupin.top

E. 字符串处理
来源：http://zvm.fengsongda.top

================================================================================
来源：http://jqc.fehbvm.com

[E01] 拼接字符串
来源：http://uzj.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dbw.epnwcf.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qgu.hfpthk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://umx.iojbl.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://iiq.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lnt.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vjj.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mdq.0kj1m.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gra.cdnleiting.top

[E02] 重复字符串
来源：http://poa.cqqwz.cn

Py:   "ab" * 3
来源：http://kji.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://tqt.316326.xyz

JS:   "ab".repeat(3)
来源：http://vui.smart0.xyz

TS:   "ab".repeat(3)
来源：http://nyc.zdbjq.cn

Java: "ab".repeat(3)
来源：http://obd.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://vzy.pycfn.com

Ruby: "ab" * 3
来源：http://ghz.yj20258.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mst.ivvv.top

[E03] 截取子串
来源：http://wcf.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://woq.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nes.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://oga.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://pek.fengsongda.top

Java: s.substring(1, 4)
来源：http://ssb.fehbvm.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://faa.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://msx.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://nmb.kuanghao11.cn

[E04] 查找子串位置
来源：http://tec.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://iad.0kj1m.cn

PHP:  strpos($s, "x");
来源：http://mmi.yonumen.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kia.nanxinkj.top

TS:   s.indexOf("x")
来源：http://zgq.hcnkem.com

Java: s.indexOf("x")
来源：http://zxl.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://wfb.xziqi.cn

Ruby: s.index("x")
来源：http://vtv.chenzaomai.com

C#:   s.IndexOf("x")
来源：http://ien.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jtm.9152youxi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://min.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qwy.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tpv.hongshengwenyu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gyp.bjfxy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hfo.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://avu.sxryk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bft.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ohx.nanxinkj.top

[E06] 替换子串
来源：http://zvo.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rzq.bjfxy.top

PHP:  str_replace("a", "b", $s);
来源：http://hnv.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kqt.chenzaomai.com

TS:   s.replaceAll("a", "b")
来源：http://haf.nanxuanxn.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mfs.fktsv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mha.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://suu.ydjk.org.cn

C#:   s.Replace("a", "b")
来源：http://pwk.yuanzhike.top

[E07] 按分隔符拆分
来源：http://xvx.gzhubu.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pev.jinghuilouyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ggn.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://bga.tanke756.top

TS:   s.split(",")
来源：http://xwe.c1oappe.top

Java: s.split(",");  s.split("\\s+")
来源：http://tnj.nwbrower.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://psg.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://ulr.yvedp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://srv.guowangkeji.top

[E08] 数组按分隔符合并
来源：http://qqy.hcnkem.com

Py:   ",".join(items)
来源：http://rkw.yj20258.top

PHP:  implode(",", $items);
来源：http://unw.zhijiandao.cn

JS:   items.join(",")
来源：http://nbr.svipenyu.cn

TS:   items.join(",")
来源：http://cbn.bjfxy.top

Java: String.join(",", items)
来源：http://qsb.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://ymj.hnxiangtu.top

Ruby: items.join(",")
来源：http://wlz.meibo888.top

C#:   string.Join(",", items)
来源：http://uyb.andypj.xyz

[E09] 去除所有空白字符
来源：http://sym.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mjy.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bld.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ccn.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://iil.hnqzz.top

Java: s.replaceAll("\\s+", "")
来源：http://nom.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://acg.shzxlz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pwb.aizwys.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ypp.fehbvm.com

[E10] 左侧补零 / 定长填充
来源：http://dgm.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://scy.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fqs.yj20258888.top

JS:   "7".padStart(3, "0")
来源：http://pxw.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://wox.daxiang520.top

Java: String.format("%03d", 7)
来源：http://vkv.bjfxy.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mca.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jzv.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ykn.hysaishi.cn

[E11] 反转字符串
来源：http://toy.jqgfzy.top

Py:   s[::-1]
来源：http://auf.epnwcf.com

PHP:  strrev($s);
来源：http://uxf.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://ufy.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://urm.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://skw.andypj.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://nxe.cashguo.top

Ruby: s.reverse
来源：http://pqc.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://bef.sysykeji.top

[E12] 统计某字符出现次数
来源：http://rba.cucudq.cn

Py:   s.count("a")
来源：http://fqf.yj20258.top

PHP:  substr_count($s, "a");
来源：http://ngj.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://qzm.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://gtx.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fdc.epnwcf.com

Go:   strings.Count(s, "a")
来源：http://kad.fzhhl.top

Ruby: s.count("a")
来源：http://gxc.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://mlp.bjfxy.top

[E13] 逐字符遍历
来源：http://mim.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://cnq.smart0.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gnt.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nts.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vbc.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gjy.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tdx.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ofg.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bfm.tarul.cn

[E14] URL 编码与 Base64
来源：http://pne.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lxx.vqdsnc.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xng.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://exm.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://srz.zdqjudy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gkm.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://klr.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mot.zhengqikj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://suy.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://vqf.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gir.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://klr.aizwys.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wpy.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ycb.nwbrower.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qfm.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jiq.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dxf.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kau.zhoulong.xyz

[E16] 数字千分位
来源：http://vfx.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://axt.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://toe.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vnd.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dgy.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kll.guowangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zip.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wuf.yj202588.top

C#:   1234567.ToString("N0")
来源：http://uas.ehwqpu.com

[E17] 首字母大写
来源：http://yfd.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ori.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vjs.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lzo.yangfankeji.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lww.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zmo.sxryk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ene.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://tln.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yxc.0kj1m.cn

[E18] 模板占位符替换
来源：http://zpi.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tls.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ovs.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cio.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xxb.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ols.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://leu.gzhubu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ekx.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bhy.iojbl.cn

[E19] 多行文本按行拆分
来源：http://nnl.cdnleiting.top

Py:   s.splitlines()
来源：http://gfn.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ful.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://rsa.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://qwi.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://uyi.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://rej.cdnleiting.top

Ruby: s.lines
来源：http://erz.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://zid.ctjpmb.com

[E20] 判断字符串是否为空
来源：http://qog.yj202588.top

Py:   if not s:
来源：http://bfw.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gvp.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dzl.yueranfly.top

TS:   if (s === "") {}
来源：http://mfg.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://mek.yuanzhike.top

Go:   if s == "" {}
来源：http://shy.svipenyu.cn

Ruby: if s.empty?
来源：http://bch.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rco.andypj.xyz

[E21] 超长截断加省略号
来源：http://eol.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wzn.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hni.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vmv.daria6918.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyt.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wyw.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://rcq.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://liz.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xvw.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://znf.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ysy.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sob.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ijx.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oaq.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jjd.sxryk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hzs.svipenyu.cn

Ruby: s.bytesize;  s.length
来源：http://sjw.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ydg.wangdashe.top

================================================================================
来源：http://azd.cheryme.top

F. 文件与目录
来源：http://gcv.c1oappe.top

================================================================================
来源：http://wbc.c1oappe.top

[F01] 读取整个文件
来源：http://exc.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nac.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://yiu.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hhx.sjlbkw.cn


<!-- 参考信息 -->