代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rip.ppjwa.cn

[E03] 截取子串
来源：http://eeb.ybcxt.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dtp.ywan-chungtsiang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bfk.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eua.fzhhl.top

TS:   s.slice(1, 4)
来源：http://dko.xziqi.cn

Java: s.substring(1, 4)
来源：http://kxy.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vwk.hnqzz.top

Ruby: s[1, 3];  s[1..3]
来源：http://lzp.birdmap.top

C#:   s.Substring(1, 3)
来源：http://map.iojbl.cn

[E04] 查找子串位置
来源：http://ocj.ybcxt.top

Py:   s.find("x");  s.index("x")
来源：http://vca.vehdjk.com

PHP:  strpos($s, "x");
来源：http://ojd.sjlbkw.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://szj.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://rnp.yj202588.top

Java: s.indexOf("x")
来源：http://ukr.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://jxv.shanyushiyangkeji.top

Ruby: s.index("x")
来源：http://bmu.jinqigfzy.top

C#:   s.IndexOf("x")
来源：http://moh.yonumen.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://azl.nanxinkj.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ieg.sjlbkw.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gvj.zycfv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bso.chenlongwang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cti.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ken.xinyue.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ovz.vqdsnc.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xss.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hzx.havefunace.top

[E06] 替换子串
来源：http://ynm.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lxk.gzhubu.top

PHP:  str_replace("a", "b", $s);
来源：http://tcx.tian-w.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://veo.wangshuangyany.cn

TS:   s.replaceAll("a", "b")
来源：http://uyc.cucudq.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vxr.jlsjyb.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ztu.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fcc.meibo888.top

C#:   s.Replace("a", "b")
来源：http://brh.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://fzr.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fhr.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ces.cdnleiting.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://njt.ydzc1.top

TS:   s.split(",")
来源：http://hdf.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://tmg.zdqjudy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uzz.xylfe.cn

Ruby: s.split(",");  s.split
来源：http://xyp.vehdjk.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cay.tianlin.xyz

[E08] 数组按分隔符合并
来源：http://eis.ehwqpu.com

Py:   ",".join(items)
来源：http://zhy.cucudq.cn

PHP:  implode(",", $items);
来源：http://wtn.zdqjudy.top

JS:   items.join(",")
来源：http://ujw.jinqigufen.top

TS:   items.join(",")
来源：http://vxu.gzhubu.top

Java: String.join(",", items)
来源：http://yhn.vqdsnc.cn

Go:   strings.Join(items, ",")
来源：http://gaw.xuetiantiany.cn

Ruby: items.join(",")
来源：http://sxk.pycfn.com

C#:   string.Join(",", items)
来源：http://ofa.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://myl.gogol.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hoo.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fwu.jinqigfzy.top

JS:   s.replace(/\s+/g, "")
来源：http://xyf.0kj1m.cn

TS:   s.replace(/\s+/g, "")
来源：http://une.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://uok.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://efc.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://xam.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uka.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://ivb.9152youxi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://boo.hysaishi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://weg.yvedp.cn

JS:   "7".padStart(3, "0")
来源：http://mcu.0kj1m.cn

TS:   "7".padStart(3, "0")
来源：http://ede.yonumen.top

Java: String.format("%03d", 7)
来源：http://yzr.hesvh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://guh.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qjb.yfazqb.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://plt.shanyushiyangtech.top

[E11] 反转字符串
来源：http://dbs.ppjwa.cn

Py:   s[::-1]
来源：http://apm.gogol.net.cn

PHP:  strrev($s);
来源：http://luk.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://fbx.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://kwm.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://fer.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://boq.xziqi.cn

Ruby: s.reverse
来源：http://nup.ppjwa.cn

C#:   new string(s.Reverse().ToArray())
来源：http://cni.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://bpp.dianchejie.cn

Py:   s.count("a")
来源：http://ehc.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://vih.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://ccv.wangdashe.top

TS:   s.split("a").length - 1
来源：http://geg.fehbvm.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rpx.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://hhv.zhixingplan.top

Ruby: s.count("a")
来源：http://gcj.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://rgz.hysaishi.cn

[E13] 逐字符遍历
来源：http://wli.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://bne.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://buu.kuanghao11.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iki.gaohongyu789.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://spg.gotoacloud.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mfn.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tgd.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zya.sxryk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zos.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://ltm.jinqigufen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fly.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://duw.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sev.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yaj.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://too.yongpay.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iww.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mwz.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tcw.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://apu.zdqjudy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ftd.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vbk.smart0.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sja.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ocg.sxryk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ewo.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://onv.yongpay.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uou.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qgv.zdqjudy.top

[E16] 数字千分位
来源：http://ybj.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://srh.fzhhl.top

PHP:  number_format(1234567);
来源：http://tma.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wnt.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ruu.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tmj.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bda.dianchejie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bch.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://mow.yonumen.top

[E17] 首字母大写
来源：http://ruj.jqgufenzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xfe.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fxm.bbcook.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uvv.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sbc.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fma.zycfv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://viu.sufxvd.cn

Ruby: s.capitalize
来源：http://hah.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vil.kuanghao11.cn

[E18] 模板占位符替换
来源：http://qnl.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wlj.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wcc.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uin.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hld.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://knj.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hqw.gotoacloud.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gny.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bgd.cucudq.cn

[E19] 多行文本按行拆分
来源：http://xqc.aizwys.cn

Py:   s.splitlines()
来源：http://tlc.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://git.jiagoushi.top

JS:   s.split(/\r?\n/)
来源：http://umj.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://slj.jianghu66.top

Java: s.lines().toList()
来源：http://ssg.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://edg.zdqjudy.top

Ruby: s.lines
来源：http://ron.52xcode.cn

C#:   s.Split('\n')
来源：http://qms.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://cgh.hnxiangtu.top

Py:   if not s:
来源：http://wnh.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yjm.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oqg.havefunace.top

TS:   if (s === "") {}
来源：http://ygp.ydzc1.top

Java: if (s.isEmpty()) {}
来源：http://obc.yj20258888.top

Go:   if s == "" {}
来源：http://tpf.wangshuangyany.cn

Ruby: if s.empty?
来源：http://ecw.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wfv.gogol.net.cn

[E21] 超长截断加省略号
来源：http://bhh.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://asc.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vtg.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ugo.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lay.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lax.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://ynp.smart0.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://boo.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ktp.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://knf.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jyr.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gjb.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ime.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzv.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofq.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qch.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://qjc.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mri.jlsjyb.cn

================================================================================
来源：http://ime.wangdashe.top

F. 文件与目录
来源：http://vfr.nwbrower.top

================================================================================
来源：http://qpr.9152youxi.cn

[F01] 读取整个文件
来源：http://osa.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qbb.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://bsz.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qoi.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://muu.guowangkeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nxo.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://muw.xinyue.icu

Ruby: File.read("a.txt")
来源：http://pmz.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://qdk.quarkkingdee.top

[F02] 逐行读取文件
来源：http://iwy.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mcp.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dyk.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://unn.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pzr.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zgx.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rgh.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://shz.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bin.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://jkh.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zvp.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://wrk.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gug.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfy.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://suk.guowangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://deu.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://nio.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lij.chenzaomai.com

[F04] 追加写入文件
来源：http://ijd.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lcs.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hnu.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdy.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgy.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rdz.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cyj.shanyushiyangtech.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nip.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rqe.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://ypx.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://khq.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://npk.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://atq.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://gep.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hym.andypj.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gps.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://ekk.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://gin.yuxming.cn

[F06] 删除文件
来源：http://ozr.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://cpb.hesvh.cn

PHP:  unlink("a.txt");
来源：http://xhf.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://eqq.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://iaq.yueranfly.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uux.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://dhw.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://rne.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://rly.cashguo.top

[F07] 创建目录（含多级）
来源：http://npp.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zbq.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uqy.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ogu.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lll.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nzd.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gex.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bxb.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfe.yj202588.top

[F08] 遍历目录
来源：http://byt.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://hbe.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xwx.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://ned.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://gyk.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gqv.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ggu.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://fnj.cashguo.top

C#:   Directory.GetFiles("dir")
来源：http://hym.nwbrower.top

[F09] 获取文件大小
来源：http://ezm.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://dkf.birdmap.top

PHP:  filesize("a.txt");
来源：http://ttq.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://tkb.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://zgt.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://kpx.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oel.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://hpa.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://xuw.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ovp.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xec.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qmq.smart0.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dbj.yongpay.top

TS:   path.extname("a.txt")
来源：http://vej.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://azj.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ktp.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yku.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nzm.chenlongwang.top

[F11] 复制与移动文件
来源：http://nko.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kzg.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://igt.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rar.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fqm.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ick.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://slr.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hza.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eyb.guannengcc.top

[F12] CSV 读写
来源：http://ofc.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vta.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jtv.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ruc.daria6918.cn

TS:   // 同上
来源：http://avg.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pku.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfb.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://grc.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iik.sxryk.cn

================================================================================
来源：http://cps.hcnkem.com

G. 面向对象
来源：http://ymm.ybcxt.top

================================================================================
来源：http://hce.nanxinkj.top

[G01] 定义类
来源：http://gjp.nwbrower.top

Py:   class User: pass
来源：http://rfp.mhx1999.top

PHP:  class User {}
来源：http://kzg.sufxvd.cn

JS:   class User {}
来源：http://gfz.zhijiandao.cn

TS:   class User { name: string = ""; }
来源：http://fyn.ydzc1.top


<!-- 参考信息 -->