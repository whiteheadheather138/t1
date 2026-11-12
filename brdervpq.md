代发 wailian999

Java: String.join(", ", list)
来源：http://tnd.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://krn.yangfankeji.com

Ruby: arr.join(", ")
来源：http://gfv.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://piy.nanxinkj.top

================================================================================
来源：http://hfj.yuxming.cn

E. 字符串处理
来源：http://sya.hfpthk.cn

================================================================================
来源：http://chf.shanyushiyangkeji.top

[E01] 拼接字符串
来源：http://mzv.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fuo.gaohongyu789.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dgn.jinqigufen.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://whl.sweek.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lhq.52xcode.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kka.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ilo.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pvo.gaohongyu789.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dxt.haohaochexian.top

[E02] 重复字符串
来源：http://wxs.daria6918.cn

Py:   "ab" * 3
来源：http://pzs.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://jyx.wangdashe.top

JS:   "ab".repeat(3)
来源：http://mvw.hcnkem.com

TS:   "ab".repeat(3)
来源：http://teg.cqqwz.cn

Java: "ab".repeat(3)
来源：http://pwv.jyoumei.cn

Go:   strings.Repeat("ab", 3)
来源：http://cji.aibaodan.cn

Ruby: "ab" * 3
来源：http://akz.daxiang520.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lpo.hnqzz.top

[E03] 截取子串
来源：http://sjg.ydjk.org.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ndk.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lzn.hesvh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jdd.smart0.xyz

TS:   s.slice(1, 4)
来源：http://rjv.sweek.top

Java: s.substring(1, 4)
来源：http://wkh.aizwys.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lqd.0kj1m.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fic.0kj1m.cn

C#:   s.Substring(1, 3)
来源：http://chx.cqqwz.cn

[E04] 查找子串位置
来源：http://cdm.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://lkc.yanxiufei.cn

PHP:  strpos($s, "x");
来源：http://fft.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://oyp.nanxuanxn.top

TS:   s.indexOf("x")
来源：http://akn.aizwys.cn

Java: s.indexOf("x")
来源：http://wgx.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://ttc.nanxuanxn.top

Ruby: s.index("x")
来源：http://bgo.cashguo.top

C#:   s.IndexOf("x")
来源：http://jcb.dianchejie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kcy.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wnl.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nca.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzx.sjlbkw.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://syw.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mik.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yeu.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://amb.jinqigfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kvs.haohaochexian.top

[E06] 替换子串
来源：http://uyo.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rsb.zycfv.cn

PHP:  str_replace("a", "b", $s);
来源：http://akx.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fbz.shanyushiyangtech.top

TS:   s.replaceAll("a", "b")
来源：http://afx.ehwqpu.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hpl.aibaodan.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fii.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qfc.hywenlv.cn

C#:   s.Replace("a", "b")
来源：http://ngu.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://iok.tarul.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ixk.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mdq.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rri.sufxvd.cn

TS:   s.split(",")
来源：http://icf.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://ucm.fengsongda.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dqr.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://hor.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vzi.cashguo.top

[E08] 数组按分隔符合并
来源：http://nkx.hesvh.cn

Py:   ",".join(items)
来源：http://ler.9152youxi.cn

PHP:  implode(",", $items);
来源：http://eoh.aibaodan.cn

JS:   items.join(",")
来源：http://qoe.fehbvm.com

TS:   items.join(",")
来源：http://fig.havefunace.top

Java: String.join(",", items)
来源：http://srx.jinqigufen.top

Go:   strings.Join(items, ",")
来源：http://klz.shuidangran.top

Ruby: items.join(",")
来源：http://baa.ydjk.org.cn

C#:   string.Join(",", items)
来源：http://dec.ehwqpu.com

[E09] 去除所有空白字符
来源：http://imu.hysaishi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uzz.xylfe.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ppw.birdmap.top

JS:   s.replace(/\s+/g, "")
来源：http://rjy.haohaochexian.top

TS:   s.replace(/\s+/g, "")
来源：http://rrh.zdqjudy.top

Java: s.replaceAll("\\s+", "")
来源：http://zkr.yonumen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ewp.zhaomingkeji.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://dyn.feifeiyinyue.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqk.zhaomingkeji.xyz

[E10] 左侧补零 / 定长填充
来源：http://qnu.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jch.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wpg.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://csa.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://shr.wangshuangyany.cn

Java: String.format("%03d", 7)
来源：http://brt.jinyuanbaomall.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://evh.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bhu.jianghu66.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xia.chenlongwang.top

[E11] 反转字符串
来源：http://msv.bjfxy.top

Py:   s[::-1]
来源：http://rsu.chenzaomai.com

PHP:  strrev($s);
来源：http://zix.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://gee.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://zpr.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://voq.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xnx.hesvh.cn

Ruby: s.reverse
来源：http://bmv.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ezd.yueranfly.top

[E12] 统计某字符出现次数
来源：http://xjy.vehdjk.com

Py:   s.count("a")
来源：http://beg.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://sih.mhx1999.top

JS:   s.split("a").length - 1
来源：http://nws.yongpay.top

TS:   s.split("a").length - 1
来源：http://wls.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jim.fzhhl.top

Go:   strings.Count(s, "a")
来源：http://lnd.316326.xyz

Ruby: s.count("a")
来源：http://ffj.gotoacloud.top

C#:   s.Count(c => c == 'a')
来源：http://xxq.epnwcf.com

[E13] 逐字符遍历
来源：http://ypx.birdmap.top

Py:   for ch in s: print(ch)
来源：http://fur.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://igz.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ywi.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lzb.cdnleiting.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kxy.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bfe.zhijiandao.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xzt.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pwp.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://pvm.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://psh.sweek.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qdr.tianlin.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wuz.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jut.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edk.ybcxt.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://peq.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://luh.guowangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mee.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://dlz.birdmap.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ujc.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qkl.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rty.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://obi.tianlin.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://txt.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://usx.jinqigfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xaq.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hxg.hywenlv.cn

[E16] 数字千分位
来源：http://qqj.yueranfly.top

Py:   f"{1234567:,}"
来源：http://bgr.daxiang520.top

PHP:  number_format(1234567);
来源：http://tht.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wtx.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xtm.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bfn.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kfm.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://txu.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://chg.guowangkeji.top

[E17] 首字母大写
来源：http://uyl.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kfp.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lki.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kde.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxr.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nlc.xylfe.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wpo.zhongyouzk.top

Ruby: s.capitalize
来源：http://rwy.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://byv.chenlongwang.top

[E18] 模板占位符替换
来源：http://dya.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nkp.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gin.shanyushiyangtech.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cga.yonumen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lqa.hnqzz.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmo.wangdashe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lyi.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ahi.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzh.c1oappe.top

[E19] 多行文本按行拆分
来源：http://zuq.chenlongwang.top

Py:   s.splitlines()
来源：http://dfc.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dew.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://zbe.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://goh.yvedp.cn

Java: s.lines().toList()
来源：http://kua.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://dfj.shanyushiyangkeji.top

Ruby: s.lines
来源：http://qeh.ehwqpu.com

C#:   s.Split('\n')
来源：http://azo.uphjek.com

[E20] 判断字符串是否为空
来源：http://ekj.xuanzx.com

Py:   if not s:
来源：http://uhl.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qne.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yyn.sweek.top

TS:   if (s === "") {}
来源：http://psl.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://wqg.wangshuangyany.cn

Go:   if s == "" {}
来源：http://wxq.daxiang520.top

Ruby: if s.empty?
来源：http://bke.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gtu.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://qxk.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vga.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mrd.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://amj.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aiw.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cnv.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://lyi.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iub.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://buc.yonumen.top

[E22] 字节长度与字符长度
来源：http://xsc.zhijiandao.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zac.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ets.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://llz.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xjt.xylfe.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xby.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://loq.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://qka.yuanzhike.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vem.shangyingyoupin.top

================================================================================
来源：http://hvy.ydjk.org.cn

F. 文件与目录
来源：http://xau.bjfxy.top

================================================================================
来源：http://ouq.svipenyu.cn

[F01] 读取整个文件
来源：http://ony.dashuyun.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kis.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://sbj.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vky.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qyi.quarkkingdee.top

Java: Files.readString(Path.of("a.txt"))
来源：http://huk.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rvf.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://bnp.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://irs.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://gqa.yueranfly.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mih.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wye.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bwu.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ouj.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dia.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sxz.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qcy.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ylg.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://sni.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eya.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://odi.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dlf.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ace.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gkp.zhixingplan.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mlw.fehbvm.com

Ruby: File.write("a.txt", "hi")
来源：http://ykf.cqqwz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zsv.jlsjyb.cn

[F04] 追加写入文件
来源：http://jyk.guowangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lro.sjlbkw.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dbo.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tti.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sdc.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xpg.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uhe.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jrg.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wmj.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://pyq.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://grt.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://bwd.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://fqj.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://gxd.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wrt.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nkp.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://nkx.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://slv.shuidangran.top

[F06] 删除文件
来源：http://gzf.wangdashe.top

Py:   os.remove("a.txt")
来源：http://paq.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://ivp.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://qwl.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://lcj.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kqy.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://azp.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://uac.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://zim.mhx1999.top

[F07] 创建目录（含多级）
来源：http://nyv.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hti.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ryi.sweek.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wea.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ckj.uphjek.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kzi.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cyq.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sjn.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ogz.xziqi.cn

[F08] 遍历目录
来源：http://tez.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://arf.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pcn.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://yws.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://udl.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jyf.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ufn.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://urb.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://hbe.vehdjk.com

[F09] 获取文件大小
来源：http://dfz.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://poz.xuanzx.com

PHP:  filesize("a.txt");
来源：http://dnw.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://hwl.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://opu.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://eqi.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://flq.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://tox.sweek.top

C#:   new FileInfo("a.txt").Length
来源：http://mbp.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://ukv.shzxlz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dvd.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yjg.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mlj.hcnkem.com

TS:   path.extname("a.txt")
来源：http://wdf.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://upb.guowangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhn.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vfd.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tig.jqgfzy.top

[F11] 复制与移动文件
来源：http://qcj.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kbd.yuxming.cn


<!-- 参考信息 -->