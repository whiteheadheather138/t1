代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://onq.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fnx.yj20258888.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gmb.fktsv.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gyy.nanxuanxn.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://avw.xziqi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fbq.sxryk.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tqw.jianghu66.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ack.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://qgr.sufxvd.cn

Py:   "ab" * 3
来源：http://jqw.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://vye.tarul.cn

JS:   "ab".repeat(3)
来源：http://uhu.andypj.xyz

TS:   "ab".repeat(3)
来源：http://kwt.ppjwa.cn

Java: "ab".repeat(3)
来源：http://pjh.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://hrr.nwbrower.top

Ruby: "ab" * 3
来源：http://khk.jinghuilouyu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://izi.yvedp.cn

[E03] 截取子串
来源：http://wid.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yxr.yanxiufei.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dda.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tzk.xuetiantiany.cn

TS:   s.slice(1, 4)
来源：http://edq.aibaodan.cn

Java: s.substring(1, 4)
来源：http://fiu.havefunace.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://giy.fzhhl.top

Ruby: s[1, 3];  s[1..3]
来源：http://ava.yuxming.cn

C#:   s.Substring(1, 3)
来源：http://bby.dashuyun.cn

[E04] 查找子串位置
来源：http://lys.jinghuilouyu.cn

Py:   s.find("x");  s.index("x")
来源：http://knw.daxiang520.top

PHP:  strpos($s, "x");
来源：http://lvb.yj202588.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://akd.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://lfs.yueranfly.top

Java: s.indexOf("x")
来源：http://riq.daria6918.cn

Go:   strings.Index(s, "x")
来源：http://rub.zycfv.cn

Ruby: s.index("x")
来源：http://xig.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://uzp.ppjwa.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://osg.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uum.fehbvm.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zzn.zhiwuduotai.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nhp.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xku.jqgufenzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nas.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kpu.tanke756.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xos.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eme.wangdashe.top

[E06] 替换子串
来源：http://ecn.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bsc.cqqwz.cn

PHP:  str_replace("a", "b", $s);
来源：http://uks.yanxiufei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hea.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://nql.ydjk.org.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bhc.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zkw.hesvh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wjj.hysaishi.cn

C#:   s.Replace("a", "b")
来源：http://emo.pengpengdd.cyou

[E07] 按分隔符拆分
来源：http://eiy.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xzc.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tcm.daxiang520.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://lgq.jinqigfzy.top

TS:   s.split(",")
来源：http://vby.zhoulong.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ybv.jqgfzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bnk.nwbrower.top

Ruby: s.split(",");  s.split
来源：http://vtl.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ulb.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://ywg.hnxiangtu.top

Py:   ",".join(items)
来源：http://sre.meibo888.top

PHP:  implode(",", $items);
来源：http://oki.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://dok.hammf.cn

TS:   items.join(",")
来源：http://lkt.hysaishi.cn

Java: String.join(",", items)
来源：http://exh.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://vbp.hnxiangtu.top

Ruby: items.join(",")
来源：http://isp.xuanzx.com

C#:   string.Join(",", items)
来源：http://ocx.zdbjq.cn

[E09] 去除所有空白字符
来源：http://jrm.jqgufenzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://djq.fengsongda.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://cyj.shzxlz.cn

JS:   s.replace(/\s+/g, "")
来源：http://nov.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://rrb.jlsjyb.cn

Java: s.replaceAll("\\s+", "")
来源：http://agb.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://mbp.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://mcg.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ecx.yanxiufei.cn

[E10] 左侧补零 / 定长填充
来源：http://rfl.fzhhl.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dvy.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ozn.smart0.xyz

JS:   "7".padStart(3, "0")
来源：http://ghs.fktsv.cn

TS:   "7".padStart(3, "0")
来源：http://ymf.shuidangran.top

Java: String.format("%03d", 7)
来源：http://cbj.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ohx.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ans.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://imm.xinyue.icu

[E11] 反转字符串
来源：http://lmr.svipenyu.cn

Py:   s[::-1]
来源：http://fxs.yj202588.top

PHP:  strrev($s);
来源：http://yjf.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://ufm.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://otb.vehdjk.com

Java: new StringBuilder(s).reverse().toString()
来源：http://eke.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://asf.yuxming.cn

Ruby: s.reverse
来源：http://edq.zdqjudy.top

C#:   new string(s.Reverse().ToArray())
来源：http://pxl.52xcode.cn

[E12] 统计某字符出现次数
来源：http://vrw.yueranfly.top

Py:   s.count("a")
来源：http://hjq.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://fzf.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://mpu.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://hvg.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://drc.tanke756.top

Go:   strings.Count(s, "a")
来源：http://nhy.tianlin.xyz

Ruby: s.count("a")
来源：http://mqu.9152youxi.cn

C#:   s.Count(c => c == 'a')
来源：http://hpi.yuxming.cn

[E13] 逐字符遍历
来源：http://wxi.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://wjs.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vug.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aay.yongpay.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hpa.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ddg.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kat.shangyingyoupin.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zzb.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://snq.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://jxr.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gwt.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ret.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fmd.xuanzx.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnw.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ebc.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sat.xziqi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://onr.jinyuanbaomall.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ibj.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://kzl.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tjr.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ikh.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://egg.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yyi.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sdx.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bcu.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://deu.ppjwa.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pvr.feifeiyinyue.top

[E16] 数字千分位
来源：http://jnd.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://bbg.xuanzx.com

PHP:  number_format(1234567);
来源：http://vdi.yangfankeji.com

JS:   (1234567).toLocaleString("en-US")
来源：http://lte.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gpi.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vqt.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rzp.jianghu66.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://isl.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://xhp.guannengcc.top

[E17] 首字母大写
来源：http://gep.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://evo.guowangkeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ypp.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zpr.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djj.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gsm.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qzt.dianchejie.cn

Ruby: s.capitalize
来源：http://akp.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vpl.ctjpmb.com

[E18] 模板占位符替换
来源：http://qxi.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tsf.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://iub.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://inf.yangfankeji.com

TS:   tpl.replaceAll("{name}", name)
来源：http://nby.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ilm.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gmq.meibo888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cwa.sufxvd.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fyo.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://eom.yj20258888.top

Py:   s.splitlines()
来源：http://azy.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vxy.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://cnz.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://ozg.zdqjudy.top

Java: s.lines().toList()
来源：http://yah.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://ykg.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://zyw.yongpay.top

C#:   s.Split('\n')
来源：http://pvv.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://pkh.tarul.cn

Py:   if not s:
来源：http://aqn.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lqp.svipenyu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ysq.ctjpmb.com

TS:   if (s === "") {}
来源：http://whh.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://rco.andypj.xyz

Go:   if s == "" {}
来源：http://kxf.hammf.cn

Ruby: if s.empty?
来源：http://xhj.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rgj.gotoacloud.top

[E21] 超长截断加省略号
来源：http://dea.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://awz.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cvv.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sai.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kum.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ric.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://rls.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://czh.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mzu.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://iav.zhiwuduotai.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rpf.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mlr.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lso.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bmw.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cur.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rqj.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://kus.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cde.52xcode.cn

================================================================================
来源：http://hto.dianchejie.cn

F. 文件与目录
来源：http://hna.jqgfzy.top

================================================================================
来源：http://jez.xziqi.cn

[F01] 读取整个文件
来源：http://rnu.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vef.sjlbkw.cn

PHP:  file_get_contents("a.txt");
来源：http://jzk.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wbb.shangyingyoupin.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://box.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mly.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qbr.yj202588.top

Ruby: File.read("a.txt")
来源：http://thd.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://rdr.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://oxh.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uwg.zhaomingkeji.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lkh.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgz.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kll.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oxl.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wav.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ovl.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://msn.hammf.cn

[F03] 写入文件（覆盖）
来源：http://eux.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sgm.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://soi.hfpthk.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpw.ydzc1.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyf.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pwh.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvw.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://zyn.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aak.shzxlz.cn

[F04] 追加写入文件
来源：http://cyu.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pqw.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kwr.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bjl.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yjx.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://drb.guannengcc.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gjh.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://udc.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://syz.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://bss.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wne.316326.xyz

PHP:  file_exists("a.txt");
来源：http://xfg.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://gti.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://qne.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ltk.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://duz.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://ukt.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://pza.cdnleiting.top

[F06] 删除文件
来源：http://qvx.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://rtp.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://uyc.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mov.chenjidiqi.icu

TS:   fs.unlinkSync("a.txt")
来源：http://rsc.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wed.feifeiyinyue.top

Go:   os.Remove("a.txt")
来源：http://cnc.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://fub.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://vad.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://zig.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vlq.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yxg.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuu.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofe.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zec.shanyushiyangtech.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dtg.gzhubu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zaf.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bqh.redwolf501.top

[F08] 遍历目录
来源：http://xfh.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kff.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qml.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://yhe.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://nyv.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sun.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xez.jyoumei.cn

Ruby: Dir.children("dir")
来源：http://vcn.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://cxq.jqgfzy.top

[F09] 获取文件大小
来源：http://tyj.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://uws.tarul.cn

PHP:  filesize("a.txt");
来源：http://ign.hongshengwenyu.top

JS:   fs.statSync("a.txt").size
来源：http://mru.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://saq.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xfa.fehbvm.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hah.meibo888.top

Ruby: File.size("a.txt")
来源：http://faw.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://idr.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://wls.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nei.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rvo.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bpl.ybcxt.top

TS:   path.extname("a.txt")
来源：http://uky.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qgn.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://may.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://amx.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://amh.jianghu66.top

[F11] 复制与移动文件
来源：http://dfm.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lxg.birdmap.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pkd.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dbr.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://amv.hysaishi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pff.redwolf501.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kvk.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://byc.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pbw.iojbl.cn

[F12] CSV 读写
来源：http://lia.chenzaomai.com


<!-- 参考信息 -->