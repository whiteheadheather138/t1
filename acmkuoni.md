代发 wailian999

Java: String.join(", ", list)
来源：http://qyk.cashguo.top

Go:   strings.Join(strs, ", ")
来源：http://wox.wangdashe.top

Ruby: arr.join(", ")
来源：http://erv.daxiang520.top

C#:   string.Join(", ", list)
来源：http://egy.jqgufenzy.top

================================================================================
来源：http://hth.bbcook.cn

E. 字符串处理
来源：http://ifn.ybcxt.top

================================================================================
来源：http://vpe.hysaishi.cn

[E01] 拼接字符串
来源：http://mfo.yanxiufei.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://shu.redwolf501.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://alw.fengsongda.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://niw.tarul.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vtj.havefunace.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cif.iojbl.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ejv.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cra.jiagoushi.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ypp.chenlongwang.top

[E02] 重复字符串
来源：http://qce.havefunace.top

Py:   "ab" * 3
来源：http://kes.kuanghao11.cn

PHP:  str_repeat("ab", 3);
来源：http://ojl.fengsongda.top

JS:   "ab".repeat(3)
来源：http://yyi.9152youxi.cn

TS:   "ab".repeat(3)
来源：http://xck.zhengqikj.top

Java: "ab".repeat(3)
来源：http://qis.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://ypp.gzhubu.top

Ruby: "ab" * 3
来源：http://lnu.fengsongda.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hoy.sxryk.cn

[E03] 截取子串
来源：http://kka.sysykeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dmo.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rrm.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://snc.sysykeji.top

TS:   s.slice(1, 4)
来源：http://fez.fehbvm.com

Java: s.substring(1, 4)
来源：http://smw.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yan.yj20258888.top

Ruby: s[1, 3];  s[1..3]
来源：http://jaj.birdmap.top

C#:   s.Substring(1, 3)
来源：http://kou.yj20258.top

[E04] 查找子串位置
来源：http://woo.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://kxh.chenzaomai.com

PHP:  strpos($s, "x");
来源：http://nro.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ije.zhijiandao.cn

TS:   s.indexOf("x")
来源：http://xmf.cheryme.top

Java: s.indexOf("x")
来源：http://pmn.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://ywi.zhengqikj.top

Ruby: s.index("x")
来源：http://afv.andypj.xyz

C#:   s.IndexOf("x")
来源：http://rhi.gotoacloud.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cqa.iojbl.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://htr.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cko.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hql.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ybc.zhiwuduotai.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://riq.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://eoa.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sqr.hongshengwenyu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lyl.shuidangran.top

[E06] 替换子串
来源：http://wph.hongshengwenyu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vcf.xziqi.cn

PHP:  str_replace("a", "b", $s);
来源：http://dnk.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bmz.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://gib.yvedp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qne.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cws.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cpx.hammf.cn

C#:   s.Replace("a", "b")
来源：http://xrd.meibo888.top

[E07] 按分隔符拆分
来源：http://ief.ivvv.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gjm.gotoacloud.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jfl.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ysc.gaohongyu789.top

TS:   s.split(",")
来源：http://vuj.xuanzx.com

Java: s.split(",");  s.split("\\s+")
来源：http://gxr.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qol.snrcjt.cn

Ruby: s.split(",");  s.split
来源：http://vdw.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qfm.xuetiantiany.cn

[E08] 数组按分隔符合并
来源：http://ntq.birdmap.top

Py:   ",".join(items)
来源：http://gnn.pycfn.com

PHP:  implode(",", $items);
来源：http://fdj.gotoacloud.top

JS:   items.join(",")
来源：http://mjt.sjlbkw.cn

TS:   items.join(",")
来源：http://tuz.zhengqikj.top

Java: String.join(",", items)
来源：http://gkm.sjlbkw.cn

Go:   strings.Join(items, ",")
来源：http://yhn.vehdjk.com

Ruby: items.join(",")
来源：http://mdf.yongpay.top

C#:   string.Join(",", items)
来源：http://ovw.52xcode.cn

[E09] 去除所有空白字符
来源：http://dhf.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wav.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lej.dashuyun.cn

JS:   s.replace(/\s+/g, "")
来源：http://xer.ydjk.org.cn

TS:   s.replace(/\s+/g, "")
来源：http://uzr.yfazqb.com

Java: s.replaceAll("\\s+", "")
来源：http://gpv.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://oxs.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://rys.yuxming.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://imw.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://xhq.gaohongyu789.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kss.gogol.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://egn.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://myy.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://lwc.shanyushiyangkeji.top

Java: String.format("%03d", 7)
来源：http://yra.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://elj.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zho.gzhubu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bde.0kj1m.cn

[E11] 反转字符串
来源：http://ong.bbcook.cn

Py:   s[::-1]
来源：http://pee.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://dcu.tanke756.top

JS:   [...s].reverse().join("")
来源：http://xsw.redwolf501.top

TS:   [...s].reverse().join("")
来源：http://tps.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jri.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jym.xuanzx.com

Ruby: s.reverse
来源：http://pdl.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ghf.hammf.cn

[E12] 统计某字符出现次数
来源：http://uuv.redwolf501.top

Py:   s.count("a")
来源：http://vaa.ybcxt.top

PHP:  substr_count($s, "a");
来源：http://tnl.guowangkeji.top

JS:   s.split("a").length - 1
来源：http://ukm.meibo888.top

TS:   s.split("a").length - 1
来源：http://svp.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://osh.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://xjn.ydjk.org.cn

Ruby: s.count("a")
来源：http://oax.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://pcf.gaohongyu789.top

[E13] 逐字符遍历
来源：http://cym.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://irj.uphjek.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gyt.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uzc.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://mxm.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wcr.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sdx.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qly.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yzl.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://vws.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fxh.pycfn.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://znp.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://igx.bjfxy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fyu.vqdsnc.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xcq.aibaodan.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qje.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mcn.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bhy.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://dme.yongpay.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gek.ivvv.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://caa.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wqh.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://woz.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://flo.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wav.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://evo.yuanzhike.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zru.yonumen.top

[E16] 数字千分位
来源：http://mxa.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://onv.ivvv.top

PHP:  number_format(1234567);
来源：http://dbh.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yoy.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://cyf.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://egm.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xxz.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kdu.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://paw.hysaishi.cn

[E17] 首字母大写
来源：http://jgg.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kfn.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ryn.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ubi.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzk.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oqm.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vkc.vehdjk.com

Ruby: s.capitalize
来源：http://upy.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rca.cdnleiting.top

[E18] 模板占位符替换
来源：http://nfp.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bko.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ana.shuidangran.top

JS:   tpl.replaceAll("{name}", name)
来源：http://muz.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://etp.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fmc.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vrb.hesvh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://slc.daria6918.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mzp.yueranfly.top

[E19] 多行文本按行拆分
来源：http://lyo.jiagoushi.top

Py:   s.splitlines()
来源：http://xpv.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ymx.zhoulong.xyz

JS:   s.split(/\r?\n/)
来源：http://icp.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://naw.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://dii.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://ags.yanxiufei.cn

Ruby: s.lines
来源：http://wlu.yfazqb.com

C#:   s.Split('\n')
来源：http://ygd.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://nmc.hammf.cn

Py:   if not s:
来源：http://cqf.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://guq.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://htm.fehbvm.com

TS:   if (s === "") {}
来源：http://bye.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://rjw.chenjidiqi.icu

Go:   if s == "" {}
来源：http://yxn.havefunace.top

Ruby: if s.empty?
来源：http://out.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lhl.chenlongwang.top

[E21] 超长截断加省略号
来源：http://rdx.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ybq.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://meb.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xla.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iaa.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cfp.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://mms.pengpengdd.cyou

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fzy.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghv.sweek.top

[E22] 字节长度与字符长度
来源：http://rdp.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pjz.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gze.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ybp.jyoumei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fyv.cucudq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xzd.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rsd.yuxming.cn

Ruby: s.bytesize;  s.length
来源：http://ngu.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fjt.fehbvm.com

================================================================================
来源：http://urf.yvedp.cn

F. 文件与目录
来源：http://hed.shuidangran.top

================================================================================
来源：http://qyx.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://uwp.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fgl.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://mzu.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dtc.gogol.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ubv.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mxq.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://byc.yuanzhike.top

Ruby: File.read("a.txt")
来源：http://jup.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://wyg.hysaishi.cn

[F02] 逐行读取文件
来源：http://mga.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://izm.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oqj.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://msi.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cgc.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eyh.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aln.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://aha.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://whg.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://tne.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqy.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mro.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rho.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://adq.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aue.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qhp.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://qtf.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hfh.fehbvm.com

[F04] 追加写入文件
来源：http://pak.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://une.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://adp.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xub.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkz.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lif.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://npq.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uwi.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hsg.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://kbw.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eht.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://mnk.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://ymh.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://vir.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wov.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tvn.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://xni.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://qlw.xziqi.cn

[F06] 删除文件
来源：http://tnr.yj20258.top

Py:   os.remove("a.txt")
来源：http://dlr.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://ipb.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://qdk.hongshengwenyu.top

TS:   fs.unlinkSync("a.txt")
来源：http://vir.hesvh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fbr.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://dho.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://oxr.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://kha.fengsongda.top

[F07] 创建目录（含多级）
来源：http://uyt.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vbf.jqgfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ybl.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cqu.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fzo.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://veu.nanxuanxn.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://otc.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ejp.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jef.hnxiangtu.top

[F08] 遍历目录
来源：http://wbo.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dhk.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sva.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://yts.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://bcg.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wqi.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://eqa.birdmap.top

Ruby: Dir.children("dir")
来源：http://ims.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://hmg.svipenyu.cn

[F09] 获取文件大小
来源：http://jzq.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://qtx.fzhhl.top

PHP:  filesize("a.txt");
来源：http://qoz.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://ulf.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://gcr.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://vwz.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mbv.nwbrower.top

Ruby: File.size("a.txt")
来源：http://ajw.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://zls.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://sif.zhongyouzk.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vbp.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bgj.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hym.ivvv.top

TS:   path.extname("a.txt")
来源：http://obz.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lgf.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clc.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kjd.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rvt.gaohongyu789.top

[F11] 复制与移动文件
来源：http://gvv.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tam.nanxuanxn.top


<!-- 参考信息 -->