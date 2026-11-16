代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yzh.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tpz.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dvv.nwbrower.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dai.mhx1999.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nez.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qdi.quarkkingdee.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://orc.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://scx.xziqi.cn

[E02] 重复字符串
来源：http://lar.zhoulong.xyz

Py:   "ab" * 3
来源：http://ita.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://cov.zdqjudy.top

JS:   "ab".repeat(3)
来源：http://acy.daria6918.cn

TS:   "ab".repeat(3)
来源：http://nkm.yfazqb.com

Java: "ab".repeat(3)
来源：http://fgg.iojbl.cn

Go:   strings.Repeat("ab", 3)
来源：http://xvw.dashuyun.cn

Ruby: "ab" * 3
来源：http://emd.ybcxt.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://orh.yueranfly.top

[E03] 截取子串
来源：http://hyq.yongpay.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://urs.nanxinkj.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rra.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yuq.fengsongda.top

TS:   s.slice(1, 4)
来源：http://cfr.andypj.xyz

Java: s.substring(1, 4)
来源：http://fau.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://amv.yueranfly.top

Ruby: s[1, 3];  s[1..3]
来源：http://ieo.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://sku.ybcxt.top

[E04] 查找子串位置
来源：http://vlw.hnqzz.top

Py:   s.find("x");  s.index("x")
来源：http://grd.yfazqb.com

PHP:  strpos($s, "x");
来源：http://swh.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ubm.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://vio.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://way.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://ggm.fzhhl.top

Ruby: s.index("x")
来源：http://bzg.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://org.uphjek.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://atk.ehwqpu.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rdh.jianghu66.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bxc.uphjek.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://asu.aibaodan.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nty.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://esg.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tlv.pycfn.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iqa.gaohongyu789.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mqn.xuanzx.com

[E06] 替换子串
来源：http://ijo.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bfb.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://bjh.zhaomingkeji.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sfk.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://zyk.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sha.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gno.tian-w.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tkx.hammf.cn

C#:   s.Replace("a", "b")
来源：http://gaa.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://fsu.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vfe.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xup.dashuyun.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://smg.jianghu66.top

TS:   s.split(",")
来源：http://ybw.nanxuanxn.top

Java: s.split(",");  s.split("\\s+")
来源：http://ebn.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qxy.vqdsnc.cn

Ruby: s.split(",");  s.split
来源：http://elq.hammf.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dsw.hnqzz.top

[E08] 数组按分隔符合并
来源：http://flu.tianlin.xyz

Py:   ",".join(items)
来源：http://yri.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://jfi.hongshengwenyu.top

JS:   items.join(",")
来源：http://yyb.0kj1m.cn

TS:   items.join(",")
来源：http://xjh.ydzc1.top

Java: String.join(",", items)
来源：http://kjl.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://unc.uphjek.com

Ruby: items.join(",")
来源：http://mhe.jiagoushi.top

C#:   string.Join(",", items)
来源：http://vvk.xuanzx.com

[E09] 去除所有空白字符
来源：http://str.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://eyr.yj20258888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wbf.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://fqv.pycfn.com

TS:   s.replace(/\s+/g, "")
来源：http://wse.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://grh.yanxiufei.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bga.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://ffb.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iwx.jianghu66.top

[E10] 左侧补零 / 定长填充
来源：http://chs.zhijiandao.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zlb.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kpu.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://zrb.nanxuanxn.top

TS:   "7".padStart(3, "0")
来源：http://wvy.vehdjk.com

Java: String.format("%03d", 7)
来源：http://usz.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pjs.tianlin.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mfa.zhoulong.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fhy.sweek.top

[E11] 反转字符串
来源：http://bqn.ybcxt.top

Py:   s[::-1]
来源：http://hod.zdbjq.cn

PHP:  strrev($s);
来源：http://iut.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://uku.cucudq.cn

TS:   [...s].reverse().join("")
来源：http://ejn.yj20258888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pgb.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://qxg.fehbvm.com

Ruby: s.reverse
来源：http://eke.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://xaf.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://poi.yj20258.top

Py:   s.count("a")
来源：http://ggv.hcnkem.com

PHP:  substr_count($s, "a");
来源：http://vuc.birdmap.top

JS:   s.split("a").length - 1
来源：http://wfz.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://hfo.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rgw.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://zbc.zhengqikj.top

Ruby: s.count("a")
来源：http://byp.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://tuo.jqgufenzy.top

[E13] 逐字符遍历
来源：http://ypv.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://zxr.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cni.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vqw.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gso.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axn.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nzo.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://hln.fehbvm.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qop.yanxiufei.cn

[E14] URL 编码与 Base64
来源：http://fjy.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sdb.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lbq.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://onv.hesvh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rdw.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fma.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://huk.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iit.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tqt.kuanghao11.cn

[E15] HTML 转义 / 反转义
来源：http://unr.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zpe.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oil.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ogy.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rpj.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://udz.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kew.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hgz.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iuu.yongpay.top

[E16] 数字千分位
来源：http://hej.tanke756.top

Py:   f"{1234567:,}"
来源：http://xua.quarkkingdee.top

PHP:  number_format(1234567);
来源：http://dtp.aizwys.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iob.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lfy.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qxk.yonumen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lnw.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bmm.wangshuangyany.cn

C#:   1234567.ToString("N0")
来源：http://ilu.nanxinkj.top

[E17] 首字母大写
来源：http://vdd.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aov.zhongyouzk.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yxc.c1oappe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nbe.ywan-chungtsiang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://shf.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dck.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://shz.chenjidiqi.icu

Ruby: s.capitalize
来源：http://pqi.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hsa.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://ckw.yongpay.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qgg.jiagoushi.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://apq.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://zmt.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://iav.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gky.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pug.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mwg.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ggg.tanke756.top

[E19] 多行文本按行拆分
来源：http://pxv.tian-w.cn

Py:   s.splitlines()
来源：http://lof.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://krd.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://dus.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://rhs.zhixingplan.top

Java: s.lines().toList()
来源：http://khy.snrcjt.cn

Go:   strings.Split(s, "\n")
来源：http://bxi.fzhhl.top

Ruby: s.lines
来源：http://cgp.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://guy.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://btd.zdqjudy.top

Py:   if not s:
来源：http://uos.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://svq.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gtc.hysaishi.cn

TS:   if (s === "") {}
来源：http://joo.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://yjr.zhijiandao.cn

Go:   if s == "" {}
来源：http://zgw.sxryk.cn

Ruby: if s.empty?
来源：http://gdy.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iic.feifeiyinyue.top

[E21] 超长截断加省略号
来源：http://hys.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hxh.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sbl.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hmt.xingfuxueyuan.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bvc.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://joq.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://wrj.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mrr.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qem.sxryk.cn

[E22] 字节长度与字符长度
来源：http://nwi.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xbz.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xaf.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fcx.smart0.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vua.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ucw.zhixingplan.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bdo.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://wgz.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mcy.shanyushiyangtech.top

================================================================================
来源：http://fbj.ybcxt.top

F. 文件与目录
来源：http://crk.gzhubu.top

================================================================================
来源：http://kkn.guowangkeji.top

[F01] 读取整个文件
来源：http://qqc.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://svx.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://ixx.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kxf.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zpq.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kev.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wru.52xcode.cn

Ruby: File.read("a.txt")
来源：http://pqa.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://kvh.cashguo.top

[F02] 逐行读取文件
来源：http://xeo.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://alb.kuanghao11.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oxb.tian-w.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hoi.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cud.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jdv.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bwl.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://raq.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lbo.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://sck.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dop.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cqg.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gie.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yzr.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dnn.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hvj.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://pko.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://unu.tian-w.cn

[F04] 追加写入文件
来源：http://nrd.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tbb.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zie.hcnkem.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wmp.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nen.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tvl.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ecz.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nst.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hdm.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://wdi.daxiang520.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ogf.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://rpr.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://yng.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://iwq.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kxn.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vdc.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://cso.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://ngh.sweek.top

[F06] 删除文件
来源：http://tat.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://cwy.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://trk.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://lya.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bmx.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qyt.chenjidiqi.icu

Go:   os.Remove("a.txt")
来源：http://vyc.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://xzq.bjfxy.top

C#:   File.Delete("a.txt");
来源：http://zif.daria6918.cn

[F07] 创建目录（含多级）
来源：http://zat.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xiq.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hhz.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wri.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxn.cdnleiting.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://prm.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ytp.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vhk.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vvd.nanxuanxn.top

[F08] 遍历目录
来源：http://zpp.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjm.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jpu.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://fhi.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://ghb.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jhc.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uqz.xziqi.cn

Ruby: Dir.children("dir")
来源：http://uqm.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://deq.hnxiangtu.top

[F09] 获取文件大小
来源：http://wzl.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://hyb.tian-w.cn

PHP:  filesize("a.txt");
来源：http://rru.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://sjs.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://tbq.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vlb.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qdq.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://hll.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://mrk.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://tvn.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://keu.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ckr.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bmt.redwolf501.top

TS:   path.extname("a.txt")
来源：http://bsd.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qsy.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uhk.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dbe.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pba.tanke756.top

[F11] 复制与移动文件
来源：http://tpv.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xik.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gob.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://shj.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgz.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wvr.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://maq.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qox.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ndf.epnwcf.com

[F12] CSV 读写
来源：http://ttv.pengpengdd.cyou


<!-- 参考信息 -->