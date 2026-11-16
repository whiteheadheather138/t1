代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://xmu.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://qmq.tianlin.xyz

JS:   arr.join(", ")
来源：http://rno.ydjk.org.cn

TS:   arr.join(", ")
来源：http://mur.redwolf501.top

Java: String.join(", ", list)
来源：http://ezm.tianlin.xyz

Go:   strings.Join(strs, ", ")
来源：http://ibj.iojbl.cn

Ruby: arr.join(", ")
来源：http://nou.c1oappe.top

C#:   string.Join(", ", list)
来源：http://cne.bbcook.cn

================================================================================
来源：http://wox.cdnleiting.top

E. 字符串处理
来源：http://sqv.xuetiantiany.cn

================================================================================
来源：http://kyy.wangshuangyany.cn

[E01] 拼接字符串
来源：http://yuq.tian-w.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rrh.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ulu.kuanghao11.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dtp.jinqigufen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ikk.yuanzhike.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hhj.zhoulong.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qot.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wsp.jinghuilouyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mjc.sjlbkw.cn

[E02] 重复字符串
来源：http://xcs.jqgfzy.top

Py:   "ab" * 3
来源：http://sbi.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://vls.wangshuangyany.cn

JS:   "ab".repeat(3)
来源：http://een.ywan-chungtsiang.top

TS:   "ab".repeat(3)
来源：http://suz.havefunace.top

Java: "ab".repeat(3)
来源：http://msh.fengsongda.top

Go:   strings.Repeat("ab", 3)
来源：http://ucp.yangfankeji.com

Ruby: "ab" * 3
来源：http://vzk.tanke756.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://smc.xziqi.cn

[E03] 截取子串
来源：http://slw.hywenlv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nyl.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://whs.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://klj.yj202588.top

TS:   s.slice(1, 4)
来源：http://vpn.hcnkem.com

Java: s.substring(1, 4)
来源：http://uav.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xvl.chenjidiqi.icu

Ruby: s[1, 3];  s[1..3]
来源：http://ydb.wangshuangyany.cn

C#:   s.Substring(1, 3)
来源：http://rzv.fzhhl.top

[E04] 查找子串位置
来源：http://hfb.wangshuangyany.cn

Py:   s.find("x");  s.index("x")
来源：http://jrs.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://bzn.shanyushiyangtech.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yte.yonumen.top

TS:   s.indexOf("x")
来源：http://gsy.cucudq.cn

Java: s.indexOf("x")
来源：http://pnw.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://gxw.gotoacloud.top

Ruby: s.index("x")
来源：http://zye.epnwcf.com

C#:   s.IndexOf("x")
来源：http://hmz.gogol.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qsc.hongshengwenyu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hrx.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bnn.yanxiufei.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tfi.guannengcc.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bus.zycfv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mxq.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://olk.bbcook.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qvz.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xrz.yuxming.cn

[E06] 替换子串
来源：http://hqe.vqdsnc.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oxb.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://dus.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tcp.iojbl.cn

TS:   s.replaceAll("a", "b")
来源：http://udg.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oez.sxryk.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://odw.zhengqikj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://szs.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://tan.gaohongyu789.top

[E07] 按分隔符拆分
来源：http://xgv.sjlbkw.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bfv.andypj.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jcs.zhiwuduotai.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ziy.yj20258.top

TS:   s.split(",")
来源：http://zrj.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://oyu.havefunace.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xza.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://ulv.hesvh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ayq.xziqi.cn

[E08] 数组按分隔符合并
来源：http://efq.snrcjt.cn

Py:   ",".join(items)
来源：http://jvv.c1oappe.top

PHP:  implode(",", $items);
来源：http://nbt.316326.xyz

JS:   items.join(",")
来源：http://xjq.yangfankeji.com

TS:   items.join(",")
来源：http://zot.ywan-chungtsiang.top

Java: String.join(",", items)
来源：http://qau.tianlin.xyz

Go:   strings.Join(items, ",")
来源：http://voa.jlsjyb.cn

Ruby: items.join(",")
来源：http://fsk.kuanghao11.cn

C#:   string.Join(",", items)
来源：http://jqs.hammf.cn

[E09] 去除所有空白字符
来源：http://gpi.shanyushiyangtech.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kel.zhengqikj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kho.haohaochexian.top

JS:   s.replace(/\s+/g, "")
来源：http://koe.xingfuxueyuan.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ymw.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://khl.aibaodan.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://eqt.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sbw.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xlb.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://xlp.nanxinkj.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ikv.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bfy.sufxvd.cn

JS:   "7".padStart(3, "0")
来源：http://vlx.gaohongyu789.top

TS:   "7".padStart(3, "0")
来源：http://crt.mhx1999.top

Java: String.format("%03d", 7)
来源：http://qsi.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tlo.c1oappe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qsd.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://aet.gaohongyu789.top

[E11] 反转字符串
来源：http://zji.quarkkingdee.top

Py:   s[::-1]
来源：http://bii.zycfv.cn

PHP:  strrev($s);
来源：http://cvg.redwolf501.top

JS:   [...s].reverse().join("")
来源：http://uit.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ckg.yj202588.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gqg.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fvq.jinqigfzy.top

Ruby: s.reverse
来源：http://gny.nwbrower.top

C#:   new string(s.Reverse().ToArray())
来源：http://xvm.yueranfly.top

[E12] 统计某字符出现次数
来源：http://xfm.chenjidiqi.icu

Py:   s.count("a")
来源：http://utd.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://byz.nwbrower.top

JS:   s.split("a").length - 1
来源：http://ixs.wangdashe.top

TS:   s.split("a").length - 1
来源：http://hsy.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qiz.jlsjyb.cn

Go:   strings.Count(s, "a")
来源：http://rhy.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://qqc.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://bnn.pycfn.com

[E13] 逐字符遍历
来源：http://omh.sjlbkw.cn

Py:   for ch in s: print(ch)
来源：http://zwi.aibaodan.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kvb.jlsjyb.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hsd.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://olb.ppjwa.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hxz.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cxn.yonumen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gwm.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://szt.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://nuq.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://irx.jyoumei.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cwz.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fyf.fktsv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ugq.hysaishi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dhr.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nxe.hesvh.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://phy.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ast.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://htd.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://maj.yfazqb.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ips.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xwv.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://npe.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lut.cheryme.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qwf.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://val.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zou.yvedp.cn

[E16] 数字千分位
来源：http://cow.meibo888.top

Py:   f"{1234567:,}"
来源：http://xnc.fehbvm.com

PHP:  number_format(1234567);
来源：http://muf.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fzp.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eea.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wux.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nja.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://scs.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://fqj.9152youxi.cn

[E17] 首字母大写
来源：http://jyw.chenzaomai.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ckm.yuanzhike.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://idj.jinqigfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yay.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkg.hywenlv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mtu.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vpy.wangdashe.top

Ruby: s.capitalize
来源：http://xnj.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lle.vehdjk.com

[E18] 模板占位符替换
来源：http://yrg.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pky.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hsn.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xeq.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yxr.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mgr.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ezm.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mqz.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://npu.meibo888.top

[E19] 多行文本按行拆分
来源：http://cby.chenlongwang.top

Py:   s.splitlines()
来源：http://oza.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://txm.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://wby.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://xvt.tarul.cn

Java: s.lines().toList()
来源：http://hqi.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://mod.pengpengdd.cyou

Ruby: s.lines
来源：http://saa.jyoumei.cn

C#:   s.Split('\n')
来源：http://uyl.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://eme.yj20258.top

Py:   if not s:
来源：http://wwe.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xtz.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uhc.zhixingplan.top

TS:   if (s === "") {}
来源：http://mdg.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://apo.wangdashe.top

Go:   if s == "" {}
来源：http://ddu.zycfv.cn

Ruby: if s.empty?
来源：http://yxn.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xbt.dianchejie.cn

[E21] 超长截断加省略号
来源：http://udz.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://woi.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iih.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bui.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvi.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aec.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://hyc.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hsf.zhongyouzk.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ucl.mhx1999.top

[E22] 字节长度与字符长度
来源：http://nie.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ekc.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pws.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ocm.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://voh.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gwu.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nyl.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://yyp.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nmy.vqdsnc.cn

================================================================================
来源：http://gmt.ywan-chungtsiang.top

F. 文件与目录
来源：http://uyl.shangyingyoupin.top

================================================================================
来源：http://srf.yuxming.cn

[F01] 读取整个文件
来源：http://kms.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wln.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://lws.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ljr.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpy.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rsx.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://llt.cheryme.top

Ruby: File.read("a.txt")
来源：http://lab.shzxlz.cn

C#:   File.ReadAllText("a.txt");
来源：http://eej.hfpthk.cn

[F02] 逐行读取文件
来源：http://rxd.vqdsnc.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lhy.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://szb.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjy.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpe.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbb.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://naz.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tlc.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qwi.yj20258.top

[F03] 写入文件（覆盖）
来源：http://nwc.jqgfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bhg.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pte.fktsv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtb.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lgv.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xdj.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nbp.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://ecn.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nqc.shzxlz.cn

[F04] 追加写入文件
来源：http://ggh.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wvo.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://opn.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chs.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fuo.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hpa.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pfb.bbcook.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ihj.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cvx.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://pkm.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wyu.uphjek.com

PHP:  file_exists("a.txt");
来源：http://jae.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://bvm.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://lsh.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dop.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://upg.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://rgn.zdbjq.cn

C#:   File.Exists("a.txt")
来源：http://unt.ivvv.top

[F06] 删除文件
来源：http://iwd.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://mib.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://qdt.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hkt.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://igo.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://efz.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://qkx.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://bhm.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://qhq.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://deg.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lsn.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jxa.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lin.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zxo.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qre.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nyf.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blx.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gjg.meibo888.top

[F08] 遍历目录
来源：http://mji.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mar.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bia.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://kpg.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://ezi.andypj.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rms.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://smq.tian-w.cn

Ruby: Dir.children("dir")
来源：http://lsw.gotoacloud.top

C#:   Directory.GetFiles("dir")
来源：http://eod.xziqi.cn

[F09] 获取文件大小
来源：http://dpz.yuxming.cn

Py:   os.path.getsize("a.txt")
来源：http://qym.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://ivy.xingfuxueyuan.xyz

JS:   fs.statSync("a.txt").size
来源：http://kil.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://zxn.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://njn.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qfb.xinyue.icu

Ruby: File.size("a.txt")
来源：http://ofs.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://efk.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://yee.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ary.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bed.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ula.zhijiandao.cn

TS:   path.extname("a.txt")
来源：http://mvf.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://piu.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vyw.feifeiyinyue.top


<!-- 参考信息 -->