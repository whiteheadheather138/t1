代发 wailian999

================================================================================
来源：http://fnp.yuxming.cn

E. 字符串处理
来源：http://qjy.zhixingplan.top

================================================================================
来源：http://rlk.xuetiantiany.cn

[E01] 拼接字符串
来源：http://tll.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ihy.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oic.tian-w.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lwi.hammf.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mcr.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tpi.shuidangran.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cqt.cqqwz.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jak.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ayd.yvedp.cn

[E02] 重复字符串
来源：http://rdm.ctjpmb.com

Py:   "ab" * 3
来源：http://mqn.daxiang520.top

PHP:  str_repeat("ab", 3);
来源：http://dmp.epnwcf.com

JS:   "ab".repeat(3)
来源：http://mrw.wangdashe.top

TS:   "ab".repeat(3)
来源：http://lpp.kuanghao11.cn

Java: "ab".repeat(3)
来源：http://dqa.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://man.wangdashe.top

Ruby: "ab" * 3
来源：http://kmw.yj202588.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://evm.cashguo.top

[E03] 截取子串
来源：http://fnt.nwbrower.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zhf.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://akc.chenlongwang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lwu.bjfxy.top

TS:   s.slice(1, 4)
来源：http://ahn.xingfuxueyuan.xyz

Java: s.substring(1, 4)
来源：http://pmj.ywan-chungtsiang.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hqp.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://tyu.hongshengwenyu.top

C#:   s.Substring(1, 3)
来源：http://zqm.dianchejie.cn

[E04] 查找子串位置
来源：http://zsn.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://obk.vehdjk.com

PHP:  strpos($s, "x");
来源：http://smt.quarkkingdee.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wxp.hywenlv.cn

TS:   s.indexOf("x")
来源：http://bxc.cheryme.top

Java: s.indexOf("x")
来源：http://tos.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://fpv.yanxiufei.cn

Ruby: s.index("x")
来源：http://dyc.sufxvd.cn

C#:   s.IndexOf("x")
来源：http://zkw.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://zrx.ctjpmb.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uzr.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fee.ppjwa.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcx.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zkw.zdbjq.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://miq.zhengqikj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pef.aizwys.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iuh.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fpw.sweek.top

[E06] 替换子串
来源：http://zzj.xuanzx.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gec.zhijiandao.cn

PHP:  str_replace("a", "b", $s);
来源：http://zxn.nwbrower.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ujb.xuetiantiany.cn

TS:   s.replaceAll("a", "b")
来源：http://lkg.chenzaomai.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jrn.jiagoushi.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kqr.gzhubu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uzl.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://btu.fehbvm.com

[E07] 按分隔符拆分
来源：http://slp.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mho.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hkn.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gin.xylfe.cn

TS:   s.split(",")
来源：http://rlg.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://mma.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cmj.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://ptj.nwbrower.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dpo.xuanzx.com

[E08] 数组按分隔符合并
来源：http://utd.hnqzz.top

Py:   ",".join(items)
来源：http://qpt.shangyingyoupin.top

PHP:  implode(",", $items);
来源：http://vyc.xuetiantiany.cn

JS:   items.join(",")
来源：http://vkf.ydzc1.top

TS:   items.join(",")
来源：http://ndv.ydzc1.top

Java: String.join(",", items)
来源：http://cjg.cheryme.top

Go:   strings.Join(items, ",")
来源：http://jec.hesvh.cn

Ruby: items.join(",")
来源：http://zbh.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://ftk.nwbrower.top

[E09] 去除所有空白字符
来源：http://uuv.vehdjk.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zqx.yj202588.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jmd.xingfuxueyuan.xyz

JS:   s.replace(/\s+/g, "")
来源：http://wwf.mhx1999.top

TS:   s.replace(/\s+/g, "")
来源：http://jpq.hfpthk.cn

Java: s.replaceAll("\\s+", "")
来源：http://roi.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://xnl.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://rma.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ydf.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://yqn.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qqj.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iby.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://mfl.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://swc.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://jsr.chenlongwang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://snf.vqdsnc.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://guc.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bqu.yangfankeji.com

[E11] 反转字符串
来源：http://pzw.bjfxy.top

Py:   s[::-1]
来源：http://zvv.jqgufenzy.top

PHP:  strrev($s);
来源：http://gch.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://qns.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://wuf.shuidangran.top

Java: new StringBuilder(s).reverse().toString()
来源：http://hng.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://sbi.hnxiangtu.top

Ruby: s.reverse
来源：http://ptp.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://ynt.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://wtz.shanyushiyangtech.top

Py:   s.count("a")
来源：http://bzo.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://cwb.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://zba.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://lia.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qce.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://cli.havefunace.top

Ruby: s.count("a")
来源：http://pyx.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://ytc.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://qmd.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://jxt.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xfa.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://zay.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bok.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jtt.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://joq.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://icr.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ifj.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://xht.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mrs.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dfj.pycfn.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sbj.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rqq.9152youxi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vud.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tkj.jqgfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mho.gogol.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ydh.wangshuangyany.cn

[E15] HTML 转义 / 反转义
来源：http://hkr.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uol.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://euz.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://opz.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://umj.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aib.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ngg.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://klx.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vna.cheryme.top

[E16] 数字千分位
来源：http://esx.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://hob.bjfxy.top

PHP:  number_format(1234567);
来源：http://sxa.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://hhr.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://tan.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gdy.hcnkem.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jpa.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://drc.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://gle.dashuyun.cn

[E17] 首字母大写
来源：http://xnv.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://krv.nwbrower.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://alv.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://afz.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wxm.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rrx.daxiang520.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lde.zhongyouzk.top

Ruby: s.capitalize
来源：http://kqy.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tym.aizwys.cn

[E18] 模板占位符替换
来源：http://gre.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nzr.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tpz.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mwe.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rvz.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qkw.gogol.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jrb.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://efh.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dfz.cucudq.cn

[E19] 多行文本按行拆分
来源：http://njo.0kj1m.cn

Py:   s.splitlines()
来源：http://jzi.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ytn.chenjidiqi.icu

JS:   s.split(/\r?\n/)
来源：http://gwz.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://tda.chenlongwang.top

Java: s.lines().toList()
来源：http://nwb.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://viz.smart0.xyz

Ruby: s.lines
来源：http://csg.wangshuangyany.cn

C#:   s.Split('\n')
来源：http://qdn.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://ztc.fzhhl.top

Py:   if not s:
来源：http://rrk.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ior.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xau.jinqigfzy.top

TS:   if (s === "") {}
来源：http://gni.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://occ.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://lja.cashguo.top

Ruby: if s.empty?
来源：http://nye.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rzm.birdmap.top

[E21] 超长截断加省略号
来源：http://rik.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fhi.yuxming.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lar.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbr.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mwa.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jab.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://uur.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ula.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmk.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://gxn.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://njs.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gcr.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lom.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nqd.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://puf.hesvh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lle.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://vev.zdbjq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rac.gzhubu.top

================================================================================
来源：http://feg.9152youxi.cn

F. 文件与目录
来源：http://xcn.fengsongda.top

================================================================================
来源：http://wmz.316326.xyz

[F01] 读取整个文件
来源：http://uut.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hem.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://cuo.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ueo.hcnkem.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jde.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yfa.chenjidiqi.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xaw.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://ckt.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://spp.cheryme.top

[F02] 逐行读取文件
来源：http://tnf.hywenlv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ove.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://djj.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxf.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkx.zdqjudy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mtu.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zep.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qss.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bvb.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://dop.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xmr.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://dqv.shanyushiyangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oak.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfr.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bqw.jiagoushi.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fon.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://fhl.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ujd.fehbvm.com

[F04] 追加写入文件
来源：http://vga.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgn.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wxc.zdqjudy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kzu.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ero.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lmr.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uuf.jinqigfzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nax.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qvu.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://aos.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyg.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://eqi.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://uln.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://nbq.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cso.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://epn.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://ins.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://bub.redwolf501.top

[F06] 删除文件
来源：http://zdd.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://nlv.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://vaa.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://oho.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://upk.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lxk.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://anz.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://usx.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://rff.hcnkem.com

[F07] 创建目录（含多级）
来源：http://lun.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mcr.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://otj.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wmv.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbd.chenlongwang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zok.jqgufenzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://moz.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sqw.kuanghao11.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mcd.ybcxt.top

[F08] 遍历目录
来源：http://wak.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://syp.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bts.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://oip.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://wqf.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://heb.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nuu.ybcxt.top

Ruby: Dir.children("dir")
来源：http://frx.nanxuanxn.top

C#:   Directory.GetFiles("dir")
来源：http://fvy.hammf.cn

[F09] 获取文件大小
来源：http://bsi.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://tme.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://nuh.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://dae.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://oek.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://kgf.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dec.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://sxt.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://auu.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://xsh.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://krp.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mgt.cheryme.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tbw.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://bqm.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jtd.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kmx.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wls.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://epv.fzhhl.top

[F11] 复制与移动文件
来源：http://lvz.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gto.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://krp.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ysw.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qen.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ndu.ydzc1.top


<!-- 参考信息 -->