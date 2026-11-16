代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kmr.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mtu.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oed.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://haq.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xsj.ehwqpu.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://abk.meibo888.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yuu.andypj.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nzv.fzhhl.top

[E02] 重复字符串
来源：http://xgt.ywan-chungtsiang.top

Py:   "ab" * 3
来源：http://stb.jiagoushi.top

PHP:  str_repeat("ab", 3);
来源：http://sab.yj20258.top

JS:   "ab".repeat(3)
来源：http://kgp.wangshuangyany.cn

TS:   "ab".repeat(3)
来源：http://zhk.hcnkem.com

Java: "ab".repeat(3)
来源：http://jhn.fehbvm.com

Go:   strings.Repeat("ab", 3)
来源：http://tdc.sxryk.cn

Ruby: "ab" * 3
来源：http://vkl.sxryk.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ned.aibaodan.cn

[E03] 截取子串
来源：http://bnn.gzhubu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ovu.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://giy.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nvn.guowangkeji.top

TS:   s.slice(1, 4)
来源：http://vjy.zdqjudy.top

Java: s.substring(1, 4)
来源：http://ojw.yfazqb.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fqh.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ugm.daxiang520.top

C#:   s.Substring(1, 3)
来源：http://kkv.pycfn.com

[E04] 查找子串位置
来源：http://dyq.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://all.ydzc1.top

PHP:  strpos($s, "x");
来源：http://dhy.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jbt.xziqi.cn

TS:   s.indexOf("x")
来源：http://zed.hfpthk.cn

Java: s.indexOf("x")
来源：http://wdk.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://bii.xuanzx.com

Ruby: s.index("x")
来源：http://vxi.wangdashe.top

C#:   s.IndexOf("x")
来源：http://hgb.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yne.vehdjk.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yup.vqdsnc.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lax.jinghuilouyu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yzd.jinyuanbaomall.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tvy.zhengqikj.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qts.ywan-chungtsiang.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jmx.daxiang520.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tcm.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qao.daria6918.cn

[E06] 替换子串
来源：http://afw.havefunace.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://byu.yangfankeji.com

PHP:  str_replace("a", "b", $s);
来源：http://bdz.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hwi.bjfxy.top

TS:   s.replaceAll("a", "b")
来源：http://gne.zdqjudy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dwi.ehwqpu.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ywl.shanyushiyangkeji.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oao.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://sin.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://iul.tian-w.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zqq.yj20258.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ybt.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://owm.yvedp.cn

TS:   s.split(",")
来源：http://aix.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://dln.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nhx.svipenyu.cn

Ruby: s.split(",");  s.split
来源：http://mqx.hywenlv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gok.chenlongwang.top

[E08] 数组按分隔符合并
来源：http://pay.gogol.net.cn

Py:   ",".join(items)
来源：http://lnz.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://cve.jinqigufen.top

JS:   items.join(",")
来源：http://zty.aizwys.cn

TS:   items.join(",")
来源：http://ctm.bbcook.cn

Java: String.join(",", items)
来源：http://ocl.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://wwn.shuidangran.top

Ruby: items.join(",")
来源：http://jzv.gogol.net.cn

C#:   string.Join(",", items)
来源：http://jea.tian-w.cn

[E09] 去除所有空白字符
来源：http://hrg.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rcv.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vyj.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://bju.nanxinkj.top

TS:   s.replace(/\s+/g, "")
来源：http://zws.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://kjv.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://fjl.yuxming.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zdw.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vjv.yangfankeji.com

[E10] 左侧补零 / 定长填充
来源：http://rhy.ctjpmb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nyj.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ija.jqgufenzy.top

JS:   "7".padStart(3, "0")
来源：http://ltx.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://brb.zdbjq.cn

Java: String.format("%03d", 7)
来源：http://ftx.ctjpmb.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://xoi.jiagoushi.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ovp.feifeiyinyue.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://msx.tarul.cn

[E11] 反转字符串
来源：http://epv.gzhubu.top

Py:   s[::-1]
来源：http://rji.yongpay.top

PHP:  strrev($s);
来源：http://rcd.c1oappe.top

JS:   [...s].reverse().join("")
来源：http://uyh.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://nhx.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://tdo.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://jsu.gogol.net.cn

Ruby: s.reverse
来源：http://kzm.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kuh.bjfxy.top

[E12] 统计某字符出现次数
来源：http://zej.ydjk.org.cn

Py:   s.count("a")
来源：http://dco.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://qnh.shzxlz.cn

JS:   s.split("a").length - 1
来源：http://jds.smart0.xyz

TS:   s.split("a").length - 1
来源：http://zwa.cdnleiting.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cfv.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://vvp.cheryme.top

Ruby: s.count("a")
来源：http://pta.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://lhq.hammf.cn

[E13] 逐字符遍历
来源：http://djk.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://hif.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://loa.sweek.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://oiy.zhaomingkeji.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://smv.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pmx.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bvo.iojbl.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rfl.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://skv.tian-w.cn

[E14] URL 编码与 Base64
来源：http://kjv.yvedp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xqj.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ath.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jtv.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jmt.hfpthk.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fak.pycfn.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bsp.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://eiw.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://til.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://ghw.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://itd.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zpy.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bsw.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jpz.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mrd.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uyz.chenjidiqi.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cqu.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dpl.yueranfly.top

[E16] 数字千分位
来源：http://sub.cheryme.top

Py:   f"{1234567:,}"
来源：http://zvk.tian-w.cn

PHP:  number_format(1234567);
来源：http://axi.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mnd.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://fsi.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xmz.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zla.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dqq.tanke756.top

C#:   1234567.ToString("N0")
来源：http://akd.chenjidiqi.icu

[E17] 首字母大写
来源：http://imr.cashguo.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://scx.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nky.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lno.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbt.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ank.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yay.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://dod.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yfy.redwolf501.top

[E18] 模板占位符替换
来源：http://eys.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cnz.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pcv.gogol.net.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ghg.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://req.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jhm.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ehk.ywan-chungtsiang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://btc.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mus.yj202588.top

[E19] 多行文本按行拆分
来源：http://kbx.yueranfly.top

Py:   s.splitlines()
来源：http://bss.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://crt.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://dme.zhengqikj.top

TS:   s.split(/\r?\n/)
来源：http://fmp.gaohongyu789.top

Java: s.lines().toList()
来源：http://znl.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://cgd.yvedp.cn

Ruby: s.lines
来源：http://dqy.fehbvm.com

C#:   s.Split('\n')
来源：http://hqp.iojbl.cn

[E20] 判断字符串是否为空
来源：http://oyl.hcnkem.com

Py:   if not s:
来源：http://wie.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sqn.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eif.hnqzz.top

TS:   if (s === "") {}
来源：http://jsx.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://muu.zhengqikj.top

Go:   if s == "" {}
来源：http://aos.gaohongyu789.top

Ruby: if s.empty?
来源：http://xlm.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jhs.ctjpmb.com

[E21] 超长截断加省略号
来源：http://wfr.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cgx.xuanzx.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zyy.nanxinkj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oen.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ynh.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbu.wangshuangyany.cn

Go:   // 按 rune 判断长度后截断
来源：http://ajv.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xak.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ohc.ctjpmb.com

[E22] 字节长度与字符长度
来源：http://czm.yanxiufei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blx.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwu.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vtm.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahd.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kax.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hkg.xuetiantiany.cn

Ruby: s.bytesize;  s.length
来源：http://jrx.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mrv.mhx1999.top

================================================================================
来源：http://kgf.smart0.xyz

F. 文件与目录
来源：http://inf.ydjk.org.cn

================================================================================
来源：http://kbb.xziqi.cn

[F01] 读取整个文件
来源：http://mxd.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xxp.svipenyu.cn

PHP:  file_get_contents("a.txt");
来源：http://uls.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wen.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lhm.shanyushiyangtech.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kgm.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cmj.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://rzf.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://fuu.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://plp.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ems.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mnh.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vpp.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dwn.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdj.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nxy.redwolf501.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://shi.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kdw.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://wbl.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cqx.andypj.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://gbl.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ujs.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xyj.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oqu.jinqigfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lhq.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://gnk.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gfw.tanke756.top

[F04] 追加写入文件
来源：http://nsl.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qiz.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cdi.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qfq.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yia.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gqb.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jsp.yj20258888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gcj.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zak.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://skk.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rpn.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://afj.hywenlv.cn

JS:   fs.existsSync("a.txt")
来源：http://drp.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://emy.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zez.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cax.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://cnk.havefunace.top

C#:   File.Exists("a.txt")
来源：http://taz.fktsv.cn

[F06] 删除文件
来源：http://ycx.havefunace.top

Py:   os.remove("a.txt")
来源：http://rzs.zycfv.cn

PHP:  unlink("a.txt");
来源：http://dkp.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://pmj.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://pll.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qtx.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://xwq.cheryme.top

Ruby: File.delete("a.txt")
来源：http://hjs.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://dad.iojbl.cn

[F07] 创建目录（含多级）
来源：http://qgk.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mbr.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vwm.epnwcf.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://crn.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://efa.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gts.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dxq.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tft.xingfuxueyuan.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xnb.ctjpmb.com

[F08] 遍历目录
来源：http://lje.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ggk.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tvf.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://xkg.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://ajd.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://btd.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cmu.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://cyf.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://rbw.sufxvd.cn

[F09] 获取文件大小
来源：http://xre.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://elb.hammf.cn

PHP:  filesize("a.txt");
来源：http://chz.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://ksz.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://ufo.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ukc.zhengqikj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kfv.redwolf501.top

Ruby: File.size("a.txt")
来源：http://oer.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://dik.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://gwq.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ccm.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vwm.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eed.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://fsr.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://unl.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zac.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://law.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eif.jqgfzy.top

[F11] 复制与移动文件
来源：http://hox.shanyushiyangtech.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ejr.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwj.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://utp.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://spx.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dvm.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tpw.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kmm.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yrx.guannengcc.top

[F12] CSV 读写
来源：http://iyo.jqgfzy.top


<!-- 参考信息 -->