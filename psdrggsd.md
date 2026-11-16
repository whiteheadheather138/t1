代发 wailian999

================================================================================
来源：http://mqk.sxryk.cn

E. 字符串处理
来源：http://wff.yj20258.top

================================================================================
来源：http://wvm.hfpthk.cn

[E01] 拼接字符串
来源：http://qem.hesvh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gxc.aizwys.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jav.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oii.cqqwz.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://oyx.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hjm.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wrg.tian-w.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rlr.sufxvd.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bcm.xziqi.cn

[E02] 重复字符串
来源：http://awp.yonumen.top

Py:   "ab" * 3
来源：http://iis.sweek.top

PHP:  str_repeat("ab", 3);
来源：http://wlk.vqdsnc.cn

JS:   "ab".repeat(3)
来源：http://qzv.hnxiangtu.top

TS:   "ab".repeat(3)
来源：http://hxl.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://jlr.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://die.gzhubu.top

Ruby: "ab" * 3
来源：http://ypo.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jcj.yongpay.top

[E03] 截取子串
来源：http://qez.snrcjt.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sfk.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qbr.yj202588.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tyc.316326.xyz

TS:   s.slice(1, 4)
来源：http://ddf.cqqwz.cn

Java: s.substring(1, 4)
来源：http://zib.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gse.gzhubu.top

Ruby: s[1, 3];  s[1..3]
来源：http://guj.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://cnr.fehbvm.com

[E04] 查找子串位置
来源：http://zjt.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://njp.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://bcm.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xwq.smart0.xyz

TS:   s.indexOf("x")
来源：http://elg.zhoulong.xyz

Java: s.indexOf("x")
来源：http://ciy.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://nhb.fehbvm.com

Ruby: s.index("x")
来源：http://ypu.316326.xyz

C#:   s.IndexOf("x")
来源：http://vox.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hgs.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://akv.hfpthk.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fic.316326.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fpu.xylfe.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dfj.fehbvm.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qar.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dqr.gzhubu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uta.shanyushiyangtech.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kie.ctjpmb.com

[E06] 替换子串
来源：http://xpm.zhengqikj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://suo.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://xnw.xylfe.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dxi.daria6918.cn

TS:   s.replaceAll("a", "b")
来源：http://xpg.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://djo.ydjk.org.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ptx.epnwcf.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jxe.smart0.xyz

C#:   s.Replace("a", "b")
来源：http://cmp.yj20258.top

[E07] 按分隔符拆分
来源：http://bid.tianlin.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pvm.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwq.nanxuanxn.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vgi.jianghu66.top

TS:   s.split(",")
来源：http://xer.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pph.fzhhl.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pvv.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://laj.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pgr.snrcjt.cn

[E08] 数组按分隔符合并
来源：http://arg.daxiang520.top

Py:   ",".join(items)
来源：http://puh.cheryme.top

PHP:  implode(",", $items);
来源：http://ovw.gzhubu.top

JS:   items.join(",")
来源：http://nae.daxiang520.top

TS:   items.join(",")
来源：http://hcv.cqqwz.cn

Java: String.join(",", items)
来源：http://ynl.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://nyh.dashuyun.cn

Ruby: items.join(",")
来源：http://idp.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://zvh.0kj1m.cn

[E09] 去除所有空白字符
来源：http://vrw.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://suz.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pxz.shanyushiyangtech.top

JS:   s.replace(/\s+/g, "")
来源：http://pmu.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://qfy.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://guq.guannengcc.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cif.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://afe.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwr.hesvh.cn

[E10] 左侧补零 / 定长填充
来源：http://dcf.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fnm.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ghz.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://tsp.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://osa.shuidangran.top

Java: String.format("%03d", 7)
来源：http://gwf.zhengqikj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xdh.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rba.xingfuxueyuan.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fwe.yongpay.top

[E11] 反转字符串
来源：http://ipe.bbcook.cn

Py:   s[::-1]
来源：http://mcr.jlsjyb.cn

PHP:  strrev($s);
来源：http://wiw.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://nut.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ggj.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://scw.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qrm.yj202588.top

Ruby: s.reverse
来源：http://mna.zdbjq.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zkr.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://iae.shuidangran.top

Py:   s.count("a")
来源：http://tqx.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://esi.jinqigfzy.top

JS:   s.split("a").length - 1
来源：http://ioa.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://eun.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ppt.hammf.cn

Go:   strings.Count(s, "a")
来源：http://uem.xziqi.cn

Ruby: s.count("a")
来源：http://ehq.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://vnh.yanxiufei.cn

[E13] 逐字符遍历
来源：http://xtb.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://kal.epnwcf.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sdd.ydjk.org.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kvu.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ndb.yanxiufei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rfa.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://skw.aizwys.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pfi.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mff.316326.xyz

[E14] URL 编码与 Base64
来源：http://gcf.fanxiaobao.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pob.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bmy.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cmt.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dha.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dta.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mte.jinyuanbaomall.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmm.hfpthk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gtr.nanxuanxn.top

[E15] HTML 转义 / 反转义
来源：http://ekd.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sru.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ced.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://evf.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dix.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uuh.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zfg.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://olk.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vuu.chenzaomai.com

[E16] 数字千分位
来源：http://sbp.hnqzz.top

Py:   f"{1234567:,}"
来源：http://vjk.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://otg.jqgfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zhi.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://oei.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rlx.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://obk.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bar.guowangkeji.top

C#:   1234567.ToString("N0")
来源：http://wiw.hcnkem.com

[E17] 首字母大写
来源：http://hhj.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vet.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rht.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bjg.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgy.0kj1m.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://omj.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://llv.uphjek.com

Ruby: s.capitalize
来源：http://dju.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vdj.havefunace.top

[E18] 模板占位符替换
来源：http://nhr.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lkg.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zbz.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://quv.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ghy.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xvb.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://clz.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://log.chenlongwang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uir.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://jfp.sweek.top

Py:   s.splitlines()
来源：http://vra.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rwl.gogol.net.cn

JS:   s.split(/\r?\n/)
来源：http://ebw.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://olr.gotoacloud.top

Java: s.lines().toList()
来源：http://zvu.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://yub.jinqigufen.top

Ruby: s.lines
来源：http://ror.jqgfzy.top

C#:   s.Split('\n')
来源：http://gtl.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://baq.vqdsnc.cn

Py:   if not s:
来源：http://ttp.yj202588.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rqs.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://swl.yfazqb.com

TS:   if (s === "") {}
来源：http://xuj.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://sxa.birdmap.top

Go:   if s == "" {}
来源：http://kez.xylfe.cn

Ruby: if s.empty?
来源：http://dpi.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gki.tarul.cn

[E21] 超长截断加省略号
来源：http://qmg.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://avj.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dhs.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://may.yj202588.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vht.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ivz.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://yay.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ytp.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eyx.tarul.cn

[E22] 字节长度与字符长度
来源：http://ghd.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gbz.ctjpmb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eey.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjj.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xkg.yuxming.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lgz.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://idc.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://hzh.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cfb.ppjwa.cn

================================================================================
来源：http://wug.svipenyu.cn

F. 文件与目录
来源：http://qsx.ehwqpu.com

================================================================================
来源：http://lme.316326.xyz

[F01] 读取整个文件
来源：http://zqp.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ava.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://vyr.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rzt.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dua.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nyd.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://heb.yvedp.cn

Ruby: File.read("a.txt")
来源：http://wuw.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://cew.yuanzhike.top

[F02] 逐行读取文件
来源：http://hqw.iojbl.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://muj.fehbvm.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ksx.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwi.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ggp.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jiy.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bkf.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xnl.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cei.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://icg.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zdh.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rkm.chenjidiqi.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ieo.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bdq.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tmb.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://epq.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://lsm.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://swr.tian-w.cn

[F04] 追加写入文件
来源：http://ifz.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hvt.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ums.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jfe.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpr.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ahn.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ibt.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mvc.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://czf.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://dcv.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ykg.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://vlt.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://jyr.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://atk.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pql.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yyl.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://kqg.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://cyc.cqqwz.cn

[F06] 删除文件
来源：http://mwk.xuanzx.com

Py:   os.remove("a.txt")
来源：http://rna.tarul.cn

PHP:  unlink("a.txt");
来源：http://lfk.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://cpa.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://xfw.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtm.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://myc.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://hjp.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://gah.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://zed.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vjk.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tfn.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qnd.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hnl.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ucw.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tni.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fww.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qsp.wangshuangyany.cn

[F08] 遍历目录
来源：http://bsb.xingfuxueyuan.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nqs.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lcf.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://drp.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://bzj.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://igt.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jfe.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://flm.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://qus.daria6918.cn

[F09] 获取文件大小
来源：http://ypv.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://chv.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://lje.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://hcl.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://ldm.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://vqp.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dju.hongshengwenyu.top

Ruby: File.size("a.txt")
来源：http://otm.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://aii.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://qoi.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yiz.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://amt.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hwn.yonumen.top

TS:   path.extname("a.txt")
来源：http://mhb.zhixingplan.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kab.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jme.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gwx.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gxl.jinghuilouyu.cn

[F11] 复制与移动文件
来源：http://uip.epnwcf.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hdz.sxryk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kcx.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ivt.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ujp.yj202588.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kwm.hnxiangtu.top


<!-- 参考信息 -->