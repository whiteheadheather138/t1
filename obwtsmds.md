代发 wailian999

================================================================================
来源：http://dfy.yangfankeji.com

E. 字符串处理
来源：http://lbd.hnqzz.top

================================================================================
来源：http://sph.zhengqikj.top

[E01] 拼接字符串
来源：http://bno.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kgo.xziqi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zhl.tianlin.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zhh.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nyb.gaohongyu789.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nul.havefunace.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dfc.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uyo.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zse.smart0.xyz

[E02] 重复字符串
来源：http://oym.yonumen.top

Py:   "ab" * 3
来源：http://yow.cucudq.cn

PHP:  str_repeat("ab", 3);
来源：http://dey.fktsv.cn

JS:   "ab".repeat(3)
来源：http://yiq.xziqi.cn

TS:   "ab".repeat(3)
来源：http://bis.shuidangran.top

Java: "ab".repeat(3)
来源：http://cpz.mhx1999.top

Go:   strings.Repeat("ab", 3)
来源：http://mgu.zdbjq.cn

Ruby: "ab" * 3
来源：http://njz.hcnkem.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gni.sxryk.cn

[E03] 截取子串
来源：http://han.sufxvd.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zhh.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sde.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hba.tarul.cn

TS:   s.slice(1, 4)
来源：http://glm.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://qko.shanyushiyangtech.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rdh.52xcode.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bup.9152youxi.cn

C#:   s.Substring(1, 3)
来源：http://sab.meibo888.top

[E04] 查找子串位置
来源：http://puy.chenjidiqi.icu

Py:   s.find("x");  s.index("x")
来源：http://cwb.tanke756.top

PHP:  strpos($s, "x");
来源：http://dpj.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dgl.9152youxi.cn

TS:   s.indexOf("x")
来源：http://ogo.nanxinkj.top

Java: s.indexOf("x")
来源：http://axf.jlsjyb.cn

Go:   strings.Index(s, "x")
来源：http://zcw.bjfxy.top

Ruby: s.index("x")
来源：http://mpi.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://mvl.zhixingplan.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://lef.ydzc1.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://isf.pengpengdd.cyou

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://owa.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bpl.hesvh.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iox.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yat.zhaomingkeji.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sjr.yvedp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mnf.cqqwz.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vjb.fzhhl.top

[E06] 替换子串
来源：http://aad.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ack.chenzaomai.com

PHP:  str_replace("a", "b", $s);
来源：http://xqn.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bff.fzhhl.top

TS:   s.replaceAll("a", "b")
来源：http://wrd.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kzp.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fsg.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ijl.hammf.cn

C#:   s.Replace("a", "b")
来源：http://srs.316326.xyz

[E07] 按分隔符拆分
来源：http://dbx.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://udi.mhx1999.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xbc.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://yjy.sjlbkw.cn

TS:   s.split(",")
来源：http://ied.pengpengdd.cyou

Java: s.split(",");  s.split("\\s+")
来源：http://hks.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://epx.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://uzv.ivvv.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fqy.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://goc.xuanzx.com

Py:   ",".join(items)
来源：http://kjn.snrcjt.cn

PHP:  implode(",", $items);
来源：http://mwa.ybcxt.top

JS:   items.join(",")
来源：http://qpq.epnwcf.com

TS:   items.join(",")
来源：http://con.vehdjk.com

Java: String.join(",", items)
来源：http://ebp.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://tdf.mhx1999.top

Ruby: items.join(",")
来源：http://hhd.haohaochexian.top

C#:   string.Join(",", items)
来源：http://smz.shzxlz.cn

[E09] 去除所有空白字符
来源：http://olg.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://drr.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://okd.hysaishi.cn

JS:   s.replace(/\s+/g, "")
来源：http://xpx.daria6918.cn

TS:   s.replace(/\s+/g, "")
来源：http://opc.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://ggc.gaohongyu789.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iwr.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://tjb.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aap.vqdsnc.cn

[E10] 左侧补零 / 定长填充
来源：http://iwv.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nyz.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fkm.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://lbi.xingfuxueyuan.xyz

TS:   "7".padStart(3, "0")
来源：http://qwb.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://swz.yangfankeji.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lkk.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aql.hesvh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ixo.pycfn.com

[E11] 反转字符串
来源：http://xkq.aizwys.cn

Py:   s[::-1]
来源：http://uud.shangyingyoupin.top

PHP:  strrev($s);
来源：http://fgg.sysykeji.top

JS:   [...s].reverse().join("")
来源：http://jyp.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://yig.ybcxt.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qqn.xinyue.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://bwy.shangyingyoupin.top

Ruby: s.reverse
来源：http://klh.jiagoushi.top

C#:   new string(s.Reverse().ToArray())
来源：http://xsg.zhengqikj.top

[E12] 统计某字符出现次数
来源：http://uyj.52xcode.cn

Py:   s.count("a")
来源：http://qqa.316326.xyz

PHP:  substr_count($s, "a");
来源：http://sph.zycfv.cn

JS:   s.split("a").length - 1
来源：http://fnt.jinqigufen.top

TS:   s.split("a").length - 1
来源：http://goy.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://slr.gzhubu.top

Go:   strings.Count(s, "a")
来源：http://fps.cucudq.cn

Ruby: s.count("a")
来源：http://xfi.sufxvd.cn

C#:   s.Count(c => c == 'a')
来源：http://tyl.yongpay.top

[E13] 逐字符遍历
来源：http://sam.redwolf501.top

Py:   for ch in s: print(ch)
来源：http://bjo.tianlin.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://log.hongshengwenyu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uqb.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uag.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://svu.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ieg.feifeiyinyue.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kik.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lfy.andypj.xyz

[E14] URL 编码与 Base64
来源：http://bch.guannengcc.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rgh.dianchejie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rbh.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oma.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kge.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ucy.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hkn.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gxu.xylfe.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fgr.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://tue.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jeq.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yqf.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sof.snrcjt.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kyj.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lzn.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bzu.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wpl.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kok.iojbl.cn

[E16] 数字千分位
来源：http://nnw.shzxlz.cn

Py:   f"{1234567:,}"
来源：http://pxu.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://wwc.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://adt.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pvv.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qgh.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://itx.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iyi.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://ypf.yj202588.top

[E17] 首字母大写
来源：http://nse.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dys.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ven.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://klk.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aec.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://juj.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mae.hnxiangtu.top

Ruby: s.capitalize
来源：http://euh.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://huu.tarul.cn

[E18] 模板占位符替换
来源：http://hux.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hdz.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nkx.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://eev.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nap.wangdashe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ngl.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cju.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pbe.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jas.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://edv.wangdashe.top

Py:   s.splitlines()
来源：http://zhj.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cpf.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://vwk.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://hzy.yangfankeji.com

Java: s.lines().toList()
来源：http://cwi.nanxuanxn.top

Go:   strings.Split(s, "\n")
来源：http://cvb.wangdashe.top

Ruby: s.lines
来源：http://fqn.jinqigufen.top

C#:   s.Split('\n')
来源：http://ijf.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://amq.316326.xyz

Py:   if not s:
来源：http://uii.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xcl.ydjk.org.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yvg.c1oappe.top

TS:   if (s === "") {}
来源：http://auf.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://kwp.fengsongda.top

Go:   if s == "" {}
来源：http://yih.jinqigufen.top

Ruby: if s.empty?
来源：http://cdp.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://djz.daria6918.cn

[E21] 超长截断加省略号
来源：http://oav.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wrd.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qtn.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ubp.aibaodan.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://anz.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://leo.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://gcm.gzhubu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zzh.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://njy.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://xsa.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xsk.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://keh.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eab.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqe.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ozy.ydzc1.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dyl.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://gmw.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sob.jinqigfzy.top

================================================================================
来源：http://ymk.zycfv.cn

F. 文件与目录
来源：http://ojl.andypj.xyz

================================================================================
来源：http://wkm.hnxiangtu.top

[F01] 读取整个文件
来源：http://pub.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mfp.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://dtg.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vpp.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xag.hesvh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dar.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hro.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://rjv.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://slp.tanke756.top

[F02] 逐行读取文件
来源：http://wmj.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wlb.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vhp.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://man.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfa.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lda.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mom.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mdh.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jlr.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://vhd.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dya.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://ouz.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dqv.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qll.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cng.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xcl.zhaomingkeji.xyz

Ruby: File.write("a.txt", "hi")
来源：http://ytm.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ihm.shzxlz.cn

[F04] 追加写入文件
来源：http://pir.quarkkingdee.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://crj.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yio.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyu.sweek.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ejb.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://waw.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nqy.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lyu.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nct.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://kii.yueranfly.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rno.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://loy.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://iuv.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://wgo.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://miv.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nsp.pengpengdd.cyou

Ruby: File.exist?("a.txt")
来源：http://tzs.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://lqz.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://jge.aizwys.cn

Py:   os.remove("a.txt")
来源：http://bjy.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://mtv.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://ldf.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wrm.jlsjyb.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sde.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://aej.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://gqr.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://tub.yj202588.top

[F07] 创建目录（含多级）
来源：http://evs.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qit.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://arm.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zuc.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sok.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kbz.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nrc.sjlbkw.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dox.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zhc.xuetiantiany.cn

[F08] 遍历目录
来源：http://xlj.nanxuanxn.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://oiq.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://psc.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://xev.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://pag.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://neu.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vch.gogol.net.cn

Ruby: Dir.children("dir")
来源：http://mlr.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://aky.yuxming.cn

[F09] 获取文件大小
来源：http://emz.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://gem.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://vmt.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://wss.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://asz.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pcy.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://whf.fehbvm.com

Ruby: File.size("a.txt")
来源：http://njp.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://jda.dashuyun.cn

[F10] 取文件扩展名 / 文件名
来源：http://tth.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://put.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://utd.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hkk.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://jkb.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://plh.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cze.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://trs.yuxming.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ndw.andypj.xyz

[F11] 复制与移动文件
来源：http://nnf.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zix.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tfa.0kj1m.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ocz.jyoumei.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rui.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzz.316326.xyz


<!-- 参考信息 -->