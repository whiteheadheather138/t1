代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://rgp.tarul.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dod.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://cww.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://awx.shanyushiyangtech.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rxw.guowangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vlt.bbcook.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://llm.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wdg.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mig.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hpb.hongshengwenyu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gbn.meibo888.top

[D26] 数组转字符串
来源：http://lrc.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://has.smart0.xyz

PHP:  implode(", ", $arr);
来源：http://xma.iojbl.cn

JS:   arr.join(", ")
来源：http://myh.xziqi.cn

TS:   arr.join(", ")
来源：http://var.ybcxt.top

Java: String.join(", ", list)
来源：http://cig.yuanzhike.top

Go:   strings.Join(strs, ", ")
来源：http://shl.guannengcc.top

Ruby: arr.join(", ")
来源：http://tmq.hnxiangtu.top

C#:   string.Join(", ", list)
来源：http://jah.sweek.top

================================================================================
来源：http://dur.jinghuilouyu.cn

E. 字符串处理
来源：http://zlx.jyoumei.cn

================================================================================
来源：http://fzu.316326.xyz

[E01] 拼接字符串
来源：http://ifn.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bnj.gotoacloud.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cfo.smart0.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lsx.kuanghao11.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ndx.tanke756.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xye.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://amm.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://afx.hammf.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rjb.hfpthk.cn

[E02] 重复字符串
来源：http://ofe.ivvv.top

Py:   "ab" * 3
来源：http://fii.gogol.net.cn

PHP:  str_repeat("ab", 3);
来源：http://qwn.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://srg.jqgfzy.top

TS:   "ab".repeat(3)
来源：http://zfn.ctjpmb.com

Java: "ab".repeat(3)
来源：http://fkq.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://ddv.jiagoushi.top

Ruby: "ab" * 3
来源：http://ohi.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://brx.yongpay.top

[E03] 截取子串
来源：http://hwo.yuanzhike.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dds.yj20258.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yhe.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fhr.zdbjq.cn

TS:   s.slice(1, 4)
来源：http://mre.tanke756.top

Java: s.substring(1, 4)
来源：http://zje.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fad.ywan-chungtsiang.top

Ruby: s[1, 3];  s[1..3]
来源：http://ydj.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://lhm.jinqigfzy.top

[E04] 查找子串位置
来源：http://opx.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://isa.dianchejie.cn

PHP:  strpos($s, "x");
来源：http://mjx.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yth.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://wrr.cashguo.top

Java: s.indexOf("x")
来源：http://kkp.sxryk.cn

Go:   strings.Index(s, "x")
来源：http://jgk.nanxuanxn.top

Ruby: s.index("x")
来源：http://xqm.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://czg.snrcjt.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rwj.tian-w.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qlc.52xcode.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pje.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kvg.0kj1m.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xxz.shanyushiyangtech.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://usb.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jtj.yongpay.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://moj.hammf.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://his.pycfn.com

[E06] 替换子串
来源：http://umx.sufxvd.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mjd.zhongyouzk.top

PHP:  str_replace("a", "b", $s);
来源：http://pxj.shanyushiyangkeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dis.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://jvj.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uex.fzhhl.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mzb.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jof.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://vlq.cucudq.cn

[E07] 按分隔符拆分
来源：http://zoc.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hga.hesvh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cza.shanyushiyangkeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cdc.havefunace.top

TS:   s.split(",")
来源：http://lqw.ehwqpu.com

Java: s.split(",");  s.split("\\s+")
来源：http://daq.jinqigfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qzb.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://xsi.nanxinkj.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ybt.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://ljv.pycfn.com

Py:   ",".join(items)
来源：http://wnx.yuanzhike.top

PHP:  implode(",", $items);
来源：http://svp.ywan-chungtsiang.top

JS:   items.join(",")
来源：http://fsr.chenjidiqi.icu

TS:   items.join(",")
来源：http://bou.52xcode.cn

Java: String.join(",", items)
来源：http://ayy.daria6918.cn

Go:   strings.Join(items, ",")
来源：http://sin.nanxinkj.top

Ruby: items.join(",")
来源：http://eta.mhx1999.top

C#:   string.Join(",", items)
来源：http://ceb.zhoulong.xyz

[E09] 去除所有空白字符
来源：http://pfy.xinyue.icu

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sxy.pengpengdd.cyou

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mke.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://mga.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://qjw.vqdsnc.cn

Java: s.replaceAll("\\s+", "")
来源：http://csa.cheryme.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gfb.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fow.zhiwuduotai.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://euz.316326.xyz

[E10] 左侧补零 / 定长填充
来源：http://kap.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pfa.haohaochexian.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ecq.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://hzd.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://eql.gotoacloud.top

Java: String.format("%03d", 7)
来源：http://yhc.shangyingyoupin.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lxg.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kpf.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fzm.hcnkem.com

[E11] 反转字符串
来源：http://ylw.yonumen.top

Py:   s[::-1]
来源：http://ztp.guowangkeji.top

PHP:  strrev($s);
来源：http://obk.havefunace.top

JS:   [...s].reverse().join("")
来源：http://ftl.tarul.cn

TS:   [...s].reverse().join("")
来源：http://kmq.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://min.yangfankeji.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://tro.zhoulong.xyz

Ruby: s.reverse
来源：http://xkh.shuidangran.top

C#:   new string(s.Reverse().ToArray())
来源：http://ipy.chenzaomai.com

[E12] 统计某字符出现次数
来源：http://kck.hammf.cn

Py:   s.count("a")
来源：http://fvi.jyoumei.cn

PHP:  substr_count($s, "a");
来源：http://bns.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://wfo.ehwqpu.com

TS:   s.split("a").length - 1
来源：http://zxt.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sev.uphjek.com

Go:   strings.Count(s, "a")
来源：http://xsq.yj20258.top

Ruby: s.count("a")
来源：http://lvy.yongpay.top

C#:   s.Count(c => c == 'a')
来源：http://pot.fengsongda.top

[E13] 逐字符遍历
来源：http://sfz.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://oiy.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvj.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://jfq.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rjp.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qzp.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://olv.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vbg.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iun.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://kya.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lum.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://gpn.cashguo.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mva.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fdb.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vqa.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zvj.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fhd.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxe.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://wwk.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xyh.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wmj.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bwr.zhixingplan.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ejn.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gsx.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jtx.nanxuanxn.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xxr.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xhf.fanxiaobao.xyz

[E16] 数字千分位
来源：http://wcb.tanke756.top

Py:   f"{1234567:,}"
来源：http://taw.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://pgi.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://vmq.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tya.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mge.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qmo.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bqj.daxiang520.top

C#:   1234567.ToString("N0")
来源：http://kby.xylfe.cn

[E17] 首字母大写
来源：http://nqw.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rci.gogol.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xpp.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ctn.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kwm.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://icp.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ivy.chenzaomai.com

Ruby: s.capitalize
来源：http://dil.jqgfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rtc.hysaishi.cn

[E18] 模板占位符替换
来源：http://kgl.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rrt.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xul.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://iaj.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ibk.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fsb.52xcode.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mrz.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xil.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cic.hcnkem.com

[E19] 多行文本按行拆分
来源：http://uuj.sufxvd.cn

Py:   s.splitlines()
来源：http://gbf.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lsb.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://gyz.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://bij.shuidangran.top

Java: s.lines().toList()
来源：http://jek.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://eko.sweek.top

Ruby: s.lines
来源：http://oab.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://rmv.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://qmt.hongshengwenyu.top

Py:   if not s:
来源：http://ngo.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://esz.uphjek.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qgo.guowangkeji.top

TS:   if (s === "") {}
来源：http://rkf.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://uoi.daxiang520.top

Go:   if s == "" {}
来源：http://bwh.yvedp.cn

Ruby: if s.empty?
来源：http://kod.yvedp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xaf.zhongyouzk.top

[E21] 超长截断加省略号
来源：http://uet.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gbv.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wyx.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jgx.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://stu.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://odw.nanxuanxn.top

Go:   // 按 rune 判断长度后截断
来源：http://ygd.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebi.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tev.vehdjk.com

[E22] 字节长度与字符长度
来源：http://upv.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iva.kuanghao11.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvf.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zak.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://god.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ttp.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ptk.bjfxy.top

Ruby: s.bytesize;  s.length
来源：http://udf.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fza.haohaochexian.top

================================================================================
来源：http://gab.yongpay.top

F. 文件与目录
来源：http://axh.shanyushiyangkeji.top

================================================================================
来源：http://wuo.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://btt.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gek.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://puo.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lsq.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qwx.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dau.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fwf.yfazqb.com

Ruby: File.read("a.txt")
来源：http://sck.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://kvl.haohaochexian.top

[F02] 逐行读取文件
来源：http://wtr.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://byv.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqh.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uwh.wangshuangyany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxo.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ilo.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://grv.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uwa.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gdn.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://ocx.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qgy.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pyy.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ehj.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjc.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yfm.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eud.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://vqv.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://csz.yj202588.top

[F04] 追加写入文件
来源：http://uxh.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://buq.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://igv.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nhj.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wpc.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fty.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kkc.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kqv.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pzo.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://hcx.mhx1999.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmk.uphjek.com

PHP:  file_exists("a.txt");
来源：http://vzq.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://vnd.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://edx.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sva.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyk.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://idw.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://yqq.hongshengwenyu.top

[F06] 删除文件
来源：http://xca.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://ttc.daxiang520.top

PHP:  unlink("a.txt");
来源：http://xzu.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://yll.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://clr.andypj.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oqq.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://kpa.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://agv.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://tva.hesvh.cn

[F07] 创建目录（含多级）
来源：http://gvy.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ssl.hcnkem.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uet.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lyv.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gga.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://efx.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ozt.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pbx.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wbz.redwolf501.top

[F08] 遍历目录
来源：http://wck.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bfp.chenzaomai.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://boj.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://zfn.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://yvl.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://prr.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lxi.meibo888.top

Ruby: Dir.children("dir")
来源：http://xtz.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://wzb.xziqi.cn

[F09] 获取文件大小
来源：http://dtk.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://mrj.316326.xyz

PHP:  filesize("a.txt");
来源：http://bgp.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://ocx.iojbl.cn


<!-- 参考信息 -->