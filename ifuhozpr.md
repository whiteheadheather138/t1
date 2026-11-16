代发 wailian999

Java: new ArrayList<>(list);
来源：http://okp.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cfe.yuanzhike.top

Ruby: arr.dup;  arr.clone
来源：http://ygs.ctjpmb.com

C#:   new List<int>(list);
来源：http://mdx.yueranfly.top

[D23] reduce 累积计算
来源：http://emn.vehdjk.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bbi.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pii.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://nek.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://czj.hnxiangtu.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://bad.xuanzx.com

Go:   // 手写循环
来源：http://bnh.jiagoushi.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fcb.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pin.fzhhl.top

[D24] 字典 / Map 基本操作
来源：http://jwg.zhengqikj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wlf.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pza.wangdashe.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://riz.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rdj.hfpthk.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qbn.yfazqb.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dtt.havefunace.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xnu.pengpengdd.cyou

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://akj.cheryme.top

[D25] Set 集合去重与交并差
来源：http://qlp.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xly.cashguo.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uzs.epnwcf.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://thb.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ypo.wangshuangyany.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://acv.zhongyouzk.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qog.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zuh.daxiang520.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xcs.nwbrower.top

[D26] 数组转字符串
来源：http://ggo.wangshuangyany.cn

Py:   ", ".join(map(str, arr))
来源：http://riq.xuetiantiany.cn

PHP:  implode(", ", $arr);
来源：http://hfd.hammf.cn

JS:   arr.join(", ")
来源：http://uus.zycfv.cn

TS:   arr.join(", ")
来源：http://hvm.sufxvd.cn

Java: String.join(", ", list)
来源：http://vnr.gogol.net.cn

Go:   strings.Join(strs, ", ")
来源：http://qmq.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://xrl.smart0.xyz

C#:   string.Join(", ", list)
来源：http://cbc.fengsongda.top

================================================================================
来源：http://rst.wangdashe.top

E. 字符串处理
来源：http://ass.tanke756.top

================================================================================
来源：http://fiz.havefunace.top

[E01] 拼接字符串
来源：http://vxn.pycfn.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jjq.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://avn.sxryk.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lja.jyoumei.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jkx.pengpengdd.cyou

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://upf.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cyy.redwolf501.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xur.ydjk.org.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hyw.snrcjt.cn

[E02] 重复字符串
来源：http://btu.iojbl.cn

Py:   "ab" * 3
来源：http://hym.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://ogj.jlsjyb.cn

JS:   "ab".repeat(3)
来源：http://nir.meibo888.top

TS:   "ab".repeat(3)
来源：http://lmd.bbcook.cn

Java: "ab".repeat(3)
来源：http://rqb.jiagoushi.top

Go:   strings.Repeat("ab", 3)
来源：http://atu.vqdsnc.cn

Ruby: "ab" * 3
来源：http://jpg.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vnl.haohaochexian.top

[E03] 截取子串
来源：http://msw.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cij.pengpengdd.cyou

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://tma.yj20258.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qwz.yonumen.top

TS:   s.slice(1, 4)
来源：http://gcc.hfpthk.cn

Java: s.substring(1, 4)
来源：http://ppa.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tgc.nanxuanxn.top

Ruby: s[1, 3];  s[1..3]
来源：http://bsz.guowangkeji.top

C#:   s.Substring(1, 3)
来源：http://tcr.xylfe.cn

[E04] 查找子串位置
来源：http://lfn.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://smd.birdmap.top

PHP:  strpos($s, "x");
来源：http://gpd.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tum.xuanzx.com

TS:   s.indexOf("x")
来源：http://mba.jlsjyb.cn

Java: s.indexOf("x")
来源：http://llh.pengpengdd.cyou

Go:   strings.Index(s, "x")
来源：http://pca.hywenlv.cn

Ruby: s.index("x")
来源：http://znu.shangyingyoupin.top

C#:   s.IndexOf("x")
来源：http://jmt.quarkkingdee.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hji.dashuyun.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lza.jiagoushi.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ams.xingfuxueyuan.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fzy.cdnleiting.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://iwh.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tin.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ahs.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nmm.bbcook.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xxb.fengsongda.top

[E06] 替换子串
来源：http://mnw.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oed.xuetiantiany.cn

PHP:  str_replace("a", "b", $s);
来源：http://pfh.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mzx.pengpengdd.cyou

TS:   s.replaceAll("a", "b")
来源：http://oma.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://chw.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qgw.kuanghao11.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ihu.uphjek.com

C#:   s.Replace("a", "b")
来源：http://kyg.sxryk.cn

[E07] 按分隔符拆分
来源：http://zvu.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://oxc.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ven.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ivj.tanke756.top

TS:   s.split(",")
来源：http://qux.jyoumei.cn

Java: s.split(",");  s.split("\\s+")
来源：http://gix.ppjwa.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ghs.316326.xyz

Ruby: s.split(",");  s.split
来源：http://cue.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xge.aizwys.cn

[E08] 数组按分隔符合并
来源：http://cvr.hcnkem.com

Py:   ",".join(items)
来源：http://vra.yj20258.top

PHP:  implode(",", $items);
来源：http://ndm.sjlbkw.cn

JS:   items.join(",")
来源：http://rjx.tarul.cn

TS:   items.join(",")
来源：http://azu.yj20258.top

Java: String.join(",", items)
来源：http://qtu.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://lnf.tianlin.xyz

Ruby: items.join(",")
来源：http://spq.iojbl.cn

C#:   string.Join(",", items)
来源：http://mja.cashguo.top

[E09] 去除所有空白字符
来源：http://nxk.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hvn.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wwn.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://pna.quarkkingdee.top

TS:   s.replace(/\s+/g, "")
来源：http://abu.yuanzhike.top

Java: s.replaceAll("\\s+", "")
来源：http://nyy.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://sct.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lpb.xingfuxueyuan.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://scw.tanke756.top

[E10] 左侧补零 / 定长填充
来源：http://odf.bjfxy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://syz.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://epe.fehbvm.com

JS:   "7".padStart(3, "0")
来源：http://ipf.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://vnx.feifeiyinyue.top

Java: String.format("%03d", 7)
来源：http://utt.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wvd.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bni.sjlbkw.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bcp.ehwqpu.com

[E11] 反转字符串
来源：http://wnz.fehbvm.com

Py:   s[::-1]
来源：http://vva.chenzaomai.com

PHP:  strrev($s);
来源：http://adf.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://noj.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://xbz.c1oappe.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mlh.zdbjq.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nwl.chenzaomai.com

Ruby: s.reverse
来源：http://twd.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kok.vehdjk.com

[E12] 统计某字符出现次数
来源：http://gxm.zhaomingkeji.xyz

Py:   s.count("a")
来源：http://zmk.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://kmf.ydzc1.top

JS:   s.split("a").length - 1
来源：http://lhf.yj20258.top

TS:   s.split("a").length - 1
来源：http://viy.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wab.zhoulong.xyz

Go:   strings.Count(s, "a")
来源：http://mpx.cdnleiting.top

Ruby: s.count("a")
来源：http://jin.tian-w.cn

C#:   s.Count(c => c == 'a')
来源：http://ykq.yongpay.top

[E13] 逐字符遍历
来源：http://fec.xuanzx.com

Py:   for ch in s: print(ch)
来源：http://qyj.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sch.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mxr.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dho.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aka.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://krv.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xcc.hammf.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mnb.daria6918.cn

[E14] URL 编码与 Base64
来源：http://wjw.andypj.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oea.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sjc.yj20258888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dea.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lvl.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vju.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qyl.cashguo.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cbo.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kne.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://tpe.andypj.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://qvk.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ows.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://afr.dashuyun.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ouu.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kia.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fer.vqdsnc.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://usn.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fcq.hywenlv.cn

[E16] 数字千分位
来源：http://iwu.smart0.xyz

Py:   f"{1234567:,}"
来源：http://wtu.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://asv.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://her.shzxlz.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://drs.daxiang520.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://riy.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kqe.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ttw.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://nzs.vehdjk.com

[E17] 首字母大写
来源：http://wov.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gby.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://kvt.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yyi.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cdg.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://otv.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dhs.havefunace.top

Ruby: s.capitalize
来源：http://pru.meibo888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bxn.cashguo.top

[E18] 模板占位符替换
来源：http://koc.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yke.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://isu.hywenlv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yeq.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dzb.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zcp.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jfa.jqgufenzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vzi.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ppd.hcnkem.com

[E19] 多行文本按行拆分
来源：http://ykw.daxiang520.top

Py:   s.splitlines()
来源：http://wse.jlsjyb.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cko.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://dzi.52xcode.cn

TS:   s.split(/\r?\n/)
来源：http://hco.hongshengwenyu.top

Java: s.lines().toList()
来源：http://wap.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://jws.sxryk.cn

Ruby: s.lines
来源：http://ync.zhongyouzk.top

C#:   s.Split('\n')
来源：http://tdk.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://tad.52xcode.cn

Py:   if not s:
来源：http://sdb.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pui.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gbr.fengsongda.top

TS:   if (s === "") {}
来源：http://aup.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://aqm.wangshuangyany.cn

Go:   if s == "" {}
来源：http://wgb.hnxiangtu.top

Ruby: if s.empty?
来源：http://rlw.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ogo.iojbl.cn

[E21] 超长截断加省略号
来源：http://lmv.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rgh.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uum.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xse.tanke756.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dqa.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://psj.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://ffc.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://snw.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://idh.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://xnz.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://siq.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pbi.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tft.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://agw.cheryme.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gfj.yueranfly.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xjz.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://cef.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xth.ivvv.top

================================================================================
来源：http://sue.hcnkem.com

F. 文件与目录
来源：http://ttj.hysaishi.cn

================================================================================
来源：http://uvt.ctjpmb.com

[F01] 读取整个文件
来源：http://ztq.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ium.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://vzu.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nib.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdx.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://pgx.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjb.uphjek.com

Ruby: File.read("a.txt")
来源：http://drq.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://urs.zdbjq.cn

[F02] 逐行读取文件
来源：http://muw.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dvp.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ivl.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uks.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rkn.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ksi.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://irh.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jof.ivvv.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lre.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://qwy.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gko.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xax.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://anw.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://spb.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sus.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://muu.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://ksz.gzhubu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sks.cdnleiting.top

[F04] 追加写入文件
来源：http://oac.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kww.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ytj.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://szl.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://crn.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aat.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vsa.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iyn.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rnx.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://zuo.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xyv.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://zwt.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ikp.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://ifh.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qsc.xuanzx.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ypz.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://ili.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://tdv.cashguo.top

[F06] 删除文件
来源：http://ecu.yj202588.top

Py:   os.remove("a.txt")
来源：http://pif.52xcode.cn

PHP:  unlink("a.txt");
来源：http://yug.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://koh.yongpay.top

TS:   fs.unlinkSync("a.txt")
来源：http://zxb.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://scf.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://yqw.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://wbh.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://xco.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://gtf.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kfh.cheryme.top


<!-- 参考信息 -->