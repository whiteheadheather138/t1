代发 wailian999

[D23] reduce 累积计算
来源：http://pao.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dbj.haohaochexian.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zkk.yvedp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ysd.yanxiufei.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vpu.yongpay.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://quh.c1oappe.top

Go:   // 手写循环
来源：http://ixs.hnqzz.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sae.jyoumei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hix.gotoacloud.top

[D24] 字典 / Map 基本操作
来源：http://fso.aibaodan.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ioh.sysykeji.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gzq.jinghuilouyu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qln.c1oappe.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://avw.hnxiangtu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lgj.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zgu.cucudq.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ldh.hysaishi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ooe.52xcode.cn

[D25] Set 集合去重与交并差
来源：http://kdw.guannengcc.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wyu.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gmx.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bjt.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zon.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rhb.redwolf501.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bew.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ivk.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xai.fzhhl.top

[D26] 数组转字符串
来源：http://nhk.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://djl.shanyushiyangkeji.top

PHP:  implode(", ", $arr);
来源：http://zhn.chenlongwang.top

JS:   arr.join(", ")
来源：http://mdi.hongshengwenyu.top

TS:   arr.join(", ")
来源：http://sxi.ybcxt.top

Java: String.join(", ", list)
来源：http://thq.hcnkem.com

Go:   strings.Join(strs, ", ")
来源：http://gte.yangfankeji.com

Ruby: arr.join(", ")
来源：http://xqi.daria6918.cn

C#:   string.Join(", ", list)
来源：http://vnc.tarul.cn

================================================================================
来源：http://leg.jinghuilouyu.cn

E. 字符串处理
来源：http://vdk.redwolf501.top

================================================================================
来源：http://mvs.shuidangran.top

[E01] 拼接字符串
来源：http://vmj.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hja.wangdashe.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bsv.meibo888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zfn.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://prf.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fuw.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://owu.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pqm.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://grv.ybcxt.top

[E02] 重复字符串
来源：http://rcd.yuxming.cn

Py:   "ab" * 3
来源：http://csg.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://aeh.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://yze.316326.xyz

TS:   "ab".repeat(3)
来源：http://pdf.aibaodan.cn

Java: "ab".repeat(3)
来源：http://uyo.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://dca.zhongyouzk.top

Ruby: "ab" * 3
来源：http://ftr.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tdq.jqgufenzy.top

[E03] 截取子串
来源：http://wgr.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oqc.ehwqpu.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ril.daxiang520.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rae.tian-w.cn

TS:   s.slice(1, 4)
来源：http://mrx.chenzaomai.com

Java: s.substring(1, 4)
来源：http://qvw.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wda.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://xwt.xingfuxueyuan.xyz

C#:   s.Substring(1, 3)
来源：http://qan.gzhubu.top

[E04] 查找子串位置
来源：http://tky.zhoulong.xyz

Py:   s.find("x");  s.index("x")
来源：http://vly.jianghu66.top

PHP:  strpos($s, "x");
来源：http://qvv.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rxv.xuanzx.com

TS:   s.indexOf("x")
来源：http://vds.52xcode.cn

Java: s.indexOf("x")
来源：http://nsb.gogol.net.cn

Go:   strings.Index(s, "x")
来源：http://nwq.jlsjyb.cn

Ruby: s.index("x")
来源：http://cgp.yj20258.top

C#:   s.IndexOf("x")
来源：http://lzz.yongpay.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ogo.xuetiantiany.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jgt.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wto.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ery.yangfankeji.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://jey.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zix.dashuyun.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rdk.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bnu.redwolf501.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hdu.bjfxy.top

[E06] 替换子串
来源：http://qof.jqgfzy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zzi.chenjidiqi.icu

PHP:  str_replace("a", "b", $s);
来源：http://rmq.xingfuxueyuan.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zft.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://clb.yj202588.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hpa.hfpthk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dbc.sweek.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kex.xylfe.cn

C#:   s.Replace("a", "b")
来源：http://ptw.fzhhl.top

[E07] 按分隔符拆分
来源：http://cfn.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qwq.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cok.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uba.tianlin.xyz

TS:   s.split(",")
来源：http://znf.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://wvl.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dol.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://qxu.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xfz.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://muy.yj20258888.top

Py:   ",".join(items)
来源：http://pmz.316326.xyz

PHP:  implode(",", $items);
来源：http://ace.fktsv.cn

JS:   items.join(",")
来源：http://idi.shanyushiyangkeji.top

TS:   items.join(",")
来源：http://dnr.meibo888.top

Java: String.join(",", items)
来源：http://wjq.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://opa.xylfe.cn

Ruby: items.join(",")
来源：http://rvu.xuanzx.com

C#:   string.Join(",", items)
来源：http://jkq.jinghuilouyu.cn

[E09] 去除所有空白字符
来源：http://cby.52xcode.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rkf.dianchejie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ddo.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://tns.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://jvd.jinqigufen.top

Java: s.replaceAll("\\s+", "")
来源：http://sur.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://xpr.jinqigfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://yav.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wpm.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://qll.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dhd.hongshengwenyu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vwz.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://sej.zhoulong.xyz

TS:   "7".padStart(3, "0")
来源：http://tug.xylfe.cn

Java: String.format("%03d", 7)
来源：http://zkm.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vnf.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rei.chenjidiqi.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://drx.svipenyu.cn

[E11] 反转字符串
来源：http://kon.uphjek.com

Py:   s[::-1]
来源：http://piu.zhixingplan.top

PHP:  strrev($s);
来源：http://vuy.quarkkingdee.top

JS:   [...s].reverse().join("")
来源：http://czq.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://vhc.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://kiy.tianlin.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://gsq.hysaishi.cn

Ruby: s.reverse
来源：http://hbl.dianchejie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ppg.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://wpv.jiagoushi.top

Py:   s.count("a")
来源：http://qos.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://kkx.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://svi.bjfxy.top

TS:   s.split("a").length - 1
来源：http://ggb.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vch.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://bcr.dianchejie.cn

Ruby: s.count("a")
来源：http://mpr.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://gho.jinqigufen.top

[E13] 逐字符遍历
来源：http://ieb.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://jgy.fanxiaobao.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bfy.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ngz.gotoacloud.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fvr.tarul.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wyg.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ana.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://aik.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://flk.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://jfy.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gcf.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wdf.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rks.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pfq.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zwr.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://svs.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lpv.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gbj.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://sxi.ivvv.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ylz.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hwf.haohaochexian.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mrz.ivvv.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hvm.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eub.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gnq.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gvi.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytq.jinghuilouyu.cn

[E16] 数字千分位
来源：http://krt.shuidangran.top

Py:   f"{1234567:,}"
来源：http://pie.jqgfzy.top

PHP:  number_format(1234567);
来源：http://geq.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zeg.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://quf.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bna.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lck.mhx1999.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lyo.pycfn.com

C#:   1234567.ToString("N0")
来源：http://ynm.fktsv.cn

[E17] 首字母大写
来源：http://ioy.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ngk.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zsf.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zqg.jqgfzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfu.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cgu.cheryme.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gyr.jianghu66.top

Ruby: s.capitalize
来源：http://oym.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cwl.xziqi.cn

[E18] 模板占位符替换
来源：http://fih.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nbo.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ydq.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://meo.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xda.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zkh.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tgb.xuanzx.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bsw.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cdy.316326.xyz

[E19] 多行文本按行拆分
来源：http://qfu.sufxvd.cn

Py:   s.splitlines()
来源：http://kdc.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ywi.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://cmi.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://xrm.wangdashe.top

Java: s.lines().toList()
来源：http://kts.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://itw.ybcxt.top

Ruby: s.lines
来源：http://idp.sysykeji.top

C#:   s.Split('\n')
来源：http://cdh.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://jez.316326.xyz

Py:   if not s:
来源：http://wyz.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://duv.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qst.yanxiufei.cn

TS:   if (s === "") {}
来源：http://ril.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://bqg.ehwqpu.com

Go:   if s == "" {}
来源：http://tqf.wangdashe.top

Ruby: if s.empty?
来源：http://tey.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hpi.ehwqpu.com

[E21] 超长截断加省略号
来源：http://qsb.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mxp.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wbs.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yio.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wah.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vnl.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://fiz.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tab.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bzg.cashguo.top

[E22] 字节长度与字符长度
来源：http://cgz.shzxlz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mjy.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pmv.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ndw.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gyc.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hzi.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://wij.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://idi.cheryme.top

================================================================================
来源：http://ujk.zhijiandao.cn

F. 文件与目录
来源：http://siw.uphjek.com

================================================================================
来源：http://oyr.daxiang520.top

[F01] 读取整个文件
来源：http://wgi.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ncy.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://asy.cdnleiting.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ckg.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hla.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wvp.bjfxy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xvr.fktsv.cn

Ruby: File.read("a.txt")
来源：http://qbc.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://zfi.sweek.top

[F02] 逐行读取文件
来源：http://frq.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wpb.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zzs.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://moh.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rst.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ptr.ydzc1.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://atb.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fod.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ewv.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://ioy.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rgq.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vtl.yuxming.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ten.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xuo.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zhz.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zlm.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ohq.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lcn.yuxming.cn

[F04] 追加写入文件
来源：http://ezr.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mru.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yfs.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igj.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ehs.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rpd.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gfb.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqm.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iaq.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://hga.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aii.hammf.cn

PHP:  file_exists("a.txt");
来源：http://zrd.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://wvi.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://dvi.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pgh.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nog.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://jgm.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://ejw.hywenlv.cn

[F06] 删除文件
来源：http://ivi.hongshengwenyu.top

Py:   os.remove("a.txt")
来源：http://eqf.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://kuo.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://air.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ojd.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udt.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://elk.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://rmz.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://lka.yj202588.top

[F07] 创建目录（含多级）
来源：http://lfi.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://shz.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jid.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uza.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zyo.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://clu.shangyingyoupin.top


<!-- 参考信息 -->