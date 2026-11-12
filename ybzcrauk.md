代发 wailian999

TS:   "ab".repeat(3)
来源：http://vwt.fktsv.cn

Java: "ab".repeat(3)
来源：http://uvp.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://vwz.yj202588.top

Ruby: "ab" * 3
来源：http://smv.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bac.ywan-chungtsiang.top

[E03] 截取子串
来源：http://ckn.bjfxy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://few.kuanghao11.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ywk.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iwz.tarul.cn

TS:   s.slice(1, 4)
来源：http://nsm.haohaochexian.top

Java: s.substring(1, 4)
来源：http://jzs.bjfxy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://apb.cheryme.top

Ruby: s[1, 3];  s[1..3]
来源：http://ibz.shzxlz.cn

C#:   s.Substring(1, 3)
来源：http://obu.uphjek.com

[E04] 查找子串位置
来源：http://hwo.tarul.cn

Py:   s.find("x");  s.index("x")
来源：http://mye.zhijiandao.cn

PHP:  strpos($s, "x");
来源：http://bov.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://arn.yfazqb.com

TS:   s.indexOf("x")
来源：http://vhi.zhoulong.xyz

Java: s.indexOf("x")
来源：http://xtv.jinyuanbaomall.cn

Go:   strings.Index(s, "x")
来源：http://fmz.zhijiandao.cn

Ruby: s.index("x")
来源：http://qjy.nanxinkj.top

C#:   s.IndexOf("x")
来源：http://ijp.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://tub.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iie.sysykeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rls.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://liw.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://qir.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://chs.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://buw.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cic.zycfv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sbq.zhiwuduotai.top

[E06] 替换子串
来源：http://bnd.nanxinkj.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bwb.tanke756.top

PHP:  str_replace("a", "b", $s);
来源：http://fgq.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vzz.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://wii.vehdjk.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rkn.bbcook.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pna.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qte.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://afz.316326.xyz

[E07] 按分隔符拆分
来源：http://ojn.52xcode.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pep.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bfc.gotoacloud.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yzs.zhengqikj.top

TS:   s.split(",")
来源：http://xug.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://mzp.mhx1999.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tuz.epnwcf.com

Ruby: s.split(",");  s.split
来源：http://lwe.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hdb.shuidangran.top

[E08] 数组按分隔符合并
来源：http://gaq.jianghu66.top

Py:   ",".join(items)
来源：http://bso.yonumen.top

PHP:  implode(",", $items);
来源：http://fdp.nwbrower.top

JS:   items.join(",")
来源：http://rnn.tian-w.cn

TS:   items.join(",")
来源：http://qrx.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://hpp.hywenlv.cn

Go:   strings.Join(items, ",")
来源：http://fcq.guannengcc.top

Ruby: items.join(",")
来源：http://rqk.fehbvm.com

C#:   string.Join(",", items)
来源：http://tge.zycfv.cn

[E09] 去除所有空白字符
来源：http://gif.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nsp.ctjpmb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uwn.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://fxh.pengpengdd.cyou

TS:   s.replace(/\s+/g, "")
来源：http://jqu.yvedp.cn

Java: s.replaceAll("\\s+", "")
来源：http://aur.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cei.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://hyf.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ydd.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://gxg.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tej.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qlq.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://dpd.yangfankeji.com

TS:   "7".padStart(3, "0")
来源：http://dbh.smart0.xyz

Java: String.format("%03d", 7)
来源：http://jto.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://krn.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zgk.ehwqpu.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ccy.zhoulong.xyz

[E11] 反转字符串
来源：http://pcq.snrcjt.cn

Py:   s[::-1]
来源：http://zin.jqgfzy.top

PHP:  strrev($s);
来源：http://ula.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://oae.yvedp.cn

TS:   [...s].reverse().join("")
来源：http://ctt.hnxiangtu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zvk.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://coq.zdqjudy.top

Ruby: s.reverse
来源：http://ihw.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://ukt.xylfe.cn

[E12] 统计某字符出现次数
来源：http://ywn.hnxiangtu.top

Py:   s.count("a")
来源：http://gvi.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://bcg.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://ljs.svipenyu.cn

TS:   s.split("a").length - 1
来源：http://yvh.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tnu.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://gsn.xuanzx.com

Ruby: s.count("a")
来源：http://dku.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://vdy.mhx1999.top

[E13] 逐字符遍历
来源：http://sjl.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://uvp.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qae.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://iec.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qyl.hfpthk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bmp.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dlb.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ogv.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mwp.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://ogq.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vty.fzhhl.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lul.ivvv.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lwd.yongpay.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mht.xinyue.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pwf.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvu.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ora.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vpq.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://mgi.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nwr.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tzj.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iiv.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qws.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://the.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hdx.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tez.birdmap.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://swx.pengpengdd.cyou

[E16] 数字千分位
来源：http://wjv.vehdjk.com

Py:   f"{1234567:,}"
来源：http://vev.hcnkem.com

PHP:  number_format(1234567);
来源：http://fdp.yuanzhike.top

JS:   (1234567).toLocaleString("en-US")
来源：http://dok.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gze.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ddn.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://umb.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ive.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://hiw.yfazqb.com

[E17] 首字母大写
来源：http://dsb.yvedp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zdz.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://lxs.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://owe.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qde.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yvd.shanyushiyangtech.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hyh.pengpengdd.cyou

Ruby: s.capitalize
来源：http://mvv.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vli.shanyushiyangkeji.top

[E18] 模板占位符替换
来源：http://mau.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vlj.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qct.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://jqx.hywenlv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ktf.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lln.sweek.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xrr.jinqigufen.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://opt.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qly.ydzc1.top

[E19] 多行文本按行拆分
来源：http://tfk.cdnleiting.top

Py:   s.splitlines()
来源：http://pvy.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vzp.zhijiandao.cn

JS:   s.split(/\r?\n/)
来源：http://hgx.zhoulong.xyz

TS:   s.split(/\r?\n/)
来源：http://tdk.andypj.xyz

Java: s.lines().toList()
来源：http://sua.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://kwr.ivvv.top

Ruby: s.lines
来源：http://mot.dianchejie.cn

C#:   s.Split('\n')
来源：http://faa.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://hvj.nwbrower.top

Py:   if not s:
来源：http://yst.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffx.chenjidiqi.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yns.cheryme.top

TS:   if (s === "") {}
来源：http://box.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://ish.kuanghao11.cn

Go:   if s == "" {}
来源：http://brk.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://siw.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uxq.cdnleiting.top

[E21] 超长截断加省略号
来源：http://xji.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lro.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qfp.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvx.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xza.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ass.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://mcr.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kqr.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sew.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://jku.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mkh.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwx.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aka.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyh.chenzaomai.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hmk.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rrz.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://ovj.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://adp.guowangkeji.top

================================================================================
来源：http://rqc.hcnkem.com

F. 文件与目录
来源：http://hss.fanxiaobao.xyz

================================================================================
来源：http://idb.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://oss.cucudq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ybm.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://hoz.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yzp.chenzaomai.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lzn.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tjt.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kyg.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://phj.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://ymo.chenlongwang.top

[F02] 逐行读取文件
来源：http://omb.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://joe.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vvu.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktc.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xgo.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://elz.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://utn.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nma.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xbt.zdqjudy.top

[F03] 写入文件（覆盖）
来源：http://qmx.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sml.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iga.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rlb.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfl.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://taj.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pwl.yongpay.top

Ruby: File.write("a.txt", "hi")
来源：http://rbt.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohx.zdqjudy.top

[F04] 追加写入文件
来源：http://otv.chenlongwang.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://icl.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hyq.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kme.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulv.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rwx.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zna.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vjw.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hwg.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://wge.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yvd.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://pjj.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://iwa.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://bqt.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xnj.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://odg.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://amv.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://nuy.aibaodan.cn

[F06] 删除文件
来源：http://gui.vqdsnc.cn

Py:   os.remove("a.txt")
来源：http://zmf.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://xxy.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://lav.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lme.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fbk.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://anr.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://gnc.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://nse.guannengcc.top

[F07] 创建目录（含多级）
来源：http://dfb.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cen.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lps.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mst.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jkj.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yrz.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sqd.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tsq.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cmu.ehwqpu.com

[F08] 遍历目录
来源：http://vho.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://snu.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gjl.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://jpt.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://wlj.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ngz.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yzh.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://rxc.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://hle.sufxvd.cn

[F09] 获取文件大小
来源：http://xqx.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://htd.hywenlv.cn

PHP:  filesize("a.txt");
来源：http://lrt.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://gcy.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://ore.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://hyf.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ckn.c1oappe.top

Ruby: File.size("a.txt")
来源：http://gzg.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://tgd.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://obl.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ktz.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kgt.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nvy.guannengcc.top

TS:   path.extname("a.txt")
来源：http://vmw.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rql.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rrk.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://djt.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gae.ydzc1.top

[F11] 复制与移动文件
来源：http://jld.zdbjq.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hpl.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cfn.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://csu.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hzq.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rtv.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kld.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ywf.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vgb.quarkkingdee.top

[F12] CSV 读写
来源：http://lvh.sysykeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bsh.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://brl.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://own.ydjk.org.cn

TS:   // 同上
来源：http://lmp.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tud.redwolf501.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dew.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gcm.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wqu.ywan-chungtsiang.top

================================================================================
来源：http://qmi.xingfuxueyuan.xyz

G. 面向对象
来源：http://hyv.fehbvm.com

================================================================================
来源：http://kcj.zdbjq.cn

[G01] 定义类
来源：http://woo.gogol.net.cn


<!-- 参考信息 -->