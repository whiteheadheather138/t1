代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gkw.zhongyouzk.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://esl.smart0.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jvl.yueranfly.top

Go:   // 手写循环累加
来源：http://bkk.yj20258.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://clz.gotoacloud.top

C#:   list.Sum();  list.Average()
来源：http://utq.yonumen.top

[D17] 最大值与最小值
来源：http://gfs.bjfxy.top

Py:   max(arr);  min(arr)
来源：http://laf.ivvv.top

PHP:  max($arr);  min($arr);
来源：http://xfl.guowangkeji.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bju.0kj1m.cn

TS:   Math.max(...arr);
来源：http://hjn.jinyuanbaomall.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wqs.haohaochexian.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://yyk.tian-w.cn

Ruby: arr.max;  arr.min
来源：http://apl.bbcook.cn

C#:   list.Max();  list.Min()
来源：http://gqi.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://gyl.hysaishi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ysa.zhongyouzk.top

PHP:  array_merge(...$nested);
来源：http://lci.sxryk.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pwk.vqdsnc.cn

TS:   nested.flat();
来源：http://iqi.52xcode.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lob.zhixingplan.top

Go:   // 手写双层循环
来源：http://uti.jyoumei.cn

Ruby: nested.flatten
来源：http://jrk.jinyuanbaomall.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mtb.cashguo.top

[D19] 按字段分组
来源：http://czp.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ukt.jyoumei.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hhz.nwbrower.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aar.wangdashe.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://gvf.shangyingyoupin.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://joe.guowangkeji.top

Go:   // 手写 map[string][]T
来源：http://cgv.jianghu66.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://kkq.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lyc.52xcode.cn

[D20] 统计每个元素出现次数
来源：http://jez.tarul.cn

Py:   Counter(arr)
来源：http://zgh.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://dkd.smart0.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kcd.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dfd.ivvv.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xsc.dianchejie.cn

Go:   // 手写 map[T]int
来源：http://exo.jianghu66.top

Ruby: arr.tally
来源：http://jhh.vqdsnc.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cmz.fktsv.cn

[D21] 判断是否包含某元素
来源：http://rhk.aizwys.cn

Py:   x in arr
来源：http://etd.cdnleiting.top

PHP:  in_array($x, $arr, true);
来源：http://ztq.dianchejie.cn

JS:   arr.includes(x)
来源：http://ips.0kj1m.cn

TS:   arr.includes(x)
来源：http://vcl.zhongyouzk.top

Java: list.contains(x)
来源：http://mnk.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://kch.jianghu66.top

Ruby: arr.include?(x)
来源：http://qhu.xingfuxueyuan.xyz

C#:   list.Contains(x)
来源：http://uas.vehdjk.com

[D22] 复制数组（避免共享引用）
来源：http://onq.hammf.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://raj.yonumen.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ttr.shangyingyoupin.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ojb.ppjwa.cn

TS:   [...arr];
来源：http://kgo.quarkkingdee.top

Java: new ArrayList<>(list);
来源：http://uvf.zhongyouzk.top

Go:   copied := append([]int(nil), arr...)
来源：http://tfv.yangfankeji.com

Ruby: arr.dup;  arr.clone
来源：http://nnb.jinqigufen.top

C#:   new List<int>(list);
来源：http://tfm.ppjwa.cn

[D23] reduce 累积计算
来源：http://rij.haohaochexian.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rnq.guannengcc.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xwi.ivvv.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dzz.zdqjudy.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zcl.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fjw.iojbl.cn

Go:   // 手写循环
来源：http://mxm.jyoumei.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://anh.jinghuilouyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bik.sufxvd.cn

[D24] 字典 / Map 基本操作
来源：http://gcz.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cqr.gogol.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://umn.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://feq.shuidangran.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://uea.fktsv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://phs.hnqzz.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jii.316326.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cbe.cdnleiting.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oih.hesvh.cn

[D25] Set 集合去重与交并差
来源：http://vny.guowangkeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jgp.yuxming.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wcq.ppjwa.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://row.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://phk.tianlin.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gfe.cdnleiting.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://khr.jinqigufen.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zty.hysaishi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wre.ybcxt.top

[D26] 数组转字符串
来源：http://cuw.9152youxi.cn

Py:   ", ".join(map(str, arr))
来源：http://src.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://bju.svipenyu.cn

JS:   arr.join(", ")
来源：http://ufz.yuanzhike.top

TS:   arr.join(", ")
来源：http://zpr.ppjwa.cn

Java: String.join(", ", list)
来源：http://zxk.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://jur.tian-w.cn

Ruby: arr.join(", ")
来源：http://ims.jqgfzy.top

C#:   string.Join(", ", list)
来源：http://jbe.yanxiufei.cn

================================================================================
来源：http://val.shanyushiyangkeji.top

E. 字符串处理
来源：http://mqy.yuxming.cn

================================================================================
来源：http://spu.ywan-chungtsiang.top

[E01] 拼接字符串
来源：http://bhh.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zba.smart0.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cmg.aizwys.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hms.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zoi.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://npn.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qps.tianlin.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vnq.shanyushiyangtech.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jng.zdqjudy.top

[E02] 重复字符串
来源：http://bff.yj20258.top

Py:   "ab" * 3
来源：http://cor.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://htd.fengsongda.top

JS:   "ab".repeat(3)
来源：http://epu.nanxuanxn.top

TS:   "ab".repeat(3)
来源：http://djx.gaohongyu789.top

Java: "ab".repeat(3)
来源：http://fni.shzxlz.cn

Go:   strings.Repeat("ab", 3)
来源：http://aew.sysykeji.top

Ruby: "ab" * 3
来源：http://igo.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zco.nanxuanxn.top

[E03] 截取子串
来源：http://dqo.hongshengwenyu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pjn.hnxiangtu.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vlw.c1oappe.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kub.yueranfly.top

TS:   s.slice(1, 4)
来源：http://ske.guannengcc.top

Java: s.substring(1, 4)
来源：http://tzh.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://utq.hongshengwenyu.top

Ruby: s[1, 3];  s[1..3]
来源：http://wbl.ydzc1.top

C#:   s.Substring(1, 3)
来源：http://rur.meibo888.top

[E04] 查找子串位置
来源：http://wsn.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://vsv.zhixingplan.top

PHP:  strpos($s, "x");
来源：http://efv.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yof.sufxvd.cn

TS:   s.indexOf("x")
来源：http://tky.yangfankeji.com

Java: s.indexOf("x")
来源：http://qjh.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://ixt.yanxiufei.cn

Ruby: s.index("x")
来源：http://pty.sysykeji.top

C#:   s.IndexOf("x")
来源：http://jxk.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zsx.sweek.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dix.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ijx.zhongyouzk.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cbi.daria6918.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dtk.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cik.ctjpmb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dvl.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cxj.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wzk.jinghuilouyu.cn

[E06] 替换子串
来源：http://dxk.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pks.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://hfk.xinyue.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ler.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://ymk.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xof.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kvw.xylfe.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://omd.daria6918.cn

C#:   s.Replace("a", "b")
来源：http://epf.hammf.cn

[E07] 按分隔符拆分
来源：http://srh.zhijiandao.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qbo.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fmv.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vzw.ivvv.top

TS:   s.split(",")
来源：http://chu.sweek.top

Java: s.split(",");  s.split("\\s+")
来源：http://wcv.sjlbkw.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hvz.chenjidiqi.icu

Ruby: s.split(",");  s.split
来源：http://ztk.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vaz.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://kqo.sufxvd.cn

Py:   ",".join(items)
来源：http://zsi.hysaishi.cn

PHP:  implode(",", $items);
来源：http://gtj.nwbrower.top

JS:   items.join(",")
来源：http://dif.ppjwa.cn

TS:   items.join(",")
来源：http://npx.uphjek.com

Java: String.join(",", items)
来源：http://wzu.tanke756.top

Go:   strings.Join(items, ",")
来源：http://okf.andypj.xyz

Ruby: items.join(",")
来源：http://wbx.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://qvw.gzhubu.top

[E09] 去除所有空白字符
来源：http://asy.yj20258.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jrj.snrcjt.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cul.cashguo.top

JS:   s.replace(/\s+/g, "")
来源：http://csz.jqgufenzy.top

TS:   s.replace(/\s+/g, "")
来源：http://qah.smart0.xyz

Java: s.replaceAll("\\s+", "")
来源：http://tpw.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wbr.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://foe.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dmo.hammf.cn

[E10] 左侧补零 / 定长填充
来源：http://jlr.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cbj.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gfs.shangyingyoupin.top

JS:   "7".padStart(3, "0")
来源：http://xky.shangyingyoupin.top

TS:   "7".padStart(3, "0")
来源：http://vpw.pycfn.com

Java: String.format("%03d", 7)
来源：http://ieb.jinghuilouyu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ggu.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://thc.epnwcf.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jwo.vehdjk.com

[E11] 反转字符串
来源：http://hlx.iojbl.cn

Py:   s[::-1]
来源：http://gmh.uphjek.com

PHP:  strrev($s);
来源：http://myg.daxiang520.top

JS:   [...s].reverse().join("")
来源：http://ofq.ppjwa.cn

TS:   [...s].reverse().join("")
来源：http://mia.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gfr.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lny.zhiwuduotai.top

Ruby: s.reverse
来源：http://ogn.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wmt.cqqwz.cn

[E12] 统计某字符出现次数
来源：http://rbr.xinyue.icu

Py:   s.count("a")
来源：http://aet.meibo888.top

PHP:  substr_count($s, "a");
来源：http://qqx.tian-w.cn

JS:   s.split("a").length - 1
来源：http://gkp.epnwcf.com

TS:   s.split("a").length - 1
来源：http://pnz.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://scd.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://lkf.aizwys.cn

Ruby: s.count("a")
来源：http://bfq.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://dwm.tian-w.cn

[E13] 逐字符遍历
来源：http://fds.tarul.cn

Py:   for ch in s: print(ch)
来源：http://xoa.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ito.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cxm.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://trc.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://igk.zhaomingkeji.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://efu.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lnc.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vys.guannengcc.top

[E14] URL 编码与 Base64
来源：http://mup.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://shu.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gqj.sjlbkw.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ejq.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ksl.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rym.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nbc.9152youxi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zya.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qyn.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://wmm.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://kcv.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ecb.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gdq.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mpk.xuetiantiany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rtl.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hxi.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pua.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kan.cqqwz.cn

[E16] 数字千分位
来源：http://fhm.yj20258888.top

Py:   f"{1234567:,}"
来源：http://aak.epnwcf.com

PHP:  number_format(1234567);
来源：http://mvm.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://tcn.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cyd.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xae.xylfe.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fgd.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://euf.sxryk.cn

C#:   1234567.ToString("N0")
来源：http://tbe.316326.xyz

[E17] 首字母大写
来源：http://cug.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lgo.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rqw.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kdo.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dkr.redwolf501.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eqa.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gyd.mhx1999.top

Ruby: s.capitalize
来源：http://wdr.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nnq.redwolf501.top

[E18] 模板占位符替换
来源：http://tel.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lwf.sufxvd.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hgz.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mwp.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rpn.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zej.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bbc.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pmn.yonumen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vuy.yvedp.cn

[E19] 多行文本按行拆分
来源：http://ctf.jinqigfzy.top

Py:   s.splitlines()
来源：http://dnr.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vax.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://tha.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://ats.shangyingyoupin.top

Java: s.lines().toList()
来源：http://cta.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://ncj.ctjpmb.com

Ruby: s.lines
来源：http://idt.xziqi.cn

C#:   s.Split('\n')
来源：http://aba.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://ipi.zhoulong.xyz

Py:   if not s:
来源：http://ijv.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgg.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pjm.nanxuanxn.top

TS:   if (s === "") {}
来源：http://rjr.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://okc.yvedp.cn

Go:   if s == "" {}
来源：http://uuk.jqgfzy.top

Ruby: if s.empty?
来源：http://zdv.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jgc.fehbvm.com

[E21] 超长截断加省略号
来源：http://vda.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yac.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eny.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ght.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://feo.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jfg.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://qgb.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://swu.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rzi.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://akc.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sjx.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmv.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://flq.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cxk.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cez.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksv.sjlbkw.cn

Ruby: s.bytesize;  s.length
来源：http://gng.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wcc.hnxiangtu.top

================================================================================
来源：http://mui.cdnleiting.top

F. 文件与目录
来源：http://zdo.feifeiyinyue.top

================================================================================
来源：http://qet.pycfn.com


<!-- 参考信息 -->