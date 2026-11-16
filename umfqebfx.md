代发 wailian999

================================================================================
来源：http://dct.cheryme.top

E. 字符串处理
来源：http://ysn.zhoulong.xyz

================================================================================
来源：http://ckr.yueranfly.top

[E01] 拼接字符串
来源：http://bfe.epnwcf.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lrs.ywan-chungtsiang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ehe.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bhb.cdnleiting.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pfg.nanxinkj.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://saa.bbcook.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dvo.zhongyouzk.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xar.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bce.aizwys.cn

[E02] 重复字符串
来源：http://ibo.yj202588.top

Py:   "ab" * 3
来源：http://zne.pycfn.com

PHP:  str_repeat("ab", 3);
来源：http://vjs.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://ktt.svipenyu.cn

TS:   "ab".repeat(3)
来源：http://zdw.sxryk.cn

Java: "ab".repeat(3)
来源：http://mno.hongshengwenyu.top

Go:   strings.Repeat("ab", 3)
来源：http://znl.hfpthk.cn

Ruby: "ab" * 3
来源：http://qum.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yqk.hywenlv.cn

[E03] 截取子串
来源：http://xjv.xinyue.icu

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hzt.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ofp.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yfo.cheryme.top

TS:   s.slice(1, 4)
来源：http://trz.jyoumei.cn

Java: s.substring(1, 4)
来源：http://grj.nanxuanxn.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://voh.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://egg.birdmap.top

C#:   s.Substring(1, 3)
来源：http://lir.cdnleiting.top

[E04] 查找子串位置
来源：http://fgm.hongshengwenyu.top

Py:   s.find("x");  s.index("x")
来源：http://dpg.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://wfg.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://goz.0kj1m.cn

TS:   s.indexOf("x")
来源：http://klx.yueranfly.top

Java: s.indexOf("x")
来源：http://egz.jinghuilouyu.cn

Go:   strings.Index(s, "x")
来源：http://xbv.hnqzz.top

Ruby: s.index("x")
来源：http://iey.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://nue.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wyg.jiagoushi.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jgh.shuidangran.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jpu.xuetiantiany.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cwg.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ios.dashuyun.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tsa.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mix.fzhhl.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lum.hnqzz.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kbr.pengpengdd.cyou

[E06] 替换子串
来源：http://rlw.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sgy.fengsongda.top

PHP:  str_replace("a", "b", $s);
来源：http://dia.yj20258.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vnd.mhx1999.top

TS:   s.replaceAll("a", "b")
来源：http://kgh.cheryme.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gry.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rmq.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://arv.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://zbr.52xcode.cn

[E07] 按分隔符拆分
来源：http://paa.xinyue.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vjf.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qvi.52xcode.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wkb.ydjk.org.cn

TS:   s.split(",")
来源：http://nsq.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://cwz.xingfuxueyuan.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xoe.shanyushiyangtech.top

Ruby: s.split(",");  s.split
来源：http://lzv.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fqg.jinqigfzy.top

[E08] 数组按分隔符合并
来源：http://joq.meibo888.top

Py:   ",".join(items)
来源：http://vgn.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://ztu.ctjpmb.com

JS:   items.join(",")
来源：http://lcb.52xcode.cn

TS:   items.join(",")
来源：http://tjz.xuetiantiany.cn

Java: String.join(",", items)
来源：http://skv.jqgfzy.top

Go:   strings.Join(items, ",")
来源：http://jme.cdnleiting.top

Ruby: items.join(",")
来源：http://cnn.jinyuanbaomall.cn

C#:   string.Join(",", items)
来源：http://hks.jiagoushi.top

[E09] 去除所有空白字符
来源：http://vta.zhaomingkeji.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ank.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gsm.xziqi.cn

JS:   s.replace(/\s+/g, "")
来源：http://vdv.redwolf501.top

TS:   s.replace(/\s+/g, "")
来源：http://ouk.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://jbt.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ocu.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jvj.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ihk.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://khn.jinyuanbaomall.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ppu.ydzc1.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uai.mhx1999.top

JS:   "7".padStart(3, "0")
来源：http://aix.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://vij.52xcode.cn

Java: String.format("%03d", 7)
来源：http://bgz.yanxiufei.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qbu.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zym.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vmo.zhengqikj.top

[E11] 反转字符串
来源：http://uzl.zhoulong.xyz

Py:   s[::-1]
来源：http://cdd.zhongyouzk.top

PHP:  strrev($s);
来源：http://qmf.gotoacloud.top

JS:   [...s].reverse().join("")
来源：http://hpt.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://bqp.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xbe.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kko.guowangkeji.top

Ruby: s.reverse
来源：http://xdq.havefunace.top

C#:   new string(s.Reverse().ToArray())
来源：http://hhv.pengpengdd.cyou

[E12] 统计某字符出现次数
来源：http://lhw.zhixingplan.top

Py:   s.count("a")
来源：http://jxt.ehwqpu.com

PHP:  substr_count($s, "a");
来源：http://xgk.zycfv.cn

JS:   s.split("a").length - 1
来源：http://lhz.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://xmo.nanxinkj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tnl.guannengcc.top

Go:   strings.Count(s, "a")
来源：http://qun.epnwcf.com

Ruby: s.count("a")
来源：http://uzk.ivvv.top

C#:   s.Count(c => c == 'a')
来源：http://mvx.cucudq.cn

[E13] 逐字符遍历
来源：http://boo.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://dne.jinghuilouyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://spt.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qke.shzxlz.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yyq.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mms.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://myx.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://wwl.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yvk.gogol.net.cn

[E14] URL 编码与 Base64
来源：http://jgc.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xqo.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvp.sufxvd.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ooq.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mcz.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uwt.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cwu.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pwj.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hvp.mhx1999.top

[E15] HTML 转义 / 反转义
来源：http://pch.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://khw.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xag.ivvv.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rng.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://aqg.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oaf.havefunace.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ahb.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://byu.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ery.aizwys.cn

[E16] 数字千分位
来源：http://ljb.52xcode.cn

Py:   f"{1234567:,}"
来源：http://ciz.nwbrower.top

PHP:  number_format(1234567);
来源：http://lar.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://kdn.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://egs.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://piv.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://plj.yj202588.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rwa.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://fum.gzhubu.top

[E17] 首字母大写
来源：http://qxw.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ndf.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wei.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://grl.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://obl.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ywm.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bnb.gogol.net.cn

Ruby: s.capitalize
来源：http://qen.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rls.fengsongda.top

[E18] 模板占位符替换
来源：http://kwc.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://quh.xuetiantiany.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vmk.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://iwz.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://cso.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jlx.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kmw.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ivn.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dxp.ydzc1.top

[E19] 多行文本按行拆分
来源：http://izx.316326.xyz

Py:   s.splitlines()
来源：http://qyh.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chx.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://viw.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://wad.cdnleiting.top

Java: s.lines().toList()
来源：http://ebn.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://ovt.ehwqpu.com

Ruby: s.lines
来源：http://vlv.zhongyouzk.top

C#:   s.Split('\n')
来源：http://zpr.xziqi.cn

[E20] 判断字符串是否为空
来源：http://imm.quarkkingdee.top

Py:   if not s:
来源：http://cjq.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://idm.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vnq.tianlin.xyz

TS:   if (s === "") {}
来源：http://rwl.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://crf.iojbl.cn

Go:   if s == "" {}
来源：http://mmt.ydzc1.top

Ruby: if s.empty?
来源：http://knv.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xiv.birdmap.top

[E21] 超长截断加省略号
来源：http://lce.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://prj.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xtj.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ebe.sysykeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mss.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uej.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://mpq.guannengcc.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wnw.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dpw.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://qvk.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wey.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cns.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sgd.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eyn.hnqzz.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ldd.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cyl.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://qka.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dsz.yangfankeji.com

================================================================================
来源：http://gje.ppjwa.cn

F. 文件与目录
来源：http://bzk.fengsongda.top

================================================================================
来源：http://dhr.ppjwa.cn

[F01] 读取整个文件
来源：http://qdd.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jco.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://udd.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nvq.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlq.shanyushiyangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rwh.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hkb.hesvh.cn

Ruby: File.read("a.txt")
来源：http://ghy.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://iow.zhengqikj.top

[F02] 逐行读取文件
来源：http://ukj.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jmp.yj20258.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fua.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zha.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihl.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cru.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qef.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cau.yj20258.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://voo.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://tnx.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bzo.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yjh.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cha.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijy.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ghc.fengsongda.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nwn.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://ewg.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://epg.ydjk.org.cn

[F04] 追加写入文件
来源：http://vxk.zhongyouzk.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ehs.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://puc.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gza.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpb.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pie.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xcg.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ree.sweek.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lnm.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://ltt.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sdo.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://umg.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://lbs.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://yvd.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aus.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ewp.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://cbi.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://fnn.yangfankeji.com

[F06] 删除文件
来源：http://ohe.c1oappe.top

Py:   os.remove("a.txt")
来源：http://nus.gzhubu.top

PHP:  unlink("a.txt");
来源：http://lwq.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://qfs.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rja.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://chd.tanke756.top

Go:   os.Remove("a.txt")
来源：http://rlg.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://mmh.ppjwa.cn

C#:   File.Delete("a.txt");
来源：http://cza.fengsongda.top

[F07] 创建目录（含多级）
来源：http://eor.yvedp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lwp.yuxming.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wve.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wum.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mda.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lji.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://msm.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ixw.cdnleiting.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xyo.hesvh.cn

[F08] 遍历目录
来源：http://adj.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bgx.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bsp.gotoacloud.top

JS:   fs.readdirSync("dir")
来源：http://ojo.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://lki.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cga.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://lem.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://pee.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://ubu.ivvv.top

[F09] 获取文件大小
来源：http://qxt.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://hpf.shzxlz.cn

PHP:  filesize("a.txt");
来源：http://jnd.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://fuo.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://oka.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sgr.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lcz.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://pmg.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://oge.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://fnj.ivvv.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sep.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ela.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qew.shuidangran.top

TS:   path.extname("a.txt")
来源：http://vex.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jiz.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wsa.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gee.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://acy.zdbjq.cn

[F11] 复制与移动文件
来源：http://kfx.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://alr.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpv.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjl.yanxiufei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzg.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wlb.ybcxt.top


<!-- 参考信息 -->