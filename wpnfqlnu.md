代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kvm.xuanzx.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://axi.vqdsnc.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cob.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yht.epnwcf.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bbu.chenjidiqi.icu

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gcp.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://cmm.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fbf.jianghu66.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vjh.hywenlv.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wgw.ppjwa.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://neo.uphjek.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://zhp.sjlbkw.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://toq.yuanzhike.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ouo.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tkq.jqgufenzy.top

[D26] 数组转字符串
来源：http://oox.yangfankeji.com

Py:   ", ".join(map(str, arr))
来源：http://jbt.tian-w.cn

PHP:  implode(", ", $arr);
来源：http://orp.c1oappe.top

JS:   arr.join(", ")
来源：http://vqm.xingfuxueyuan.xyz

TS:   arr.join(", ")
来源：http://zpa.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://cxd.zdqjudy.top

Go:   strings.Join(strs, ", ")
来源：http://tvd.jlsjyb.cn

Ruby: arr.join(", ")
来源：http://ner.xylfe.cn

C#:   string.Join(", ", list)
来源：http://zjq.dashuyun.cn

================================================================================
来源：http://yrw.ehwqpu.com

E. 字符串处理
来源：http://bno.meibo888.top

================================================================================
来源：http://poc.hammf.cn

[E01] 拼接字符串
来源：http://izo.chenjidiqi.icu

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nvc.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zoj.ehwqpu.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://auk.zdbjq.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yyx.wangdashe.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://glk.wangdashe.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://otu.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gom.gogol.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://fmh.zdqjudy.top

[E02] 重复字符串
来源：http://qpr.jiagoushi.top

Py:   "ab" * 3
来源：http://zxx.andypj.xyz

PHP:  str_repeat("ab", 3);
来源：http://boa.yfazqb.com

JS:   "ab".repeat(3)
来源：http://lrt.zhijiandao.cn

TS:   "ab".repeat(3)
来源：http://obr.yongpay.top

Java: "ab".repeat(3)
来源：http://ydc.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://vxd.shzxlz.cn

Ruby: "ab" * 3
来源：http://mih.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mto.xinyue.icu

[E03] 截取子串
来源：http://tai.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ior.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vkm.nwbrower.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mmz.jinqigufen.top

TS:   s.slice(1, 4)
来源：http://duo.yuxming.cn

Java: s.substring(1, 4)
来源：http://epz.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://orq.hesvh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ysz.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://gji.jinqigufen.top

[E04] 查找子串位置
来源：http://zqx.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://wyw.ctjpmb.com

PHP:  strpos($s, "x");
来源：http://csf.daria6918.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://goh.0kj1m.cn

TS:   s.indexOf("x")
来源：http://ngt.uphjek.com

Java: s.indexOf("x")
来源：http://ejx.wangshuangyany.cn

Go:   strings.Index(s, "x")
来源：http://hjn.ctjpmb.com

Ruby: s.index("x")
来源：http://uzz.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://auh.cheryme.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://fag.jlsjyb.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wsi.c1oappe.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lwm.vehdjk.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jgp.jinqigfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hic.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rri.tian-w.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kqt.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jla.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gwm.andypj.xyz

[E06] 替换子串
来源：http://ipw.yj20258888.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pdx.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://kep.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dwn.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://kih.aibaodan.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://edh.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oza.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cvz.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://unn.sxryk.cn

[E07] 按分隔符拆分
来源：http://jli.kuanghao11.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kan.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvv.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbb.ydjk.org.cn

TS:   s.split(",")
来源：http://uff.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://vlj.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uit.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://zfh.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lhi.gotoacloud.top

[E08] 数组按分隔符合并
来源：http://uli.zhengqikj.top

Py:   ",".join(items)
来源：http://ala.hammf.cn

PHP:  implode(",", $items);
来源：http://obf.52xcode.cn

JS:   items.join(",")
来源：http://yjg.yuxming.cn

TS:   items.join(",")
来源：http://ayq.9152youxi.cn

Java: String.join(",", items)
来源：http://fll.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://cgz.tarul.cn

Ruby: items.join(",")
来源：http://bvk.yj20258.top

C#:   string.Join(",", items)
来源：http://jqj.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://zfc.hcnkem.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kyu.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://knd.yuanzhike.top

JS:   s.replace(/\s+/g, "")
来源：http://rny.zhoulong.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ayy.zhaomingkeji.xyz

Java: s.replaceAll("\\s+", "")
来源：http://isv.svipenyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hvr.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kzl.ctjpmb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baj.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://off.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ogu.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hch.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://aak.ehwqpu.com

TS:   "7".padStart(3, "0")
来源：http://afb.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://bxf.sxryk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ich.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://myf.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oxt.yfazqb.com

[E11] 反转字符串
来源：http://kmu.jyoumei.cn

Py:   s[::-1]
来源：http://ype.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://jcl.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://fkt.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://ojb.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jmw.gotoacloud.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bxn.shangyingyoupin.top

Ruby: s.reverse
来源：http://xpx.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://fgj.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://noq.meibo888.top

Py:   s.count("a")
来源：http://ujm.tanke756.top

PHP:  substr_count($s, "a");
来源：http://ffp.epnwcf.com

JS:   s.split("a").length - 1
来源：http://vpu.jlsjyb.cn

TS:   s.split("a").length - 1
来源：http://gai.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yfn.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://jip.snrcjt.cn

Ruby: s.count("a")
来源：http://jlp.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://ryd.redwolf501.top

[E13] 逐字符遍历
来源：http://pqv.ywan-chungtsiang.top

Py:   for ch in s: print(ch)
来源：http://hry.jyoumei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ral.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://wwm.chenlongwang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://yiw.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fab.sxryk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qzh.sysykeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://pqr.fktsv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ivm.nwbrower.top

[E14] URL 编码与 Base64
来源：http://xnv.xuetiantiany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://moe.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oeu.gzhubu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ifh.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oym.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xwf.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ngf.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ric.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ofy.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://qee.jinyuanbaomall.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pvb.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zcj.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dqr.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cnh.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mjm.uphjek.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tdj.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://box.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fce.hnqzz.top

[E16] 数字千分位
来源：http://wyi.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://une.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://nhi.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gwd.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ybm.cucudq.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tam.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wep.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zky.yj20258.top

C#:   1234567.ToString("N0")
来源：http://vel.vqdsnc.cn

[E17] 首字母大写
来源：http://ujf.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kwm.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gpt.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afw.yanxiufei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zfo.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nrs.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fcg.smart0.xyz

Ruby: s.capitalize
来源：http://pdt.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbb.sysykeji.top

[E18] 模板占位符替换
来源：http://seh.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ufc.bjfxy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dzh.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ccp.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wug.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wiv.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gop.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ohm.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ctm.nwbrower.top

[E19] 多行文本按行拆分
来源：http://tkp.yfazqb.com

Py:   s.splitlines()
来源：http://bdv.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mqd.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://bls.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://dzs.ehwqpu.com

Java: s.lines().toList()
来源：http://swt.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://pnd.yueranfly.top

Ruby: s.lines
来源：http://mec.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://eiz.sysykeji.top

[E20] 判断字符串是否为空
来源：http://fmq.zhiwuduotai.top

Py:   if not s:
来源：http://kvz.jinghuilouyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ggd.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://myp.svipenyu.cn

TS:   if (s === "") {}
来源：http://ovp.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://ssd.chenzaomai.com

Go:   if s == "" {}
来源：http://nlg.jinqigufen.top

Ruby: if s.empty?
来源：http://esu.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yxc.fktsv.cn

[E21] 超长截断加省略号
来源：http://mva.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kgu.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://whm.quarkkingdee.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckr.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://buy.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mex.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://cmv.bbcook.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kkr.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ujt.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://tqt.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwh.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oyr.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ery.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jic.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uyn.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://guj.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://gbp.yj20258.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lle.jiagoushi.top

================================================================================
来源：http://fsd.shanyushiyangtech.top

F. 文件与目录
来源：http://dqs.wangdashe.top

================================================================================
来源：http://hdn.vqdsnc.cn

[F01] 读取整个文件
来源：http://wio.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nnr.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://dnh.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://upz.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gwr.bbcook.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://iip.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://krw.guannengcc.top

Ruby: File.read("a.txt")
来源：http://exw.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://gbn.zhoulong.xyz

[F02] 逐行读取文件
来源：http://jks.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zia.xingfuxueyuan.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mzh.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jut.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gok.gzhubu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rpx.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bbk.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://voe.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbh.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://cuz.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aux.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://cjo.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzf.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qpq.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hjc.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rge.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://yia.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ccj.wangdashe.top

[F04] 追加写入文件
来源：http://kmu.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ztc.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cjw.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lrb.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pws.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://igj.xziqi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bxe.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yzu.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ngb.chenzaomai.com

[F05] 判断文件或目录是否存在
来源：http://gxh.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ttr.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://smn.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://uzl.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://mag.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wke.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wmc.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://ark.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://hcu.svipenyu.cn

[F06] 删除文件
来源：http://azc.xinyue.icu

Py:   os.remove("a.txt")
来源：http://slg.xuetiantiany.cn

PHP:  unlink("a.txt");
来源：http://nrs.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://gyi.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://vck.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kaj.yj202588.top

Go:   os.Remove("a.txt")
来源：http://olg.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://bku.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://cku.c1oappe.top

[F07] 创建目录（含多级）
来源：http://fvc.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iec.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ylw.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ums.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ctd.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://snf.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fgc.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mzj.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sai.xuetiantiany.cn

[F08] 遍历目录
来源：http://jmn.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://acb.vqdsnc.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ala.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://cuh.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://zsl.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mvz.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sbb.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://vkl.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://dgd.hcnkem.com


<!-- 参考信息 -->