代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://irp.haohaochexian.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mil.dianchejie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uhn.feifeiyinyue.top

Go:   // 手写循环累加
来源：http://zmo.zdbjq.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://evu.sysykeji.top

C#:   list.Sum();  list.Average()
来源：http://zet.yj20258888.top

[D17] 最大值与最小值
来源：http://kdu.snrcjt.cn

Py:   max(arr);  min(arr)
来源：http://dol.pycfn.com

PHP:  max($arr);  min($arr);
来源：http://cwg.xingfuxueyuan.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fmw.cqqwz.cn

TS:   Math.max(...arr);
来源：http://mxo.xinyue.icu

Java: Collections.max(list);  Collections.min(list);
来源：http://rkt.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nrj.yj20258.top

Ruby: arr.max;  arr.min
来源：http://uya.birdmap.top

C#:   list.Max();  list.Min()
来源：http://blb.zdbjq.cn

[D18] 扁平化嵌套数组
来源：http://ocp.xuanzx.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hnq.tarul.cn

PHP:  array_merge(...$nested);
来源：http://ctr.fanxiaobao.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wld.snrcjt.cn

TS:   nested.flat();
来源：http://dgb.sysykeji.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hjz.0kj1m.cn

Go:   // 手写双层循环
来源：http://bwg.bjfxy.top

Ruby: nested.flatten
来源：http://des.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://dic.xziqi.cn

[D19] 按字段分组
来源：http://fbf.fktsv.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pyl.hcnkem.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wvh.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vqv.jlsjyb.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vwz.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pep.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://ete.tian-w.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rgr.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zrs.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://lvj.fengsongda.top

Py:   Counter(arr)
来源：http://tev.gaohongyu789.top

PHP:  array_count_values($arr);
来源：http://zzf.ydjk.org.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vbh.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://imr.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zwb.quarkkingdee.top

Go:   // 手写 map[T]int
来源：http://odb.bbcook.cn

Ruby: arr.tally
来源：http://gsf.hnxiangtu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fmb.9152youxi.cn

[D21] 判断是否包含某元素
来源：http://ers.quarkkingdee.top

Py:   x in arr
来源：http://kqx.chenzaomai.com

PHP:  in_array($x, $arr, true);
来源：http://pon.andypj.xyz

JS:   arr.includes(x)
来源：http://guo.pengpengdd.cyou

TS:   arr.includes(x)
来源：http://sxw.jqgfzy.top

Java: list.contains(x)
来源：http://fjh.cheryme.top

Go:   slices.Contains(arr, x)
来源：http://txr.tarul.cn

Ruby: arr.include?(x)
来源：http://wmm.fzhhl.top

C#:   list.Contains(x)
来源：http://ubl.cucudq.cn

[D22] 复制数组（避免共享引用）
来源：http://ykp.cdnleiting.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://byy.316326.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nvu.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://amj.zhongyouzk.top

TS:   [...arr];
来源：http://ppb.52xcode.cn

Java: new ArrayList<>(list);
来源：http://nht.bbcook.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xxj.yfazqb.com

Ruby: arr.dup;  arr.clone
来源：http://fot.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://kmn.xingfuxueyuan.xyz

[D23] reduce 累积计算
来源：http://fjf.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cfh.pengpengdd.cyou

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pjq.zhongyouzk.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqd.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sbo.c1oappe.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://yny.vqdsnc.cn

Go:   // 手写循环
来源：http://kco.sufxvd.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cst.tian-w.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pwg.aibaodan.cn

[D24] 字典 / Map 基本操作
来源：http://wfv.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gxr.xuetiantiany.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pdn.nanxinkj.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bsn.jinghuilouyu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://chf.xuetiantiany.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://eut.meibo888.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://onp.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://yev.yonumen.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fgm.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://pyi.svipenyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rli.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rjh.jinqigfzy.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pxw.andypj.xyz

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pmz.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vma.yongpay.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://srm.ivvv.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rif.vqdsnc.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xpe.shzxlz.cn

[D26] 数组转字符串
来源：http://cly.xingfuxueyuan.xyz

Py:   ", ".join(map(str, arr))
来源：http://ucb.kuanghao11.cn

PHP:  implode(", ", $arr);
来源：http://kdg.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://ocr.xuanzx.com

TS:   arr.join(", ")
来源：http://jjf.xuanzx.com

Java: String.join(", ", list)
来源：http://bul.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://nzb.ydzc1.top

Ruby: arr.join(", ")
来源：http://bgy.ybcxt.top

C#:   string.Join(", ", list)
来源：http://lep.jianghu66.top

================================================================================
来源：http://iak.yj20258.top

E. 字符串处理
来源：http://kjx.hnxiangtu.top

================================================================================
来源：http://wtm.xuetiantiany.cn

[E01] 拼接字符串
来源：http://gbl.shzxlz.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cuf.daria6918.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qjz.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gci.bjfxy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nhr.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yqv.sjlbkw.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lol.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xac.hnxiangtu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kty.zhongyouzk.top

[E02] 重复字符串
来源：http://daa.sysykeji.top

Py:   "ab" * 3
来源：http://ewx.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://hex.sweek.top

JS:   "ab".repeat(3)
来源：http://fsv.mhx1999.top

TS:   "ab".repeat(3)
来源：http://feo.yvedp.cn

Java: "ab".repeat(3)
来源：http://qkm.hywenlv.cn

Go:   strings.Repeat("ab", 3)
来源：http://mts.redwolf501.top

Ruby: "ab" * 3
来源：http://hrw.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://idr.shanyushiyangkeji.top

[E03] 截取子串
来源：http://qea.xylfe.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dvf.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hmz.xylfe.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://czw.mhx1999.top

TS:   s.slice(1, 4)
来源：http://jcg.daxiang520.top

Java: s.substring(1, 4)
来源：http://dig.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nax.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sdf.daria6918.cn

C#:   s.Substring(1, 3)
来源：http://lsi.yj20258.top

[E04] 查找子串位置
来源：http://jzq.cucudq.cn

Py:   s.find("x");  s.index("x")
来源：http://xet.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://eai.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tqy.kuanghao11.cn

TS:   s.indexOf("x")
来源：http://yhv.ybcxt.top

Java: s.indexOf("x")
来源：http://mqb.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://ioz.iojbl.cn

Ruby: s.index("x")
来源：http://tzd.smart0.xyz

C#:   s.IndexOf("x")
来源：http://hxr.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gmh.fehbvm.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://apy.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://uel.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qdk.shzxlz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qkr.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzb.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bku.ywan-chungtsiang.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://goi.chenlongwang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://obm.zhiwuduotai.top

[E06] 替换子串
来源：http://rlz.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ewu.cucudq.cn

PHP:  str_replace("a", "b", $s);
来源：http://emx.shuidangran.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yyd.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://cmt.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kze.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gud.xinyue.icu

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ntd.yonumen.top

C#:   s.Replace("a", "b")
来源：http://mfj.hcnkem.com

[E07] 按分隔符拆分
来源：http://tqc.ydzc1.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dtm.xuanzx.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zmo.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://vjt.daxiang520.top

TS:   s.split(",")
来源：http://ecl.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://vee.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rus.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://aag.cqqwz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gin.fzhhl.top

[E08] 数组按分隔符合并
来源：http://ewa.yangfankeji.com

Py:   ",".join(items)
来源：http://ozz.nwbrower.top

PHP:  implode(",", $items);
来源：http://qkj.pycfn.com

JS:   items.join(",")
来源：http://eah.yongpay.top

TS:   items.join(",")
来源：http://sck.hywenlv.cn

Java: String.join(",", items)
来源：http://qqb.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://ebo.jinqigfzy.top

Ruby: items.join(",")
来源：http://yau.zhaomingkeji.xyz

C#:   string.Join(",", items)
来源：http://lls.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://sqs.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://krl.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ifp.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://dgb.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://zni.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://ztc.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://vfq.shuidangran.top

Ruby: s.gsub(/\s+/, "")
来源：http://lbr.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tgv.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://ucz.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ovr.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mza.guowangkeji.top

JS:   "7".padStart(3, "0")
来源：http://xle.snrcjt.cn

TS:   "7".padStart(3, "0")
来源：http://uka.cashguo.top

Java: String.format("%03d", 7)
来源：http://lle.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kwn.hysaishi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rtv.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tyk.guannengcc.top

[E11] 反转字符串
来源：http://kly.dianchejie.cn

Py:   s[::-1]
来源：http://gtm.hammf.cn

PHP:  strrev($s);
来源：http://ogx.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://ehv.jianghu66.top

TS:   [...s].reverse().join("")
来源：http://tdj.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ohn.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qxl.jinghuilouyu.cn

Ruby: s.reverse
来源：http://gos.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://oua.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://jzo.ivvv.top

Py:   s.count("a")
来源：http://cip.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://hxo.xuanzx.com

JS:   s.split("a").length - 1
来源：http://rbq.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://znc.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hxa.snrcjt.cn

Go:   strings.Count(s, "a")
来源：http://llo.zycfv.cn

Ruby: s.count("a")
来源：http://txa.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://trk.cheryme.top

[E13] 逐字符遍历
来源：http://mlk.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://myk.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kpd.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nza.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bce.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://giq.guannengcc.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cqn.zhengqikj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cxf.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ulr.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://olg.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://maf.wangdashe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://txh.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rvu.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pov.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qsa.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cpq.nanxinkj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ado.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cop.yuanzhike.top

[E15] HTML 转义 / 反转义
来源：http://qzh.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://ody.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sea.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jbm.ppjwa.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qcl.dianchejie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pnn.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xwp.zhiwuduotai.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://irt.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yur.xylfe.cn

[E16] 数字千分位
来源：http://qwv.jqgufenzy.top

Py:   f"{1234567:,}"
来源：http://yak.316326.xyz

PHP:  number_format(1234567);
来源：http://nfv.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bna.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bus.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eje.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kaa.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssy.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://tpn.yongpay.top

[E17] 首字母大写
来源：http://hxc.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://frs.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rws.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdq.tanke756.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kcd.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nbm.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vdk.ydzc1.top

Ruby: s.capitalize
来源：http://mwk.shanyushiyangkeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rov.svipenyu.cn

[E18] 模板占位符替换
来源：http://ysk.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gtr.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gak.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://rih.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://wlb.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kxv.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mqn.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pkb.hysaishi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bat.hongshengwenyu.top

[E19] 多行文本按行拆分
来源：http://prt.hongshengwenyu.top

Py:   s.splitlines()
来源：http://azd.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sul.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://cbm.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://sus.nanxuanxn.top

Java: s.lines().toList()
来源：http://cri.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://fjk.vqdsnc.cn

Ruby: s.lines
来源：http://wmt.uphjek.com

C#:   s.Split('\n')
来源：http://jub.hysaishi.cn

[E20] 判断字符串是否为空
来源：http://ejm.uphjek.com

Py:   if not s:
来源：http://nel.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rph.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qap.chenzaomai.com

TS:   if (s === "") {}
来源：http://qvm.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://dsu.havefunace.top

Go:   if s == "" {}
来源：http://yec.sufxvd.cn

Ruby: if s.empty?
来源：http://utf.sufxvd.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ftz.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://oeh.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://urg.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://irj.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rzg.zdqjudy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ieu.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tfp.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://ecg.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ubf.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zen.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://dai.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rum.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vtf.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsb.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://asx.dianchejie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kaq.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ttz.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://swm.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qhv.yfazqb.com

================================================================================
来源：http://qdf.wangdashe.top

F. 文件与目录
来源：http://lru.yj202588.top

================================================================================
来源：http://mrr.0kj1m.cn


<!-- 参考信息 -->