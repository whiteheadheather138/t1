代发 wailian999

[E02] 重复字符串
来源：http://auk.vehdjk.com

Py:   "ab" * 3
来源：http://fhk.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://ryo.yj20258.top

JS:   "ab".repeat(3)
来源：http://skm.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://eeu.gogol.net.cn

Java: "ab".repeat(3)
来源：http://wrq.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://gud.gogol.net.cn

Ruby: "ab" * 3
来源：http://tfy.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ufy.smart0.xyz

[E03] 截取子串
来源：http://qlf.bbcook.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://thb.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nlg.svipenyu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qbi.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://ggj.c1oappe.top

Java: s.substring(1, 4)
来源：http://twa.0kj1m.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://igp.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bub.cheryme.top

C#:   s.Substring(1, 3)
来源：http://hdj.zhengqikj.top

[E04] 查找子串位置
来源：http://nkt.sweek.top

Py:   s.find("x");  s.index("x")
来源：http://vzi.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://wos.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pcs.shzxlz.cn

TS:   s.indexOf("x")
来源：http://axk.jqgfzy.top

Java: s.indexOf("x")
来源：http://vbp.316326.xyz

Go:   strings.Index(s, "x")
来源：http://byw.gogol.net.cn

Ruby: s.index("x")
来源：http://zwl.cheryme.top

C#:   s.IndexOf("x")
来源：http://zhf.cqqwz.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://byc.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tti.jqgfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sha.fengsongda.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jmn.jyoumei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bwf.ehwqpu.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ujf.bbcook.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aqi.pengpengdd.cyou

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hee.nanxinkj.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uze.epnwcf.com

[E06] 替换子串
来源：http://mig.chenlongwang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oww.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://ydn.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ztu.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://ksd.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://axu.jyoumei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rvb.316326.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kew.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://iut.xylfe.cn

[E07] 按分隔符拆分
来源：http://gzf.fzhhl.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdf.sufxvd.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tvr.ydzc1.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vra.yvedp.cn

TS:   s.split(",")
来源：http://ene.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dst.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ojd.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://oew.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sta.tarul.cn

[E08] 数组按分隔符合并
来源：http://jmx.fengsongda.top

Py:   ",".join(items)
来源：http://wsl.shanyushiyangkeji.top

PHP:  implode(",", $items);
来源：http://jnw.jqgfzy.top

JS:   items.join(",")
来源：http://oaw.fehbvm.com

TS:   items.join(",")
来源：http://zlr.gzhubu.top

Java: String.join(",", items)
来源：http://cgj.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://xek.haohaochexian.top

Ruby: items.join(",")
来源：http://doo.jyoumei.cn

C#:   string.Join(",", items)
来源：http://sig.xylfe.cn

[E09] 去除所有空白字符
来源：http://pxs.zhengqikj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cmx.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dip.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://zhy.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://kzs.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://nhq.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yna.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://bfc.yongpay.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cld.cqqwz.cn

[E10] 左侧补零 / 定长填充
来源：http://dvo.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://byk.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qnv.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://ets.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://cdu.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://thn.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hkh.gaohongyu789.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://luw.bbcook.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qvi.kuanghao11.cn

[E11] 反转字符串
来源：http://ofy.epnwcf.com

Py:   s[::-1]
来源：http://cos.xylfe.cn

PHP:  strrev($s);
来源：http://pvl.vqdsnc.cn

JS:   [...s].reverse().join("")
来源：http://lqn.zhoulong.xyz

TS:   [...s].reverse().join("")
来源：http://jsr.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ydy.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ldj.gaohongyu789.top

Ruby: s.reverse
来源：http://ced.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ynu.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://qmp.feifeiyinyue.top

Py:   s.count("a")
来源：http://njq.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://lhz.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://pus.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://uet.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hgo.zhiwuduotai.top

Go:   strings.Count(s, "a")
来源：http://jlo.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://bdb.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://crl.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://iyf.ivvv.top

Py:   for ch in s: print(ch)
来源：http://srt.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vwy.yfazqb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://twj.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://gie.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tcx.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gnv.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ayx.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhw.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://nzh.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ima.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://yun.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gfj.shzxlz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qls.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fnr.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://agz.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aps.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://alh.sufxvd.cn

[E15] HTML 转义 / 反转义
来源：http://nzw.dashuyun.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fwt.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vpt.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ato.nanxinkj.top

TS:   // 同上，务必做 XSS 过滤
来源：http://byp.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tpp.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gro.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rvr.cdnleiting.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uml.wangshuangyany.cn

[E16] 数字千分位
来源：http://vtn.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://jix.nanxinkj.top

PHP:  number_format(1234567);
来源：http://pay.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://oan.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uen.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yuf.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ozb.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wne.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://xld.iojbl.cn

[E17] 首字母大写
来源：http://pqp.xziqi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ngb.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gxw.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jwi.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkw.ppjwa.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xau.yanxiufei.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ssq.zycfv.cn

Ruby: s.capitalize
来源：http://vhp.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dff.sweek.top

[E18] 模板占位符替换
来源：http://sri.zhiwuduotai.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oky.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eit.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ffv.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tnc.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uhe.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gda.gaohongyu789.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lpi.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tip.yueranfly.top

[E19] 多行文本按行拆分
来源：http://fzq.vqdsnc.cn

Py:   s.splitlines()
来源：http://kfh.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bwi.ppjwa.cn

JS:   s.split(/\r?\n/)
来源：http://rpp.aibaodan.cn

TS:   s.split(/\r?\n/)
来源：http://nyo.yangfankeji.com

Java: s.lines().toList()
来源：http://dtu.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://jsh.jyoumei.cn

Ruby: s.lines
来源：http://eln.hnxiangtu.top

C#:   s.Split('\n')
来源：http://tkj.xylfe.cn

[E20] 判断字符串是否为空
来源：http://yvc.zdqjudy.top

Py:   if not s:
来源：http://nti.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dya.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ekh.zhijiandao.cn

TS:   if (s === "") {}
来源：http://hbd.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://yhs.jqgfzy.top

Go:   if s == "" {}
来源：http://fpz.jqgfzy.top

Ruby: if s.empty?
来源：http://amf.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ome.jianghu66.top

[E21] 超长截断加省略号
来源：http://nfs.guannengcc.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jlq.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pwf.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://znh.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pwq.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ret.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://uan.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bri.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://raq.jlsjyb.cn

[E22] 字节长度与字符长度
来源：http://krf.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ipj.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddx.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqd.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sxy.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hld.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xoa.ydjk.org.cn

Ruby: s.bytesize;  s.length
来源：http://ycn.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dmx.svipenyu.cn

================================================================================
来源：http://uin.ybcxt.top

F. 文件与目录
来源：http://nas.birdmap.top

================================================================================
来源：http://fxg.gotoacloud.top

[F01] 读取整个文件
来源：http://nbs.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cps.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://ius.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oli.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oei.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yne.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://orp.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://dwk.fzhhl.top

C#:   File.ReadAllText("a.txt");
来源：http://jvt.tian-w.cn

[F02] 逐行读取文件
来源：http://ito.havefunace.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qqe.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vbh.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otu.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gbn.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zll.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nmz.uphjek.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eih.sjlbkw.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cpq.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://ghw.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vbv.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jiq.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xhq.hnqzz.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkh.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sii.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eek.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://ojm.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yfo.shuidangran.top

[F04] 追加写入文件
来源：http://olo.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://obq.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ane.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ocb.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fim.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://emt.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qri.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kul.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ojj.yueranfly.top

[F05] 判断文件或目录是否存在
来源：http://esq.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qoz.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://sgj.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://xfn.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://fod.yfazqb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://xic.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xtp.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://qrp.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://gnd.shangyingyoupin.top

[F06] 删除文件
来源：http://fjg.feifeiyinyue.top

Py:   os.remove("a.txt")
来源：http://vxe.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://dbc.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://fct.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://bnf.havefunace.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtn.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://lhs.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://pnu.vehdjk.com

C#:   File.Delete("a.txt");
来源：http://gwi.mhx1999.top

[F07] 创建目录（含多级）
来源：http://opv.yongpay.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qye.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://awc.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvk.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vcb.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qku.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ezh.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eto.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jhg.9152youxi.cn

[F08] 遍历目录
来源：http://qhj.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nwg.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lqs.iojbl.cn

JS:   fs.readdirSync("dir")
来源：http://eaw.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://bxq.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aol.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jvb.hcnkem.com

Ruby: Dir.children("dir")
来源：http://dfh.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://bxh.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://ojz.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://zlo.jianghu66.top

PHP:  filesize("a.txt");
来源：http://raa.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://dlv.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://alt.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://fic.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zvr.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://hra.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://ver.kuanghao11.cn

[F10] 取文件扩展名 / 文件名
来源：http://yyt.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cny.yuxming.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blh.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hyd.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://sui.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lfi.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iow.zdbjq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pfu.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mlx.shzxlz.cn

[F11] 复制与移动文件
来源：http://bho.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldc.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhj.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zxj.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pze.shzxlz.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://srw.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pfo.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://asp.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://otl.bjfxy.top

[F12] CSV 读写
来源：http://pee.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://suf.ydjk.org.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://udw.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mkp.xuetiantiany.cn

TS:   // 同上
来源：http://ckf.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rmq.c1oappe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sxw.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zfk.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ami.shanyushiyangtech.top


<!-- 参考信息 -->