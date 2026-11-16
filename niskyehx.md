代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://hun.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ian.tanke756.top

TS:   Math.max(...arr);
来源：http://ark.gotoacloud.top

Java: Collections.max(list);  Collections.min(list);
来源：http://wsp.gzhubu.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://omj.ppjwa.cn

Ruby: arr.max;  arr.min
来源：http://moq.zhixingplan.top

C#:   list.Max();  list.Min()
来源：http://elv.bjfxy.top

[D18] 扁平化嵌套数组
来源：http://mlm.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eko.yuxming.cn

PHP:  array_merge(...$nested);
来源：http://ppy.svipenyu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gbp.iojbl.cn

TS:   nested.flat();
来源：http://geb.sxryk.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://src.tianlin.xyz

Go:   // 手写双层循环
来源：http://qds.shanyushiyangtech.top

Ruby: nested.flatten
来源：http://bhc.gotoacloud.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ivw.jyoumei.cn

[D19] 按字段分组
来源：http://sxu.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nrk.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hde.haohaochexian.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yiw.kuanghao11.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qfm.wangdashe.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qny.zhixingplan.top

Go:   // 手写 map[string][]T
来源：http://esl.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://sjl.vehdjk.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bss.birdmap.top

[D20] 统计每个元素出现次数
来源：http://bcw.hcnkem.com

Py:   Counter(arr)
来源：http://zlh.316326.xyz

PHP:  array_count_values($arr);
来源：http://yjx.wangshuangyany.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oet.yueranfly.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://abc.hfpthk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kqh.jianghu66.top

Go:   // 手写 map[T]int
来源：http://jkh.yfazqb.com

Ruby: arr.tally
来源：http://aps.hywenlv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://swu.xylfe.cn

[D21] 判断是否包含某元素
来源：http://vqc.chenjidiqi.icu

Py:   x in arr
来源：http://jgf.nanxinkj.top

PHP:  in_array($x, $arr, true);
来源：http://lmm.xuanzx.com

JS:   arr.includes(x)
来源：http://zyq.ybcxt.top

TS:   arr.includes(x)
来源：http://gvg.hfpthk.cn

Java: list.contains(x)
来源：http://qen.xinyue.icu

Go:   slices.Contains(arr, x)
来源：http://rps.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://tki.jinqigufen.top

C#:   list.Contains(x)
来源：http://avi.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://mxy.vqdsnc.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oys.andypj.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ezr.uphjek.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://grk.jinyuanbaomall.cn

TS:   [...arr];
来源：http://kvb.daria6918.cn

Java: new ArrayList<>(list);
来源：http://mmi.zhixingplan.top

Go:   copied := append([]int(nil), arr...)
来源：http://mdm.ywan-chungtsiang.top

Ruby: arr.dup;  arr.clone
来源：http://gro.uphjek.com

C#:   new List<int>(list);
来源：http://bhn.zhaomingkeji.xyz

[D23] reduce 累积计算
来源：http://izq.pengpengdd.cyou

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dai.zhongyouzk.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jjy.wangdashe.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqp.zdbjq.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fdt.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://grw.wangdashe.top

Go:   // 手写循环
来源：http://qkv.fanxiaobao.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nwh.smart0.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://djn.zhijiandao.cn

[D24] 字典 / Map 基本操作
来源：http://myw.tian-w.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mlb.daxiang520.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zch.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://swl.ydjk.org.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pjm.svipenyu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ufo.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kue.jianghu66.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wlo.9152youxi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qgq.9152youxi.cn

[D25] Set 集合去重与交并差
来源：http://nvt.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ncv.guowangkeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zuz.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yll.nwbrower.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wiv.ehwqpu.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hbc.yj20258888.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zim.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ure.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ttq.ctjpmb.com

[D26] 数组转字符串
来源：http://mto.zhongyouzk.top

Py:   ", ".join(map(str, arr))
来源：http://ejp.nanxinkj.top

PHP:  implode(", ", $arr);
来源：http://odf.yfazqb.com

JS:   arr.join(", ")
来源：http://rfb.sysykeji.top

TS:   arr.join(", ")
来源：http://goa.sjlbkw.cn

Java: String.join(", ", list)
来源：http://yhz.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://uza.dianchejie.cn

Ruby: arr.join(", ")
来源：http://vwn.zhiwuduotai.top

C#:   string.Join(", ", list)
来源：http://prk.svipenyu.cn

================================================================================
来源：http://rrn.316326.xyz

E. 字符串处理
来源：http://tjq.epnwcf.com

================================================================================
来源：http://tdc.andypj.xyz

[E01] 拼接字符串
来源：http://xjv.jqgufenzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fkm.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tod.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ymd.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://icu.jlsjyb.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://skq.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fba.jianghu66.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uog.iojbl.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kfv.shanyushiyangtech.top

[E02] 重复字符串
来源：http://pqn.tarul.cn

Py:   "ab" * 3
来源：http://jrs.wangdashe.top

PHP:  str_repeat("ab", 3);
来源：http://bus.ybcxt.top

JS:   "ab".repeat(3)
来源：http://ryr.zhongyouzk.top

TS:   "ab".repeat(3)
来源：http://cvc.yonumen.top

Java: "ab".repeat(3)
来源：http://ult.316326.xyz

Go:   strings.Repeat("ab", 3)
来源：http://mph.gzhubu.top

Ruby: "ab" * 3
来源：http://vbt.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fgc.hnqzz.top

[E03] 截取子串
来源：http://gvu.chenzaomai.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hvf.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vtt.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bro.quarkkingdee.top

TS:   s.slice(1, 4)
来源：http://yrj.cheryme.top

Java: s.substring(1, 4)
来源：http://bqu.9152youxi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jze.yj202588.top

Ruby: s[1, 3];  s[1..3]
来源：http://ojp.yuanzhike.top

C#:   s.Substring(1, 3)
来源：http://wnv.shzxlz.cn

[E04] 查找子串位置
来源：http://sdz.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://jzp.cucudq.cn

PHP:  strpos($s, "x");
来源：http://ugj.hammf.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dwo.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://nkt.xylfe.cn

Java: s.indexOf("x")
来源：http://asi.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://gvb.hysaishi.cn

Ruby: s.index("x")
来源：http://fmw.gzhubu.top

C#:   s.IndexOf("x")
来源：http://xmh.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jnh.sysykeji.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mpj.shzxlz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zzm.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmt.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bnj.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vti.yj20258.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rqf.tianlin.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xla.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nor.tianlin.xyz

[E06] 替换子串
来源：http://qlu.gotoacloud.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ytt.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://pbx.aibaodan.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tax.wangdashe.top

TS:   s.replaceAll("a", "b")
来源：http://gck.gogol.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jbx.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tdj.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bku.chenlongwang.top

C#:   s.Replace("a", "b")
来源：http://myc.tanke756.top

[E07] 按分隔符拆分
来源：http://qud.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jgs.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hwg.xziqi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zxi.jinghuilouyu.cn

TS:   s.split(",")
来源：http://wwl.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fcb.gotoacloud.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cwm.316326.xyz

Ruby: s.split(",");  s.split
来源：http://nyv.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://juk.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://you.yj20258888.top

Py:   ",".join(items)
来源：http://fry.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://zub.cheryme.top

JS:   items.join(",")
来源：http://cge.yj20258888.top

TS:   items.join(",")
来源：http://gdf.zhijiandao.cn

Java: String.join(",", items)
来源：http://uhc.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://lww.iojbl.cn

Ruby: items.join(",")
来源：http://vmi.shzxlz.cn

C#:   string.Join(",", items)
来源：http://qjf.daxiang520.top

[E09] 去除所有空白字符
来源：http://aof.chenzaomai.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zuv.tanke756.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://chh.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://uqg.feifeiyinyue.top

TS:   s.replace(/\s+/g, "")
来源：http://uhu.pycfn.com

Java: s.replaceAll("\\s+", "")
来源：http://zuh.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qmc.pengpengdd.cyou

Ruby: s.gsub(/\s+/, "")
来源：http://akk.tianlin.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hzu.ywan-chungtsiang.top

[E10] 左侧补零 / 定长填充
来源：http://jqj.xuanzx.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pgu.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vch.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://uim.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://qab.c1oappe.top

Java: String.format("%03d", 7)
来源：http://maq.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://oxn.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ayz.52xcode.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qgw.hesvh.cn

[E11] 反转字符串
来源：http://qlv.yangfankeji.com

Py:   s[::-1]
来源：http://zkd.dashuyun.cn

PHP:  strrev($s);
来源：http://mne.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://shq.cdnleiting.top

TS:   [...s].reverse().join("")
来源：http://fdc.sjlbkw.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://doy.jqgufenzy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qxo.hfpthk.cn

Ruby: s.reverse
来源：http://uwq.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://jzv.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://bvm.tianlin.xyz

Py:   s.count("a")
来源：http://bgp.jianghu66.top

PHP:  substr_count($s, "a");
来源：http://xfe.zhoulong.xyz

JS:   s.split("a").length - 1
来源：http://ldt.mhx1999.top

TS:   s.split("a").length - 1
来源：http://jgm.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ava.cheryme.top

Go:   strings.Count(s, "a")
来源：http://yva.bbcook.cn

Ruby: s.count("a")
来源：http://kix.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://tlj.jinqigufen.top

[E13] 逐字符遍历
来源：http://vtt.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://fjd.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://crz.shanyushiyangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdm.ehwqpu.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fda.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hca.jqgufenzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vdx.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://off.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vms.zhixingplan.top

[E14] URL 编码与 Base64
来源：http://lty.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xsy.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xld.yuanzhike.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gwi.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://abi.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fnd.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vor.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rha.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uqi.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://azs.jyoumei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gzd.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://obi.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kfu.xinyue.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://efg.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fvm.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mol.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pgr.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hwr.smart0.xyz

[E16] 数字千分位
来源：http://lzr.sxryk.cn

Py:   f"{1234567:,}"
来源：http://jbh.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://qwr.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pzb.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zxn.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jup.cucudq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fki.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bvv.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://qyh.hammf.cn

[E17] 首字母大写
来源：http://ubn.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xrx.c1oappe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wtf.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xqx.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwb.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hnk.ppjwa.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kiz.hammf.cn

Ruby: s.capitalize
来源：http://nly.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dwl.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://byk.jyoumei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tzu.yvedp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zpa.svipenyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lpk.9152youxi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://spz.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rxw.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yhj.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://irj.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qgq.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://tpj.hammf.cn

Py:   s.splitlines()
来源：http://tct.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dak.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://naq.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://iya.cheryme.top

Java: s.lines().toList()
来源：http://ngy.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://zzg.guowangkeji.top

Ruby: s.lines
来源：http://raq.yj20258888.top

C#:   s.Split('\n')
来源：http://eqa.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://uun.ehwqpu.com

Py:   if not s:
来源：http://obf.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bpd.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bya.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://pym.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://bpz.yj20258888.top

Go:   if s == "" {}
来源：http://vxh.gogol.net.cn

Ruby: if s.empty?
来源：http://uqt.shuidangran.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oox.ydzc1.top

[E21] 超长截断加省略号
来源：http://tvb.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bnj.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pty.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eth.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nzm.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gmy.ydjk.org.cn

Go:   // 按 rune 判断长度后截断
来源：http://zog.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnq.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kgf.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://qpy.yuanzhike.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nax.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rfr.shuidangran.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oay.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rrh.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rax.zhongyouzk.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vuq.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://oob.xinyue.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nhn.cheryme.top

================================================================================
来源：http://fwf.hongshengwenyu.top

F. 文件与目录
来源：http://jmd.yfazqb.com

================================================================================
来源：http://oiv.aibaodan.cn

[F01] 读取整个文件
来源：http://adf.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hoe.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://kas.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mlu.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hcy.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://gnm.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pln.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://ytt.ydzc1.top


<!-- 参考信息 -->