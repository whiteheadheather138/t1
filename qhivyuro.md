代发 wailian999

Java: String.join(", ", list)
来源：http://llr.yueranfly.top

Go:   strings.Join(strs, ", ")
来源：http://qgx.chenzaomai.com

Ruby: arr.join(", ")
来源：http://wxk.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://amj.xinyue.icu

================================================================================
来源：http://inz.jiagoushi.top

E. 字符串处理
来源：http://xjv.0kj1m.cn

================================================================================
来源：http://jtv.gaohongyu789.top

[E01] 拼接字符串
来源：http://xjs.zdqjudy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jwn.xylfe.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lzn.pycfn.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uol.quarkkingdee.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tuz.cheryme.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gta.316326.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://rel.shuidangran.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wsl.xylfe.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jhw.bjfxy.top

[E02] 重复字符串
来源：http://joe.feifeiyinyue.top

Py:   "ab" * 3
来源：http://mko.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://yut.xuanzx.com

JS:   "ab".repeat(3)
来源：http://yzu.yonumen.top

TS:   "ab".repeat(3)
来源：http://lhg.9152youxi.cn

Java: "ab".repeat(3)
来源：http://zhq.yuxming.cn

Go:   strings.Repeat("ab", 3)
来源：http://imp.jlsjyb.cn

Ruby: "ab" * 3
来源：http://eal.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yuj.tianlin.xyz

[E03] 截取子串
来源：http://wji.dianchejie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gor.chenjidiqi.icu

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://crs.yonumen.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://csx.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://xce.yongpay.top

Java: s.substring(1, 4)
来源：http://aqe.feifeiyinyue.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rys.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ojj.zhiwuduotai.top

C#:   s.Substring(1, 3)
来源：http://fdz.guannengcc.top

[E04] 查找子串位置
来源：http://nqb.316326.xyz

Py:   s.find("x");  s.index("x")
来源：http://shg.iojbl.cn

PHP:  strpos($s, "x");
来源：http://yvw.ctjpmb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://usu.zdbjq.cn

TS:   s.indexOf("x")
来源：http://plt.bjfxy.top

Java: s.indexOf("x")
来源：http://qcf.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://evr.xuanzx.com

Ruby: s.index("x")
来源：http://jqq.sweek.top

C#:   s.IndexOf("x")
来源：http://udz.yuanzhike.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xcy.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ojl.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ihc.0kj1m.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://njp.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kky.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xwu.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qzk.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://out.sufxvd.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kjc.guannengcc.top

[E06] 替换子串
来源：http://jao.haohaochexian.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vxs.ivvv.top

PHP:  str_replace("a", "b", $s);
来源：http://gcy.zhoulong.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uiw.hysaishi.cn

TS:   s.replaceAll("a", "b")
来源：http://qxh.haohaochexian.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cqt.meibo888.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mpq.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tdk.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://dnq.sxryk.cn

[E07] 按分隔符拆分
来源：http://mhy.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iwz.fanxiaobao.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://oxw.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bia.birdmap.top

TS:   s.split(",")
来源：http://tvj.xylfe.cn

Java: s.split(",");  s.split("\\s+")
来源：http://adx.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sql.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://flg.pengpengdd.cyou

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zuo.zhijiandao.cn

[E08] 数组按分隔符合并
来源：http://iuh.meibo888.top

Py:   ",".join(items)
来源：http://nlu.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://iey.9152youxi.cn

JS:   items.join(",")
来源：http://ngz.jyoumei.cn

TS:   items.join(",")
来源：http://xuq.yj20258888.top

Java: String.join(",", items)
来源：http://fnh.snrcjt.cn

Go:   strings.Join(items, ",")
来源：http://tid.smart0.xyz

Ruby: items.join(",")
来源：http://ajy.hfpthk.cn

C#:   string.Join(",", items)
来源：http://kkt.mhx1999.top

[E09] 去除所有空白字符
来源：http://dzh.yueranfly.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pjm.redwolf501.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mwo.ydzc1.top

JS:   s.replace(/\s+/g, "")
来源：http://yak.ydzc1.top

TS:   s.replace(/\s+/g, "")
来源：http://vme.tian-w.cn

Java: s.replaceAll("\\s+", "")
来源：http://dgl.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://tnq.jyoumei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zow.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://icr.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://sct.hesvh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://brq.zdbjq.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lpr.cheryme.top

JS:   "7".padStart(3, "0")
来源：http://vyk.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://car.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://kky.jinqigufen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://epp.yvedp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jtr.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dsn.haohaochexian.top

[E11] 反转字符串
来源：http://gaa.feifeiyinyue.top

Py:   s[::-1]
来源：http://znu.shuidangran.top

PHP:  strrev($s);
来源：http://hut.yuanzhike.top

JS:   [...s].reverse().join("")
来源：http://ihm.xziqi.cn

TS:   [...s].reverse().join("")
来源：http://wmn.yuxming.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qti.mhx1999.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xfz.fktsv.cn

Ruby: s.reverse
来源：http://ukc.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://tfa.52xcode.cn

[E12] 统计某字符出现次数
来源：http://krk.chenzaomai.com

Py:   s.count("a")
来源：http://snc.pycfn.com

PHP:  substr_count($s, "a");
来源：http://ssq.andypj.xyz

JS:   s.split("a").length - 1
来源：http://zwk.xziqi.cn

TS:   s.split("a").length - 1
来源：http://rry.xinyue.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ohd.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://dhz.cashguo.top

Ruby: s.count("a")
来源：http://sik.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://zpj.zhoulong.xyz

[E13] 逐字符遍历
来源：http://anj.chenlongwang.top

Py:   for ch in s: print(ch)
来源：http://quj.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dge.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://koi.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://ika.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jzk.vqdsnc.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rik.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://byo.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rjy.yueranfly.top

[E14] URL 编码与 Base64
来源：http://vsz.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xxz.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ovh.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kyb.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fim.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qax.sufxvd.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hxy.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jvu.wangshuangyany.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yfe.zycfv.cn

[E15] HTML 转义 / 反转义
来源：http://rvi.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bbg.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nhe.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cav.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pip.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://abe.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qlf.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hzy.jyoumei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://snu.sjlbkw.cn

[E16] 数字千分位
来源：http://pqh.zhaomingkeji.xyz

Py:   f"{1234567:,}"
来源：http://qmw.cheryme.top

PHP:  number_format(1234567);
来源：http://tey.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wjq.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ztr.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zcv.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ihg.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nrk.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://cxo.nwbrower.top

[E17] 首字母大写
来源：http://jra.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dep.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://prd.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dyz.gaohongyu789.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yqh.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gjo.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lom.yanxiufei.cn

Ruby: s.capitalize
来源：http://rcr.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wvy.svipenyu.cn

[E18] 模板占位符替换
来源：http://qxb.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xww.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xil.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://yas.wangshuangyany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fhr.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lwc.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yff.ybcxt.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://edp.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nba.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://yxq.zhoulong.xyz

Py:   s.splitlines()
来源：http://unj.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sus.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://imi.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://jwt.dianchejie.cn

Java: s.lines().toList()
来源：http://fed.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://jah.jinyuanbaomall.cn

Ruby: s.lines
来源：http://yay.havefunace.top

C#:   s.Split('\n')
来源：http://ryr.52xcode.cn

[E20] 判断字符串是否为空
来源：http://qhy.yongpay.top

Py:   if not s:
来源：http://bjj.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zde.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qif.nanxuanxn.top

TS:   if (s === "") {}
来源：http://bpz.gzhubu.top

Java: if (s.isEmpty()) {}
来源：http://kev.cashguo.top

Go:   if s == "" {}
来源：http://zfv.jlsjyb.cn

Ruby: if s.empty?
来源：http://pfg.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gmc.gzhubu.top

[E21] 超长截断加省略号
来源：http://kkx.haohaochexian.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kwz.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezq.cheryme.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryq.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lnm.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pfq.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://wwh.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ucu.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lgo.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://czn.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yrh.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://npq.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://njn.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tpj.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ntl.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vyr.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://mtc.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dyl.xingfuxueyuan.xyz

================================================================================
来源：http://pqd.sysykeji.top

F. 文件与目录
来源：http://plz.gotoacloud.top

================================================================================
来源：http://ofm.zdqjudy.top

[F01] 读取整个文件
来源：http://rvm.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wbw.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://hoz.wangshuangyany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xzs.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://axn.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://mni.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gwa.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://hld.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://uwt.xinyue.icu

[F02] 逐行读取文件
来源：http://bxk.316326.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://glj.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gsb.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ozp.jinyuanbaomall.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sia.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nud.smart0.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ufv.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ifp.jinyuanbaomall.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://koc.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://tle.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fsx.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://axy.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wtg.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxo.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vuc.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xap.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://nwj.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://frn.jinqigufen.top

[F04] 追加写入文件
来源：http://ahs.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zit.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pln.vqdsnc.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mit.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ozb.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xum.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jpi.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://geo.birdmap.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fcy.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://nia.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gyw.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://zdj.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://fiw.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://yab.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vhm.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vxq.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://cay.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://pza.cheryme.top

[F06] 删除文件
来源：http://noo.zycfv.cn

Py:   os.remove("a.txt")
来源：http://uwk.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://qom.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wlw.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://hpz.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsu.birdmap.top

Go:   os.Remove("a.txt")
来源：http://ksg.chenjidiqi.icu

Ruby: File.delete("a.txt")
来源：http://blx.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://ome.9152youxi.cn

[F07] 创建目录（含多级）
来源：http://rcw.hywenlv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hqc.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gcj.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aor.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://npc.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nca.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gfe.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gyl.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://azg.gaohongyu789.top

[F08] 遍历目录
来源：http://wcr.pengpengdd.cyou

Py:   for name in os.listdir("dir"): print(name)
来源：http://sqs.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wnp.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://wgi.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://ans.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fes.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rrh.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://xts.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://izr.ivvv.top

[F09] 获取文件大小
来源：http://rpq.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://kwr.xylfe.cn

PHP:  filesize("a.txt");
来源：http://jup.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://ath.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://jla.xuetiantiany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yfj.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hyr.daria6918.cn

Ruby: File.size("a.txt")
来源：http://rhn.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://uxc.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://bwb.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mrk.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://miw.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wrn.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://sxd.fengsongda.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mcz.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wjx.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sfb.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uul.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://jsp.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ecx.zhoulong.xyz


<!-- 参考信息 -->