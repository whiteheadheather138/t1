代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://aad.ppjwa.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://alk.tarul.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://kae.dashuyun.cn

Go:   // 手写循环累加
来源：http://fdr.ctjpmb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rir.shangyingyoupin.top

C#:   list.Sum();  list.Average()
来源：http://las.haohaochexian.top

[D17] 最大值与最小值
来源：http://uyy.guowangkeji.top

Py:   max(arr);  min(arr)
来源：http://lch.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://dco.316326.xyz

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tmk.tian-w.cn

TS:   Math.max(...arr);
来源：http://qjr.aizwys.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zqh.jianghu66.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://clv.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://gni.fktsv.cn

C#:   list.Max();  list.Min()
来源：http://cto.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://jzp.yj20258888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wmt.hysaishi.cn

PHP:  array_merge(...$nested);
来源：http://ytl.xylfe.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rjc.hammf.cn

TS:   nested.flat();
来源：http://len.cucudq.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uoz.cheryme.top

Go:   // 手写双层循环
来源：http://bqn.0kj1m.cn

Ruby: nested.flatten
来源：http://har.snrcjt.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gxh.zhongyouzk.top

[D19] 按字段分组
来源：http://mcn.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cvk.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://lvz.nanxuanxn.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zhx.jqgufenzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qby.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://owe.jiagoushi.top

Go:   // 手写 map[string][]T
来源：http://fai.mhx1999.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xjd.zdqjudy.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mng.aizwys.cn

[D20] 统计每个元素出现次数
来源：http://mzs.daxiang520.top

Py:   Counter(arr)
来源：http://baa.yuanzhike.top

PHP:  array_count_values($arr);
来源：http://ctr.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nor.pengpengdd.cyou

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ssx.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zky.tanke756.top

Go:   // 手写 map[T]int
来源：http://ggn.ppjwa.cn

Ruby: arr.tally
来源：http://kzb.pengpengdd.cyou

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jqc.sxryk.cn

[D21] 判断是否包含某元素
来源：http://tvo.9152youxi.cn

Py:   x in arr
来源：http://wjo.fanxiaobao.xyz

PHP:  in_array($x, $arr, true);
来源：http://cyo.aibaodan.cn

JS:   arr.includes(x)
来源：http://olb.chenzaomai.com

TS:   arr.includes(x)
来源：http://oxx.jiagoushi.top

Java: list.contains(x)
来源：http://eqo.316326.xyz

Go:   slices.Contains(arr, x)
来源：http://yij.shzxlz.cn

Ruby: arr.include?(x)
来源：http://hqc.hfpthk.cn

C#:   list.Contains(x)
来源：http://sob.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://oej.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sqs.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://thx.mhx1999.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rad.zdqjudy.top

TS:   [...arr];
来源：http://shf.snrcjt.cn

Java: new ArrayList<>(list);
来源：http://wlm.9152youxi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://hqo.feifeiyinyue.top

Ruby: arr.dup;  arr.clone
来源：http://aae.xinyue.icu

C#:   new List<int>(list);
来源：http://lty.c1oappe.top

[D23] reduce 累积计算
来源：http://bhf.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sho.c1oappe.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://puc.dianchejie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tpy.yongpay.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fvj.hesvh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cnq.cucudq.cn

Go:   // 手写循环
来源：http://sdz.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uwf.cashguo.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://syt.ehwqpu.com

[D24] 字典 / Map 基本操作
来源：http://vnq.52xcode.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wch.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://izt.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dzp.quarkkingdee.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://try.dashuyun.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://unn.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bjh.yangfankeji.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nuy.redwolf501.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gqm.ydzc1.top

[D25] Set 集合去重与交并差
来源：http://xkp.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://usg.bbcook.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mqv.sufxvd.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ykj.redwolf501.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uib.0kj1m.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qvp.c1oappe.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iiv.jqgfzy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://edv.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://plu.sjlbkw.cn

[D26] 数组转字符串
来源：http://dqi.gzhubu.top

Py:   ", ".join(map(str, arr))
来源：http://sam.meibo888.top

PHP:  implode(", ", $arr);
来源：http://mve.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://vrk.zycfv.cn

TS:   arr.join(", ")
来源：http://mpy.yonumen.top

Java: String.join(", ", list)
来源：http://bez.havefunace.top

Go:   strings.Join(strs, ", ")
来源：http://syp.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://wcb.yongpay.top

C#:   string.Join(", ", list)
来源：http://tut.zhoulong.xyz

================================================================================
来源：http://qjd.jinghuilouyu.cn

E. 字符串处理
来源：http://pou.iojbl.cn

================================================================================
来源：http://cfw.ivvv.top

[E01] 拼接字符串
来源：http://oov.0kj1m.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://tor.ehwqpu.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://kvk.shangyingyoupin.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jwv.shangyingyoupin.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://awb.hammf.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cdz.jqgufenzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://scv.shanyushiyangtech.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rst.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jpt.vqdsnc.cn

[E02] 重复字符串
来源：http://ilj.yj20258.top

Py:   "ab" * 3
来源：http://qbc.shangyingyoupin.top

PHP:  str_repeat("ab", 3);
来源：http://eur.0kj1m.cn

JS:   "ab".repeat(3)
来源：http://zeb.epnwcf.com

TS:   "ab".repeat(3)
来源：http://pxz.quarkkingdee.top

Java: "ab".repeat(3)
来源：http://cin.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://awp.vqdsnc.cn

Ruby: "ab" * 3
来源：http://plk.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yoj.mhx1999.top

[E03] 截取子串
来源：http://zrz.iojbl.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://quk.ppjwa.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zct.sysykeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yjm.mhx1999.top

TS:   s.slice(1, 4)
来源：http://ocp.fktsv.cn

Java: s.substring(1, 4)
来源：http://cay.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zde.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pgm.zhongyouzk.top

C#:   s.Substring(1, 3)
来源：http://ydz.hysaishi.cn

[E04] 查找子串位置
来源：http://zae.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://dmf.shzxlz.cn

PHP:  strpos($s, "x");
来源：http://yiu.ppjwa.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blo.hysaishi.cn

TS:   s.indexOf("x")
来源：http://qpb.ybcxt.top

Java: s.indexOf("x")
来源：http://tdh.dashuyun.cn

Go:   strings.Index(s, "x")
来源：http://tzv.cheryme.top

Ruby: s.index("x")
来源：http://yqz.xinyue.icu

C#:   s.IndexOf("x")
来源：http://aaj.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gpi.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hac.uphjek.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fik.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imh.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://weh.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nxk.daxiang520.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qyf.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vro.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dsn.xinyue.icu

[E06] 替换子串
来源：http://rqo.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whg.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://dwl.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eek.yvedp.cn

TS:   s.replaceAll("a", "b")
来源：http://xag.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://num.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fju.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hzb.9152youxi.cn

C#:   s.Replace("a", "b")
来源：http://htf.tanke756.top

[E07] 按分隔符拆分
来源：http://bqu.fengsongda.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://act.jinqigufen.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mra.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sga.cdnleiting.top

TS:   s.split(",")
来源：http://vwr.hnxiangtu.top

Java: s.split(",");  s.split("\\s+")
来源：http://fzc.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wje.cdnleiting.top

Ruby: s.split(",");  s.split
来源：http://mjt.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cqx.vqdsnc.cn

[E08] 数组按分隔符合并
来源：http://qwz.birdmap.top

Py:   ",".join(items)
来源：http://qwa.fktsv.cn

PHP:  implode(",", $items);
来源：http://utn.meibo888.top

JS:   items.join(",")
来源：http://drx.kuanghao11.cn

TS:   items.join(",")
来源：http://laa.ydjk.org.cn

Java: String.join(",", items)
来源：http://zbs.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://iem.gzhubu.top

Ruby: items.join(",")
来源：http://mwu.nanxuanxn.top

C#:   string.Join(",", items)
来源：http://xax.meibo888.top

[E09] 去除所有空白字符
来源：http://xkx.ehwqpu.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zwe.fzhhl.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hxa.gaohongyu789.top

JS:   s.replace(/\s+/g, "")
来源：http://xvs.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://crl.jianghu66.top

Java: s.replaceAll("\\s+", "")
来源：http://vfv.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://imz.ppjwa.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fcu.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bqa.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://lsq.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gkf.wangdashe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xtp.fktsv.cn

JS:   "7".padStart(3, "0")
来源：http://lvd.xinyue.icu

TS:   "7".padStart(3, "0")
来源：http://bsz.xuanzx.com

Java: String.format("%03d", 7)
来源：http://tko.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ihf.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qrd.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fng.andypj.xyz

[E11] 反转字符串
来源：http://wal.ctjpmb.com

Py:   s[::-1]
来源：http://vvb.aibaodan.cn

PHP:  strrev($s);
来源：http://cgx.ydjk.org.cn

JS:   [...s].reverse().join("")
来源：http://iwj.fengsongda.top

TS:   [...s].reverse().join("")
来源：http://zxm.jianghu66.top

Java: new StringBuilder(s).reverse().toString()
来源：http://myq.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://thi.ctjpmb.com

Ruby: s.reverse
来源：http://klw.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fpy.9152youxi.cn

[E12] 统计某字符出现次数
来源：http://pbe.hcnkem.com

Py:   s.count("a")
来源：http://wxu.ywan-chungtsiang.top

PHP:  substr_count($s, "a");
来源：http://lre.xuetiantiany.cn

JS:   s.split("a").length - 1
来源：http://ujg.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://jtw.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://raq.jinyuanbaomall.cn

Go:   strings.Count(s, "a")
来源：http://ppn.jianghu66.top

Ruby: s.count("a")
来源：http://suu.yj20258.top

C#:   s.Count(c => c == 'a')
来源：http://djr.nanxuanxn.top

[E13] 逐字符遍历
来源：http://tfp.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://sec.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gkd.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zdw.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lcg.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qpw.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ker.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://maa.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mua.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://qhe.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vsc.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qgv.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rgh.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rbg.ehwqpu.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://utw.aizwys.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jzy.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eqc.hammf.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://eyb.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://leb.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://air.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ofo.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hba.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://azg.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xtn.ppjwa.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bkh.sxryk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gfu.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fin.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://hpl.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://aus.tanke756.top

PHP:  number_format(1234567);
来源：http://uxx.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vns.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://knr.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://onm.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iwd.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fai.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://bfd.yongpay.top

[E17] 首字母大写
来源：http://qqk.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rxy.52xcode.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dtb.epnwcf.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jhr.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://odn.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gjp.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lvu.dashuyun.cn

Ruby: s.capitalize
来源：http://bwx.vqdsnc.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nbu.birdmap.top

[E18] 模板占位符替换
来源：http://kaq.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yhg.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pbr.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pzp.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ukd.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uzc.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jhp.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nxp.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bex.sweek.top

[E19] 多行文本按行拆分
来源：http://rzn.yuanzhike.top

Py:   s.splitlines()
来源：http://hpj.bjfxy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xpi.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://tvt.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://gtn.meibo888.top

Java: s.lines().toList()
来源：http://ugc.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://cty.birdmap.top

Ruby: s.lines
来源：http://kus.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://deo.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://thi.hfpthk.cn

Py:   if not s:
来源：http://xor.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vmj.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yyb.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://sqq.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://nex.bbcook.cn

Go:   if s == "" {}
来源：http://yak.nanxinkj.top

Ruby: if s.empty?
来源：http://mdt.jlsjyb.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qwq.52xcode.cn

[E21] 超长截断加省略号
来源：http://kkn.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://egm.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwj.pycfn.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://emf.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://usn.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ari.yj202588.top

Go:   // 按 rune 判断长度后截断
来源：http://hxy.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dyk.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://usw.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://dhx.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mtt.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmb.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uek.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qsx.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://txe.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hrn.uphjek.com

Ruby: s.bytesize;  s.length
来源：http://yyc.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hot.mhx1999.top

================================================================================
来源：http://tpe.zhengqikj.top

F. 文件与目录
来源：http://blr.snrcjt.cn

================================================================================
来源：http://kdc.316326.xyz


<!-- 参考信息 -->