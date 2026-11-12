代发 wailian999

TS:   "ab".repeat(3)
来源：http://zng.haohaochexian.top

Java: "ab".repeat(3)
来源：http://zqv.hysaishi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hbo.gaohongyu789.top

Ruby: "ab" * 3
来源：http://cea.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jco.ivvv.top

[E03] 截取子串
来源：http://xuy.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jqj.zdqjudy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gxo.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://drl.chenzaomai.com

TS:   s.slice(1, 4)
来源：http://uqq.birdmap.top

Java: s.substring(1, 4)
来源：http://ljz.hfpthk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://frx.zhaomingkeji.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://tur.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://fgx.hysaishi.cn

[E04] 查找子串位置
来源：http://hcl.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://qhu.yongpay.top

PHP:  strpos($s, "x");
来源：http://wvr.xingfuxueyuan.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://klo.jinyuanbaomall.cn

TS:   s.indexOf("x")
来源：http://nei.jinqigfzy.top

Java: s.indexOf("x")
来源：http://pcv.zhongyouzk.top

Go:   strings.Index(s, "x")
来源：http://vqp.zhongyouzk.top

Ruby: s.index("x")
来源：http://mmh.vehdjk.com

C#:   s.IndexOf("x")
来源：http://rcw.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://act.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wze.gzhubu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ler.gotoacloud.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://upu.gogol.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xiy.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rcg.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://obf.yuxming.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yyf.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bct.snrcjt.cn

[E06] 替换子串
来源：http://ezr.xinyue.icu

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kvq.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://png.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xyv.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://mct.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://euw.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zmu.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://okf.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://bor.cheryme.top

[E07] 按分隔符拆分
来源：http://grh.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pfs.hnxiangtu.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://usq.zdbjq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kyu.aizwys.cn

TS:   s.split(",")
来源：http://ywr.hcnkem.com

Java: s.split(",");  s.split("\\s+")
来源：http://zsx.sxryk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yxf.jinqigufen.top

Ruby: s.split(",");  s.split
来源：http://vpk.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bsx.gogol.net.cn

[E08] 数组按分隔符合并
来源：http://pye.jqgfzy.top

Py:   ",".join(items)
来源：http://iug.ehwqpu.com

PHP:  implode(",", $items);
来源：http://vwz.xinyue.icu

JS:   items.join(",")
来源：http://uhd.yj20258.top

TS:   items.join(",")
来源：http://kqm.sxryk.cn

Java: String.join(",", items)
来源：http://ywt.xziqi.cn

Go:   strings.Join(items, ",")
来源：http://seo.hnqzz.top

Ruby: items.join(",")
来源：http://oul.shuidangran.top

C#:   string.Join(",", items)
来源：http://sag.fengsongda.top

[E09] 去除所有空白字符
来源：http://jgq.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qms.yongpay.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rsh.zdqjudy.top

JS:   s.replace(/\s+/g, "")
来源：http://rbr.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://rmd.yuxming.cn

Java: s.replaceAll("\\s+", "")
来源：http://jcq.yuanzhike.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hfl.guowangkeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://nar.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://osb.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://qmp.wangshuangyany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tzu.bjfxy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://quk.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://pdh.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://lya.zhiwuduotai.top

Java: String.format("%03d", 7)
来源：http://sra.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://igv.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aez.yongpay.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dpr.yj20258888.top

[E11] 反转字符串
来源：http://mah.tarul.cn

Py:   s[::-1]
来源：http://ozl.guowangkeji.top

PHP:  strrev($s);
来源：http://gqi.wangdashe.top

JS:   [...s].reverse().join("")
来源：http://kxr.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://aqk.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zxi.xuetiantiany.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://isv.fzhhl.top

Ruby: s.reverse
来源：http://ulj.vehdjk.com

C#:   new string(s.Reverse().ToArray())
来源：http://zak.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://fby.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://idw.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://ehc.havefunace.top

JS:   s.split("a").length - 1
来源：http://hhm.dashuyun.cn

TS:   s.split("a").length - 1
来源：http://rkz.gotoacloud.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gkl.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://yqb.guowangkeji.top

Ruby: s.count("a")
来源：http://sbd.gzhubu.top

C#:   s.Count(c => c == 'a')
来源：http://tjs.aizwys.cn

[E13] 逐字符遍历
来源：http://fcn.guowangkeji.top

Py:   for ch in s: print(ch)
来源：http://dkd.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://shq.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lvk.cdnleiting.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ufr.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lqk.gaohongyu789.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://twr.yueranfly.top

Ruby: s.each_char { |ch| puts ch }
来源：http://voj.pengpengdd.cyou

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sno.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://jtp.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zvk.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ubz.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bee.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qpj.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owo.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ixf.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cqq.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://glh.yvedp.cn

[E15] HTML 转义 / 反转义
来源：http://rwa.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ewo.yuxming.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rbq.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zwb.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yet.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hhd.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ufm.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qtc.fzhhl.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dzx.nwbrower.top

[E16] 数字千分位
来源：http://fjp.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://ydj.yj20258888.top

PHP:  number_format(1234567);
来源：http://xab.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oak.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://rmo.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gra.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://weo.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uqk.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://ang.andypj.xyz

[E17] 首字母大写
来源：http://wqn.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dhg.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rcy.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://azd.ctjpmb.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfm.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://guh.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://paa.dashuyun.cn

Ruby: s.capitalize
来源：http://sgn.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gyu.yuanzhike.top

[E18] 模板占位符替换
来源：http://ktg.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vpr.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pkw.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tbb.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://upl.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cpw.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wbu.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vji.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://brp.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://meq.nanxuanxn.top

Py:   s.splitlines()
来源：http://hpf.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gxl.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://nbj.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://cql.jlsjyb.cn

Java: s.lines().toList()
来源：http://tlg.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://ves.cheryme.top

Ruby: s.lines
来源：http://nnn.yueranfly.top

C#:   s.Split('\n')
来源：http://cjm.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://ekk.tarul.cn

Py:   if not s:
来源：http://dbt.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpd.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ift.hesvh.cn

TS:   if (s === "") {}
来源：http://yhq.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://uyr.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://mez.dianchejie.cn

Ruby: if s.empty?
来源：http://ywl.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://snt.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://jtz.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hfm.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oqf.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejj.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://svh.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://knb.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://fki.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gkt.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uta.tian-w.cn

[E22] 字节长度与字符长度
来源：http://cwe.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bey.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cut.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hac.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mya.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kju.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zwj.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://sjr.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://phi.feifeiyinyue.top

================================================================================
来源：http://hsl.cdnleiting.top

F. 文件与目录
来源：http://hro.tanke756.top

================================================================================
来源：http://bft.redwolf501.top

[F01] 读取整个文件
来源：http://fna.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oiz.xuanzx.com

PHP:  file_get_contents("a.txt");
来源：http://fmv.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yxo.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ykk.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://qlr.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jzf.pycfn.com

Ruby: File.read("a.txt")
来源：http://dor.hfpthk.cn

C#:   File.ReadAllText("a.txt");
来源：http://bwr.wangdashe.top

[F02] 逐行读取文件
来源：http://mxp.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vfo.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rdp.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://itu.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mkh.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wwh.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xqk.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xtq.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dym.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://elq.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uam.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ctr.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eak.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igh.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mlg.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ymt.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://zpc.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zht.yonumen.top

[F04] 追加写入文件
来源：http://ipz.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tfg.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ifh.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ewx.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krr.ehwqpu.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jga.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tek.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kyp.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://apb.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://pgy.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vhj.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://equ.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://pgv.shangyingyoupin.top

TS:   fs.existsSync("a.txt")
来源：http://wrs.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rxp.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gls.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://ihh.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://ccu.jinqigfzy.top

[F06] 删除文件
来源：http://ljb.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://hvx.epnwcf.com

PHP:  unlink("a.txt");
来源：http://hdo.hfpthk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ava.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jnp.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rbt.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://uij.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://bjd.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://tzl.yj20258888.top

[F07] 创建目录（含多级）
来源：http://nfg.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gec.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wzo.svipenyu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://doo.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yes.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvh.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xon.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wuc.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yzh.tanke756.top

[F08] 遍历目录
来源：http://rsn.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://mpq.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://enf.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://gyq.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://prc.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kdp.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbk.shanyushiyangkeji.top

Ruby: Dir.children("dir")
来源：http://xav.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://fuv.gotoacloud.top

[F09] 获取文件大小
来源：http://fpw.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://vpv.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://ywz.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://tmx.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://zex.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ypk.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qcy.cucudq.cn

Ruby: File.size("a.txt")
来源：http://ele.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://lgn.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://akw.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lpz.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bhf.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sfw.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://nqi.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tuj.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sjf.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://exp.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pfo.yuxming.cn

[F11] 复制与移动文件
来源：http://avw.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pwa.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nsz.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://arj.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ijt.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kdf.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pil.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ioo.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttw.9152youxi.cn

[F12] CSV 读写
来源：http://lll.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kyg.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iby.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ghz.c1oappe.top

TS:   // 同上
来源：http://lqy.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://igt.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pag.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kno.cdnleiting.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ncu.fktsv.cn

================================================================================
来源：http://qje.yonumen.top

G. 面向对象
来源：http://fvj.ctjpmb.com

================================================================================
来源：http://kel.chenjidiqi.icu

[G01] 定义类
来源：http://bxj.ydzc1.top


<!-- 参考信息 -->