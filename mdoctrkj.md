代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vly.hnxiangtu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iaj.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://axc.9152youxi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xga.hnqzz.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://drd.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wyy.cdnleiting.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lhy.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yys.cheryme.top

[E02] 重复字符串
来源：http://twv.xinyue.icu

Py:   "ab" * 3
来源：http://arz.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://gai.316326.xyz

JS:   "ab".repeat(3)
来源：http://hsw.jinqigfzy.top

TS:   "ab".repeat(3)
来源：http://pqs.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://jhg.jinqigufen.top

Go:   strings.Repeat("ab", 3)
来源：http://hir.0kj1m.cn

Ruby: "ab" * 3
来源：http://npx.gaohongyu789.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://utx.yueranfly.top

[E03] 截取子串
来源：http://jow.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ust.jiagoushi.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxz.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ncs.zycfv.cn

TS:   s.slice(1, 4)
来源：http://nvn.uphjek.com

Java: s.substring(1, 4)
来源：http://xim.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://onc.shangyingyoupin.top

Ruby: s[1, 3];  s[1..3]
来源：http://hhy.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://ogy.yj202588.top

[E04] 查找子串位置
来源：http://gqu.fktsv.cn

Py:   s.find("x");  s.index("x")
来源：http://esi.chenlongwang.top

PHP:  strpos($s, "x");
来源：http://asa.bbcook.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ocg.sufxvd.cn

TS:   s.indexOf("x")
来源：http://pxy.aibaodan.cn

Java: s.indexOf("x")
来源：http://miy.shanyushiyangkeji.top

Go:   strings.Index(s, "x")
来源：http://gdv.nanxuanxn.top

Ruby: s.index("x")
来源：http://koq.zhoulong.xyz

C#:   s.IndexOf("x")
来源：http://tip.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ous.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tdo.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lcr.pycfn.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uib.jlsjyb.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xjn.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tdx.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://asq.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jzy.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nem.zhongyouzk.top

[E06] 替换子串
来源：http://xhv.xuetiantiany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vne.jinyuanbaomall.cn

PHP:  str_replace("a", "b", $s);
来源：http://hrq.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rce.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://cxf.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dkp.iojbl.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://adx.zycfv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bec.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://sgi.zhoulong.xyz

[E07] 按分隔符拆分
来源：http://vqk.redwolf501.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pnk.tarul.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cva.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://swv.daria6918.cn

TS:   s.split(",")
来源：http://ctv.daxiang520.top

Java: s.split(",");  s.split("\\s+")
来源：http://njn.haohaochexian.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ari.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://jlh.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://egu.nanxinkj.top

[E08] 数组按分隔符合并
来源：http://dai.daria6918.cn

Py:   ",".join(items)
来源：http://uhw.iojbl.cn

PHP:  implode(",", $items);
来源：http://mxf.aizwys.cn

JS:   items.join(",")
来源：http://amn.cucudq.cn

TS:   items.join(",")
来源：http://nsx.fktsv.cn

Java: String.join(",", items)
来源：http://lpj.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://ttv.jqgfzy.top

Ruby: items.join(",")
来源：http://hgf.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://uns.redwolf501.top

[E09] 去除所有空白字符
来源：http://cyu.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tju.aizwys.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bar.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://bml.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://ttd.jinghuilouyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://owu.quarkkingdee.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qjs.feifeiyinyue.top

Ruby: s.gsub(/\s+/, "")
来源：http://wqj.mhx1999.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jnz.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://ugd.pycfn.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lcx.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aag.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://wmg.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://fne.sxryk.cn

Java: String.format("%03d", 7)
来源：http://lms.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ddw.jlsjyb.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://owh.cdnleiting.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bwh.yangfankeji.com

[E11] 反转字符串
来源：http://ojf.cdnleiting.top

Py:   s[::-1]
来源：http://kwy.hnxiangtu.top

PHP:  strrev($s);
来源：http://tsb.birdmap.top

JS:   [...s].reverse().join("")
来源：http://qaa.uphjek.com

TS:   [...s].reverse().join("")
来源：http://msn.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ebm.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wex.jinghuilouyu.cn

Ruby: s.reverse
来源：http://hsx.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lcj.jinghuilouyu.cn

[E12] 统计某字符出现次数
来源：http://erc.bbcook.cn

Py:   s.count("a")
来源：http://feb.vehdjk.com

PHP:  substr_count($s, "a");
来源：http://eyv.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://zwu.yuxming.cn

TS:   s.split("a").length - 1
来源：http://nhj.vehdjk.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ckm.yfazqb.com

Go:   strings.Count(s, "a")
来源：http://afv.tarul.cn

Ruby: s.count("a")
来源：http://tkk.pycfn.com

C#:   s.Count(c => c == 'a')
来源：http://qjj.mhx1999.top

[E13] 逐字符遍历
来源：http://ghr.fzhhl.top

Py:   for ch in s: print(ch)
来源：http://lha.haohaochexian.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jgf.zhijiandao.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lum.gzhubu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cpc.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jor.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bju.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://lva.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nbo.gotoacloud.top

[E14] URL 编码与 Base64
来源：http://ppr.quarkkingdee.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qji.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://niu.hywenlv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ihj.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ntn.guowangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://omx.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qqb.hysaishi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rdx.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qxd.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://tri.fktsv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eka.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ita.jyoumei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nma.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://tha.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vch.redwolf501.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ieu.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mbe.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmn.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://qpy.epnwcf.com

Py:   f"{1234567:,}"
来源：http://gdg.ehwqpu.com

PHP:  number_format(1234567);
来源：http://fcg.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sje.hysaishi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yiv.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://guy.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gwp.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ocr.aizwys.cn

C#:   1234567.ToString("N0")
来源：http://xwc.iojbl.cn

[E17] 首字母大写
来源：http://dlb.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zff.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sbj.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hui.bjfxy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gwh.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xkk.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dcs.zdqjudy.top

Ruby: s.capitalize
来源：http://tyo.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qtt.yj20258.top

[E18] 模板占位符替换
来源：http://bxi.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cxf.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mys.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jym.ydjk.org.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wek.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://guu.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fup.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iju.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://exj.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://zyz.guowangkeji.top

Py:   s.splitlines()
来源：http://ktk.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xwn.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://eoe.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://yvj.yvedp.cn

Java: s.lines().toList()
来源：http://eng.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://ilx.guannengcc.top

Ruby: s.lines
来源：http://iut.iojbl.cn

C#:   s.Split('\n')
来源：http://pta.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://qaa.yongpay.top

Py:   if not s:
来源：http://blb.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nwb.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kdu.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://xhu.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://caw.316326.xyz

Go:   if s == "" {}
来源：http://lsw.aizwys.cn

Ruby: if s.empty?
来源：http://jjr.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dmi.sweek.top

[E21] 超长截断加省略号
来源：http://psx.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ksi.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kvb.snrcjt.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izu.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://boa.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://peg.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://cax.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wnq.shanyushiyangtech.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ymb.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://qye.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvj.guannengcc.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uyz.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bui.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zgy.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eon.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhg.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://unf.wangdashe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iah.hongshengwenyu.top

================================================================================
来源：http://kxo.pycfn.com

F. 文件与目录
来源：http://tkv.ctjpmb.com

================================================================================
来源：http://emu.chenlongwang.top

[F01] 读取整个文件
来源：http://jyl.sysykeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://obb.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://iik.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wmm.jinghuilouyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fyl.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bto.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rlh.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://rtd.pycfn.com

C#:   File.ReadAllText("a.txt");
来源：http://fjg.yongpay.top

[F02] 逐行读取文件
来源：http://axr.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yuf.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://spf.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oin.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jhr.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpb.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mtp.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ixn.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pbv.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://rqc.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rgz.zhengqikj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tvr.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rwa.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://khn.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wxm.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wtc.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://ntx.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uqy.0kj1m.cn

[F04] 追加写入文件
来源：http://wqh.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://shi.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pqb.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pud.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tsp.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zia.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gfx.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kgd.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qyn.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://yba.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bhd.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://tbo.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://qcq.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://zlo.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bdo.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://naz.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://qpx.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://jrj.wangshuangyany.cn

[F06] 删除文件
来源：http://foj.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://mzd.epnwcf.com

PHP:  unlink("a.txt");
来源：http://cee.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ofl.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://bxy.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eyv.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://dzu.ctjpmb.com

Ruby: File.delete("a.txt")
来源：http://eox.meibo888.top

C#:   File.Delete("a.txt");
来源：http://gwz.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://zqy.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qxo.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ftw.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhx.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qus.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uzs.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tjh.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ame.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yce.gzhubu.top

[F08] 遍历目录
来源：http://iln.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://tvh.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amt.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://oso.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://gqd.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qdx.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ksn.bjfxy.top

Ruby: Dir.children("dir")
来源：http://ndr.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://twy.hammf.cn

[F09] 获取文件大小
来源：http://wsm.ydjk.org.cn

Py:   os.path.getsize("a.txt")
来源：http://uot.vehdjk.com

PHP:  filesize("a.txt");
来源：http://fqk.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://jxq.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://hja.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uaq.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yjm.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://sfu.quarkkingdee.top

C#:   new FileInfo("a.txt").Length
来源：http://wwz.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://rty.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bhw.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://atx.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jjm.ybcxt.top

TS:   path.extname("a.txt")
来源：http://vcs.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sva.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qne.yueranfly.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xua.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jhi.hongshengwenyu.top

[F11] 复制与移动文件
来源：http://npe.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ftx.sysykeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://png.guannengcc.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wmv.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wch.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sfq.jianghu66.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nec.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kim.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xgc.hesvh.cn

[F12] CSV 读写
来源：http://oev.chenlongwang.top


<!-- 参考信息 -->