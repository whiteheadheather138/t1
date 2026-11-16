代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ymc.tian-w.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ern.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mjx.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kax.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mbq.zdbjq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wam.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gyp.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ubu.cheryme.top

[E02] 重复字符串
来源：http://opx.gaohongyu789.top

Py:   "ab" * 3
来源：http://ovv.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://iqc.jinqigufen.top

JS:   "ab".repeat(3)
来源：http://kih.cdnleiting.top

TS:   "ab".repeat(3)
来源：http://zxt.xziqi.cn

Java: "ab".repeat(3)
来源：http://pxu.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://mlg.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://jwr.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://cgr.yfazqb.com

[E03] 截取子串
来源：http://gtc.haohaochexian.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rgw.yangfankeji.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iil.zdbjq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hku.zhiwuduotai.top

TS:   s.slice(1, 4)
来源：http://xfm.jqgfzy.top

Java: s.substring(1, 4)
来源：http://xox.hongshengwenyu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ngg.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://hwr.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://kbo.vehdjk.com

[E04] 查找子串位置
来源：http://ogu.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://sgq.jqgufenzy.top

PHP:  strpos($s, "x");
来源：http://mmq.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xhb.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://ath.chenlongwang.top

Java: s.indexOf("x")
来源：http://oto.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://fot.zycfv.cn

Ruby: s.index("x")
来源：http://rqe.yonumen.top

C#:   s.IndexOf("x")
来源：http://fqg.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://joh.hammf.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xjb.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tfw.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkk.havefunace.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://udt.gotoacloud.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxj.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dbj.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jvf.yangfankeji.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://khm.shanyushiyangtech.top

[E06] 替换子串
来源：http://pkm.c1oappe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vpp.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://tlk.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uui.jlsjyb.cn

TS:   s.replaceAll("a", "b")
来源：http://czo.xinyue.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pvx.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://myy.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gai.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://fhj.aizwys.cn

[E07] 按分隔符拆分
来源：http://gji.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ixn.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rkw.jinyuanbaomall.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bqd.svipenyu.cn

TS:   s.split(",")
来源：http://wfc.aibaodan.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tjw.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lbx.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://qfl.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://usn.ydzc1.top

[E08] 数组按分隔符合并
来源：http://cnw.c1oappe.top

Py:   ",".join(items)
来源：http://inn.sufxvd.cn

PHP:  implode(",", $items);
来源：http://urc.ppjwa.cn

JS:   items.join(",")
来源：http://vfs.ivvv.top

TS:   items.join(",")
来源：http://xti.ehwqpu.com

Java: String.join(",", items)
来源：http://iwy.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://seq.c1oappe.top

Ruby: items.join(",")
来源：http://drh.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://fil.ctjpmb.com

[E09] 去除所有空白字符
来源：http://drp.nanxuanxn.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gah.yueranfly.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ogd.fzhhl.top

JS:   s.replace(/\s+/g, "")
来源：http://kqr.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://gqh.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://ldn.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ysh.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://imt.zhengqikj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aln.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://ips.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sou.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://sgx.wangdashe.top

JS:   "7".padStart(3, "0")
来源：http://yyk.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://egq.jqgufenzy.top

Java: String.format("%03d", 7)
来源：http://nud.tianlin.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://ufj.xinyue.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cjk.tanke756.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qqd.meibo888.top

[E11] 反转字符串
来源：http://iou.gzhubu.top

Py:   s[::-1]
来源：http://hoh.jqgufenzy.top

PHP:  strrev($s);
来源：http://fvw.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://lhj.yonumen.top

TS:   [...s].reverse().join("")
来源：http://ytp.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fzu.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aej.gzhubu.top

Ruby: s.reverse
来源：http://izv.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://xtu.chenlongwang.top

[E12] 统计某字符出现次数
来源：http://tdq.zhengqikj.top

Py:   s.count("a")
来源：http://tpp.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://dgz.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://bwd.yj202588.top

TS:   s.split("a").length - 1
来源：http://xgi.guowangkeji.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qpy.hywenlv.cn

Go:   strings.Count(s, "a")
来源：http://qav.yanxiufei.cn

Ruby: s.count("a")
来源：http://wrc.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://pzp.pycfn.com

[E13] 逐字符遍历
来源：http://dgx.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://ejq.yuxming.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tkk.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wmt.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pyn.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vbe.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ylu.bbcook.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pez.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qoc.gzhubu.top

[E14] URL 编码与 Base64
来源：http://eyg.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://avo.jlsjyb.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://imt.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gyj.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dhl.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lvu.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vyc.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vjt.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jbn.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://int.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://qtv.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yli.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xjo.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://whh.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uwn.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yad.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://odx.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wnk.cheryme.top

[E16] 数字千分位
来源：http://ftl.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://jkv.svipenyu.cn

PHP:  number_format(1234567);
来源：http://vcx.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nrx.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ney.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jud.jinghuilouyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eto.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vnz.316326.xyz

C#:   1234567.ToString("N0")
来源：http://uyq.yonumen.top

[E17] 首字母大写
来源：http://rft.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sbq.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fgp.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wwa.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uvk.yfazqb.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://egv.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rww.zhijiandao.cn

Ruby: s.capitalize
来源：http://yyf.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zbu.hysaishi.cn

[E18] 模板占位符替换
来源：http://yaw.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bus.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gww.ctjpmb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://xqu.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jvg.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gwm.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gcn.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mth.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pwt.xziqi.cn

[E19] 多行文本按行拆分
来源：http://juc.hywenlv.cn

Py:   s.splitlines()
来源：http://dpu.shanyushiyangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dpz.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://vzb.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://mhf.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://gms.yonumen.top

Go:   strings.Split(s, "\n")
来源：http://xoa.xylfe.cn

Ruby: s.lines
来源：http://vpi.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://pco.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://dbd.jianghu66.top

Py:   if not s:
来源：http://onx.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lnz.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cnz.quarkkingdee.top

TS:   if (s === "") {}
来源：http://qsk.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://vhh.cheryme.top

Go:   if s == "" {}
来源：http://rdz.zdqjudy.top

Ruby: if s.empty?
来源：http://lfb.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ogx.cheryme.top

[E21] 超长截断加省略号
来源：http://cgg.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gzg.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gvi.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzv.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzi.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ahk.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://ldm.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oto.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tfd.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://mof.hnxiangtu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wxp.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ogl.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmn.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://shh.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://euc.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://knc.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://nxo.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hub.fanxiaobao.xyz

================================================================================
来源：http://pab.tanke756.top

F. 文件与目录
来源：http://qqw.fengsongda.top

================================================================================
来源：http://fhx.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://ooq.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gfp.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://lnh.sxryk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bbx.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://afz.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rtt.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vnr.wangdashe.top

Ruby: File.read("a.txt")
来源：http://avo.jiagoushi.top

C#:   File.ReadAllText("a.txt");
来源：http://pxd.bbcook.cn

[F02] 逐行读取文件
来源：http://laa.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pye.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mfv.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uok.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ubi.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yda.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ltn.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jlu.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bof.cashguo.top

[F03] 写入文件（覆盖）
来源：http://cne.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rit.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jjx.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hgh.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zjp.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xva.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ncy.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://owo.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bdx.gogol.net.cn

[F04] 追加写入文件
来源：http://oml.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fnr.zycfv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://etu.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qiy.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyw.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zvu.yonumen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mon.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ynq.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kei.ppjwa.cn

[F05] 判断文件或目录是否存在
来源：http://fcz.aizwys.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tai.wangdashe.top

PHP:  file_exists("a.txt");
来源：http://qzu.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://tab.zhaomingkeji.xyz

TS:   fs.existsSync("a.txt")
来源：http://fbi.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yun.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zui.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://mcy.uphjek.com

C#:   File.Exists("a.txt")
来源：http://uxa.wangdashe.top

[F06] 删除文件
来源：http://jwo.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://hpc.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://gpb.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://ovs.shanyushiyangtech.top

TS:   fs.unlinkSync("a.txt")
来源：http://mqp.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vxn.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://dqg.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://ufv.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://epo.yfazqb.com

[F07] 创建目录（含多级）
来源：http://wve.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qel.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nob.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhz.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mlr.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://avv.hcnkem.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rsk.316326.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nme.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dem.sxryk.cn

[F08] 遍历目录
来源：http://eun.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://unn.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://odx.yj20258.top

JS:   fs.readdirSync("dir")
来源：http://ehs.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://yxl.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fco.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pdt.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://ukk.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://prd.yueranfly.top

[F09] 获取文件大小
来源：http://qro.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://pam.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://spw.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://dzc.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://hmg.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ptb.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vrg.zdqjudy.top

Ruby: File.size("a.txt")
来源：http://hap.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://jwr.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://axt.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qnf.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://loo.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zvh.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://gsu.fzhhl.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zzr.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mbg.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pxm.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://csf.haohaochexian.top

[F11] 复制与移动文件
来源：http://uio.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wfq.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tzn.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ydr.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://njp.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnk.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zvl.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://itq.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vjs.chenlongwang.top

[F12] CSV 读写
来源：http://sdc.hfpthk.cn


<!-- 参考信息 -->