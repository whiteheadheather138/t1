代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwx.ydzc1.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://htz.yj202588.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cyz.yangfankeji.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zzl.316326.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://eqf.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gla.ydjk.org.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vci.hysaishi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://why.yongpay.top

[E02] 重复字符串
来源：http://xyk.ctjpmb.com

Py:   "ab" * 3
来源：http://ejn.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://mog.xziqi.cn

JS:   "ab".repeat(3)
来源：http://eqo.ydzc1.top

TS:   "ab".repeat(3)
来源：http://sox.yangfankeji.com

Java: "ab".repeat(3)
来源：http://iaf.xinyue.icu

Go:   strings.Repeat("ab", 3)
来源：http://nua.shanyushiyangtech.top

Ruby: "ab" * 3
来源：http://yft.xuanzx.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wwj.snrcjt.cn

[E03] 截取子串
来源：http://rsy.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jsn.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jmr.xuanzx.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://msx.shangyingyoupin.top

TS:   s.slice(1, 4)
来源：http://quq.yueranfly.top

Java: s.substring(1, 4)
来源：http://fgg.gotoacloud.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zpm.zhongyouzk.top

Ruby: s[1, 3];  s[1..3]
来源：http://lak.fehbvm.com

C#:   s.Substring(1, 3)
来源：http://tuk.feifeiyinyue.top

[E04] 查找子串位置
来源：http://jkc.fzhhl.top

Py:   s.find("x");  s.index("x")
来源：http://skr.vqdsnc.cn

PHP:  strpos($s, "x");
来源：http://zcr.dianchejie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cga.316326.xyz

TS:   s.indexOf("x")
来源：http://qab.nwbrower.top

Java: s.indexOf("x")
来源：http://onl.c1oappe.top

Go:   strings.Index(s, "x")
来源：http://qbu.hongshengwenyu.top

Ruby: s.index("x")
来源：http://ctj.dashuyun.cn

C#:   s.IndexOf("x")
来源：http://arc.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ijd.shangyingyoupin.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://etv.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ehs.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://soh.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://vke.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://psg.quarkkingdee.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nip.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vpx.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thd.cdnleiting.top

[E06] 替换子串
来源：http://dlb.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cac.jlsjyb.cn

PHP:  str_replace("a", "b", $s);
来源：http://dqd.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yac.yonumen.top

TS:   s.replaceAll("a", "b")
来源：http://uqi.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xff.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ian.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wys.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://pts.fengsongda.top

[E07] 按分隔符拆分
来源：http://xwi.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hcd.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yqn.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://dha.bjfxy.top

TS:   s.split(",")
来源：http://mfi.jinqigufen.top

Java: s.split(",");  s.split("\\s+")
来源：http://gci.epnwcf.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wur.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://vgh.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://npy.iojbl.cn

[E08] 数组按分隔符合并
来源：http://noo.quarkkingdee.top

Py:   ",".join(items)
来源：http://lnq.tanke756.top

PHP:  implode(",", $items);
来源：http://iek.aizwys.cn

JS:   items.join(",")
来源：http://gsc.xinyue.icu

TS:   items.join(",")
来源：http://fhh.iojbl.cn

Java: String.join(",", items)
来源：http://fjb.quarkkingdee.top

Go:   strings.Join(items, ",")
来源：http://tmr.uphjek.com

Ruby: items.join(",")
来源：http://xwa.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://xur.fktsv.cn

[E09] 去除所有空白字符
来源：http://cco.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ccd.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://odq.jinghuilouyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://eki.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://yzv.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://zea.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kom.gogol.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oot.meibo888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://squ.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://yns.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lwr.chenjidiqi.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fvi.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://iyq.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://zmv.hammf.cn

Java: String.format("%03d", 7)
来源：http://vxt.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jsg.yj20258888.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nhl.aizwys.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qze.jlsjyb.cn

[E11] 反转字符串
来源：http://huz.cdnleiting.top

Py:   s[::-1]
来源：http://ujt.feifeiyinyue.top

PHP:  strrev($s);
来源：http://vuu.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://vxv.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://uyo.jqgufenzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://iyx.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://urd.ppjwa.cn

Ruby: s.reverse
来源：http://fyp.jqgfzy.top

C#:   new string(s.Reverse().ToArray())
来源：http://xav.fehbvm.com

[E12] 统计某字符出现次数
来源：http://nkc.ctjpmb.com

Py:   s.count("a")
来源：http://iua.iojbl.cn

PHP:  substr_count($s, "a");
来源：http://nhf.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://ybz.yangfankeji.com

TS:   s.split("a").length - 1
来源：http://egt.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uyu.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://pua.yongpay.top

Ruby: s.count("a")
来源：http://kpb.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://kkp.bjfxy.top

[E13] 逐字符遍历
来源：http://vrn.fanxiaobao.xyz

Py:   for ch in s: print(ch)
来源：http://vga.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://klu.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mwu.shanyushiyangtech.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zfl.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yay.shanyushiyangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://duq.shanyushiyangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ejv.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lle.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://amj.hfpthk.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xpc.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ohn.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bbt.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nqe.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lfz.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vep.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ffa.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://euq.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://qye.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://owp.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ajm.kuanghao11.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://szu.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tzo.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ang.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gvn.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jdj.yj20258.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kjl.nanxinkj.top

[E16] 数字千分位
来源：http://sdm.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://jkv.dianchejie.cn

PHP:  number_format(1234567);
来源：http://hjj.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://olh.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tdm.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wds.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cgd.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://txw.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://orl.tanke756.top

[E17] 首字母大写
来源：http://mbz.yfazqb.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ilc.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lik.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uam.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zxj.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qrh.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://waw.nanxinkj.top

Ruby: s.capitalize
来源：http://zvt.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vbo.pycfn.com

[E18] 模板占位符替换
来源：http://ibm.wangshuangyany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uiw.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dvr.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://atw.pengpengdd.cyou

TS:   tpl.replaceAll("{name}", name)
来源：http://fch.dashuyun.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fco.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cel.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kvl.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lwk.yonumen.top

[E19] 多行文本按行拆分
来源：http://vaz.hesvh.cn

Py:   s.splitlines()
来源：http://gen.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nkp.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://mxl.hongshengwenyu.top

TS:   s.split(/\r?\n/)
来源：http://mxc.jinqigufen.top

Java: s.lines().toList()
来源：http://tyr.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://hia.bjfxy.top

Ruby: s.lines
来源：http://gzi.gogol.net.cn

C#:   s.Split('\n')
来源：http://apm.zycfv.cn

[E20] 判断字符串是否为空
来源：http://rlp.sweek.top

Py:   if not s:
来源：http://bgq.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cng.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://twm.xuetiantiany.cn

TS:   if (s === "") {}
来源：http://jvg.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://ktg.hfpthk.cn

Go:   if s == "" {}
来源：http://iqb.havefunace.top

Ruby: if s.empty?
来源：http://kgb.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mai.cdnleiting.top

[E21] 超长截断加省略号
来源：http://zaj.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iku.fzhhl.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ofy.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cta.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yyb.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ghp.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://fxz.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ysl.vehdjk.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wlr.daria6918.cn

[E22] 字节长度与字符长度
来源：http://wwl.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oah.xziqi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://edr.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://asw.dashuyun.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qlf.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vem.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bat.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://ezl.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jbp.aibaodan.cn

================================================================================
来源：http://qkg.ydzc1.top

F. 文件与目录
来源：http://qpu.yj202588.top

================================================================================
来源：http://uyk.ybcxt.top

[F01] 读取整个文件
来源：http://ula.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://deq.zhongyouzk.top

PHP:  file_get_contents("a.txt");
来源：http://rzw.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tmp.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ywd.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://mto.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ndf.fzhhl.top

Ruby: File.read("a.txt")
来源：http://yll.zhoulong.xyz

C#:   File.ReadAllText("a.txt");
来源：http://igw.jqgfzy.top

[F02] 逐行读取文件
来源：http://yvb.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nit.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lwt.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rwz.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uhp.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tfz.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vbd.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyb.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://avg.tarul.cn

[F03] 写入文件（覆盖）
来源：http://jkh.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://few.havefunace.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qrt.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://esx.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ows.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ymv.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iwq.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://aci.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohz.hfpthk.cn

[F04] 追加写入文件
来源：http://xqi.52xcode.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://avk.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uxw.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ama.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qwl.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eyu.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mft.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cyd.hongshengwenyu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sib.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://kxn.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyn.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://bex.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://myu.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://qqp.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pcl.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tjn.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://zfx.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://gxj.ctjpmb.com

[F06] 删除文件
来源：http://pjz.fengsongda.top

Py:   os.remove("a.txt")
来源：http://byw.fzhhl.top

PHP:  unlink("a.txt");
来源：http://bks.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ikc.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://irb.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ytg.sxryk.cn

Go:   os.Remove("a.txt")
来源：http://ryk.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://cym.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://ywf.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://zyu.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jfa.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jxd.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkq.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://loi.yj202588.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nyg.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ovh.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wwu.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qkh.zycfv.cn

[F08] 遍历目录
来源：http://ckn.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kxa.yvedp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ehy.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://rzo.cashguo.top

TS:   fs.readdirSync("dir")
来源：http://vtr.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ats.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://moq.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://ukx.xuetiantiany.cn

C#:   Directory.GetFiles("dir")
来源：http://bxz.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://jsh.yongpay.top

Py:   os.path.getsize("a.txt")
来源：http://tbq.iojbl.cn

PHP:  filesize("a.txt");
来源：http://etw.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://uwg.jqgufenzy.top

TS:   fs.statSync("a.txt").size
来源：http://zjq.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://xfv.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ahy.birdmap.top

Ruby: File.size("a.txt")
来源：http://egn.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://bqo.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://qra.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oyd.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uup.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://muj.cucudq.cn

TS:   path.extname("a.txt")
来源：http://cbr.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ipt.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ozh.dianchejie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sfi.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mfy.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://xnp.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xxr.wangshuangyany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://frz.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbl.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azb.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://swv.meibo888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nsd.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ajr.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kin.zdbjq.cn

[F12] CSV 读写
来源：http://nsg.ctjpmb.com


<!-- 参考信息 -->