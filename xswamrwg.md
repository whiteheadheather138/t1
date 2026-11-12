代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hnm.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://uhj.zhoulong.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lvi.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yot.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jbi.gaohongyu789.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tbo.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yhm.aizwys.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bdp.jyoumei.cn

[E02] 重复字符串
来源：http://ybw.hysaishi.cn

Py:   "ab" * 3
来源：http://sqk.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://jbg.meibo888.top

JS:   "ab".repeat(3)
来源：http://sci.zhixingplan.top

TS:   "ab".repeat(3)
来源：http://qyk.c1oappe.top

Java: "ab".repeat(3)
来源：http://ksd.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://esr.ydjk.org.cn

Ruby: "ab" * 3
来源：http://bnv.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yvj.nwbrower.top

[E03] 截取子串
来源：http://opm.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://enp.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dia.chenzaomai.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nya.ehwqpu.com

TS:   s.slice(1, 4)
来源：http://rag.yongpay.top

Java: s.substring(1, 4)
来源：http://tas.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wix.vqdsnc.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hzl.zycfv.cn

C#:   s.Substring(1, 3)
来源：http://cgq.guannengcc.top

[E04] 查找子串位置
来源：http://fly.fanxiaobao.xyz

Py:   s.find("x");  s.index("x")
来源：http://tgg.guowangkeji.top

PHP:  strpos($s, "x");
来源：http://sqe.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ewt.xinyue.icu

TS:   s.indexOf("x")
来源：http://xgj.jqgfzy.top

Java: s.indexOf("x")
来源：http://kje.316326.xyz

Go:   strings.Index(s, "x")
来源：http://vyn.yangfankeji.com

Ruby: s.index("x")
来源：http://ror.yvedp.cn

C#:   s.IndexOf("x")
来源：http://ahq.guowangkeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eym.gotoacloud.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oqu.zhongyouzk.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vbn.jqgfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qfg.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cqu.shzxlz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wxp.jinqigufen.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://muj.ybcxt.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eum.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eig.hammf.cn

[E06] 替换子串
来源：http://rhs.wangdashe.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fer.sxryk.cn

PHP:  str_replace("a", "b", $s);
来源：http://tez.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mhs.zhengqikj.top

TS:   s.replaceAll("a", "b")
来源：http://vhm.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ubu.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://isn.jinqigufen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pfv.vqdsnc.cn

C#:   s.Replace("a", "b")
来源：http://dim.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://eta.zhixingplan.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bpd.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ahg.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xkj.fktsv.cn

TS:   s.split(",")
来源：http://jzr.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://fvh.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wqm.sweek.top

Ruby: s.split(",");  s.split
来源：http://sbc.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://czs.cheryme.top

[E08] 数组按分隔符合并
来源：http://hdy.snrcjt.cn

Py:   ",".join(items)
来源：http://xqv.mhx1999.top

PHP:  implode(",", $items);
来源：http://lnq.xziqi.cn

JS:   items.join(",")
来源：http://cdw.yonumen.top

TS:   items.join(",")
来源：http://rse.cdnleiting.top

Java: String.join(",", items)
来源：http://whq.tarul.cn

Go:   strings.Join(items, ",")
来源：http://xgr.zdbjq.cn

Ruby: items.join(",")
来源：http://eqf.hcnkem.com

C#:   string.Join(",", items)
来源：http://ebf.redwolf501.top

[E09] 去除所有空白字符
来源：http://bbv.316326.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ina.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bgk.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://bit.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://sbu.yueranfly.top

Java: s.replaceAll("\\s+", "")
来源：http://tnf.jianghu66.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbo.316326.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://zzj.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ufr.yj20258888.top

[E10] 左侧补零 / 定长填充
来源：http://tln.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://thn.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://izl.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://djo.yj20258.top

TS:   "7".padStart(3, "0")
来源：http://qzx.epnwcf.com

Java: String.format("%03d", 7)
来源：http://lzi.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zia.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxp.vehdjk.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://idi.ehwqpu.com

[E11] 反转字符串
来源：http://zur.gzhubu.top

Py:   s[::-1]
来源：http://flp.jiagoushi.top

PHP:  strrev($s);
来源：http://xha.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://ocn.tarul.cn

TS:   [...s].reverse().join("")
来源：http://hrs.hywenlv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vbg.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ifx.havefunace.top

Ruby: s.reverse
来源：http://xdk.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://odz.mhx1999.top

[E12] 统计某字符出现次数
来源：http://sgl.aizwys.cn

Py:   s.count("a")
来源：http://bru.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://eou.jyoumei.cn

JS:   s.split("a").length - 1
来源：http://mgn.hammf.cn

TS:   s.split("a").length - 1
来源：http://bwy.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://igo.xingfuxueyuan.xyz

Go:   strings.Count(s, "a")
来源：http://hxf.jinqigufen.top

Ruby: s.count("a")
来源：http://vhs.zhoulong.xyz

C#:   s.Count(c => c == 'a')
来源：http://vae.bbcook.cn

[E13] 逐字符遍历
来源：http://ypq.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://ulb.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vzd.smart0.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ixc.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://xse.chenlongwang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zcf.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fgh.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://gbp.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mlv.andypj.xyz

[E14] URL 编码与 Base64
来源：http://fln.yongpay.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ztp.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bcj.nwbrower.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uwy.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kva.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zuq.ctjpmb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xex.bbcook.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://htw.sweek.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ysi.yueranfly.top

[E15] HTML 转义 / 反转义
来源：http://ebi.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://upp.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qbw.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aiv.yj20258888.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yjf.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xpe.kuanghao11.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yww.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hhy.cheryme.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kkd.andypj.xyz

[E16] 数字千分位
来源：http://xys.hcnkem.com

Py:   f"{1234567:,}"
来源：http://ouc.sweek.top

PHP:  number_format(1234567);
来源：http://ius.daria6918.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gvy.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hcc.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rkx.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eoy.hnxiangtu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://duz.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://rcx.fzhhl.top

[E17] 首字母大写
来源：http://was.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://suj.hnqzz.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mhi.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gkc.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://osd.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://stx.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jfv.pycfn.com

Ruby: s.capitalize
来源：http://ihb.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xjc.epnwcf.com

[E18] 模板占位符替换
来源：http://vyk.zdqjudy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://llv.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eoj.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://owl.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bqd.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://knk.xziqi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kfs.vehdjk.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fnb.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fyg.316326.xyz

[E19] 多行文本按行拆分
来源：http://isa.hcnkem.com

Py:   s.splitlines()
来源：http://dto.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jyt.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://oxv.ivvv.top

TS:   s.split(/\r?\n/)
来源：http://sdw.mhx1999.top

Java: s.lines().toList()
来源：http://csv.jqgfzy.top

Go:   strings.Split(s, "\n")
来源：http://jbp.sxryk.cn

Ruby: s.lines
来源：http://tfe.sxryk.cn

C#:   s.Split('\n')
来源：http://xua.xylfe.cn

[E20] 判断字符串是否为空
来源：http://awb.haohaochexian.top

Py:   if not s:
来源：http://pui.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oly.aizwys.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qoy.xingfuxueyuan.xyz

TS:   if (s === "") {}
来源：http://kwt.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://zzx.jinqigfzy.top

Go:   if s == "" {}
来源：http://uaa.cdnleiting.top

Ruby: if s.empty?
来源：http://uyq.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ozt.hnqzz.top

[E21] 超长截断加省略号
来源：http://hog.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://snu.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://egp.yj20258.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dkq.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://waq.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rxf.iojbl.cn

Go:   // 按 rune 判断长度后截断
来源：http://czd.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://okf.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qcu.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://pju.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://btb.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://acy.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pik.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qjs.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mjt.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ffm.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://ory.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tpv.xylfe.cn

================================================================================
来源：http://gal.ehwqpu.com

F. 文件与目录
来源：http://ptm.sweek.top

================================================================================
来源：http://udw.jiagoushi.top

[F01] 读取整个文件
来源：http://nag.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qau.wangdashe.top

PHP:  file_get_contents("a.txt");
来源：http://nwz.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ihi.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vti.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tod.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qrl.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://sig.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://uiy.hnxiangtu.top

[F02] 逐行读取文件
来源：http://gki.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ajr.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://goz.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwf.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxv.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://avk.pycfn.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wyv.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qdd.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gdw.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://jmn.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fef.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lhy.ywan-chungtsiang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubi.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yiw.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cyb.kuanghao11.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vqi.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://gcr.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gey.cheryme.top

[F04] 追加写入文件
来源：http://tsb.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tir.sweek.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xxo.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mjb.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rtr.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vna.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://isr.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qyt.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rbj.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://xsu.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jue.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://dlw.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://kyh.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://xdb.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kok.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vph.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://nky.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://irs.sufxvd.cn

[F06] 删除文件
来源：http://yzc.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://myh.xziqi.cn

PHP:  unlink("a.txt");
来源：http://nkg.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://hda.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hao.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fxx.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://otj.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://spt.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://chq.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://llg.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ivy.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fuv.zhengqikj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://txt.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhn.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bhf.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://paf.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bva.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jfh.9152youxi.cn

[F08] 遍历目录
来源：http://zrs.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vgn.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hzx.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://jfr.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://epv.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bfe.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://czr.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://edb.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://loi.smart0.xyz

[F09] 获取文件大小
来源：http://lim.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://mrx.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://hyz.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://ruj.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://beu.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://etz.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rbd.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://lgf.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://qlr.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://ucr.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvh.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ici.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ker.feifeiyinyue.top

TS:   path.extname("a.txt")
来源：http://hio.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxq.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wbb.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ill.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mzl.aibaodan.cn

[F11] 复制与移动文件
来源：http://nzz.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sqb.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxp.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wjd.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkq.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lqn.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://frv.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://evz.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rwi.wangdashe.top

[F12] CSV 读写
来源：http://ifg.ydzc1.top


<!-- 参考信息 -->