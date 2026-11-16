代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qth.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gqg.zhengqikj.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bod.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uif.xylfe.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ztx.aizwys.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://phj.feifeiyinyue.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jdj.fengsongda.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jhh.dashuyun.cn

[E02] 重复字符串
来源：http://ydn.mhx1999.top

Py:   "ab" * 3
来源：http://lsx.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://atb.xuanzx.com

JS:   "ab".repeat(3)
来源：http://zum.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://ubj.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://yye.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://nvd.hongshengwenyu.top

Ruby: "ab" * 3
来源：http://mfj.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jyr.gogol.net.cn

[E03] 截取子串
来源：http://cge.yfazqb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sui.ydjk.org.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://csk.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zgi.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://yej.c1oappe.top

Java: s.substring(1, 4)
来源：http://kns.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wre.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://izy.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://zzm.zhiwuduotai.top

[E04] 查找子串位置
来源：http://npq.chenlongwang.top

Py:   s.find("x");  s.index("x")
来源：http://xwf.zhongyouzk.top

PHP:  strpos($s, "x");
来源：http://jii.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qyq.hysaishi.cn

TS:   s.indexOf("x")
来源：http://vlg.meibo888.top

Java: s.indexOf("x")
来源：http://vem.epnwcf.com

Go:   strings.Index(s, "x")
来源：http://zlk.snrcjt.cn

Ruby: s.index("x")
来源：http://wnl.sjlbkw.cn

C#:   s.IndexOf("x")
来源：http://ftv.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://buh.cqqwz.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tmz.yangfankeji.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dje.yfazqb.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aku.nanxuanxn.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nqr.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rpw.jianghu66.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kng.wangshuangyany.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wti.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rvu.hesvh.cn

[E06] 替换子串
来源：http://jyo.yanxiufei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jzl.feifeiyinyue.top

PHP:  str_replace("a", "b", $s);
来源：http://afd.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ovw.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://jgi.hammf.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jqt.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ljk.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xmd.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://bhr.hcnkem.com

[E07] 按分隔符拆分
来源：http://hqt.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tnd.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dwi.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kwb.ivvv.top

TS:   s.split(",")
来源：http://afp.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bud.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://paz.shangyingyoupin.top

Ruby: s.split(",");  s.split
来源：http://geh.quarkkingdee.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lef.redwolf501.top

[E08] 数组按分隔符合并
来源：http://iih.fanxiaobao.xyz

Py:   ",".join(items)
来源：http://twc.xziqi.cn

PHP:  implode(",", $items);
来源：http://rkv.aibaodan.cn

JS:   items.join(",")
来源：http://chl.yj20258.top

TS:   items.join(",")
来源：http://tbw.52xcode.cn

Java: String.join(",", items)
来源：http://qad.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://rph.gogol.net.cn

Ruby: items.join(",")
来源：http://aek.ivvv.top

C#:   string.Join(",", items)
来源：http://qqf.svipenyu.cn

[E09] 去除所有空白字符
来源：http://cnc.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://txx.chenjidiqi.icu

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gtg.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://vcl.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://yvr.daxiang520.top

Java: s.replaceAll("\\s+", "")
来源：http://jsm.zhaomingkeji.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://pkb.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wzw.iojbl.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tsc.cdnleiting.top

[E10] 左侧补零 / 定长填充
来源：http://vyv.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tua.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wrs.9152youxi.cn

JS:   "7".padStart(3, "0")
来源：http://uir.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://tuy.nanxinkj.top

Java: String.format("%03d", 7)
来源：http://mig.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fpe.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rmi.cheryme.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mxc.jqgfzy.top

[E11] 反转字符串
来源：http://flv.jinyuanbaomall.cn

Py:   s[::-1]
来源：http://vcg.zhongyouzk.top

PHP:  strrev($s);
来源：http://fmi.ybcxt.top

JS:   [...s].reverse().join("")
来源：http://exl.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://nrh.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://fds.0kj1m.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pyr.yvedp.cn

Ruby: s.reverse
来源：http://aee.jlsjyb.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xsc.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://cil.yuanzhike.top

Py:   s.count("a")
来源：http://vws.haohaochexian.top

PHP:  substr_count($s, "a");
来源：http://tuj.yfazqb.com

JS:   s.split("a").length - 1
来源：http://qxu.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://bif.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://nwk.jiagoushi.top

Go:   strings.Count(s, "a")
来源：http://rdd.ehwqpu.com

Ruby: s.count("a")
来源：http://fxf.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://qwc.nanxinkj.top

[E13] 逐字符遍历
来源：http://wvz.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://hkp.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lse.hfpthk.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lci.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jgp.meibo888.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cnn.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cfj.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wbo.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wve.sysykeji.top

[E14] URL 编码与 Base64
来源：http://ghh.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wme.chenlongwang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://cyq.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://khd.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rji.jianghu66.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cnf.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nbf.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sme.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gcw.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://wac.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dpg.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wpj.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fgk.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dqk.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ctz.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhw.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jjo.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hdz.hcnkem.com

[E16] 数字千分位
来源：http://rfx.bbcook.cn

Py:   f"{1234567:,}"
来源：http://xgg.xinyue.icu

PHP:  number_format(1234567);
来源：http://xoz.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ekl.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kwx.wangdashe.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kkp.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bdn.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xxj.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://gqn.daria6918.cn

[E17] 首字母大写
来源：http://ehw.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dzw.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ccx.yj20258888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://akm.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dzw.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fjl.yj20258888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dqc.feifeiyinyue.top

Ruby: s.capitalize
来源：http://keu.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xoc.kuanghao11.cn

[E18] 模板占位符替换
来源：http://lhx.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xkz.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ope.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lfo.jinqigfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://irp.meibo888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mvl.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mlo.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zmh.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ghz.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://tsn.hammf.cn

Py:   s.splitlines()
来源：http://foa.quarkkingdee.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qqd.xziqi.cn

JS:   s.split(/\r?\n/)
来源：http://hjo.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://sdq.nanxinkj.top

Java: s.lines().toList()
来源：http://mqy.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://jsw.xylfe.cn

Ruby: s.lines
来源：http://tmb.yj20258888.top

C#:   s.Split('\n')
来源：http://fuz.gaohongyu789.top

[E20] 判断字符串是否为空
来源：http://dur.yuanzhike.top

Py:   if not s:
来源：http://mpz.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xvs.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lca.snrcjt.cn

TS:   if (s === "") {}
来源：http://iak.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://elt.jinqigufen.top

Go:   if s == "" {}
来源：http://wnl.tian-w.cn

Ruby: if s.empty?
来源：http://wts.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tie.chenzaomai.com

[E21] 超长截断加省略号
来源：http://uhm.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kuz.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kib.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qbw.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kyg.yuxming.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wdg.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://uyt.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qha.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hvv.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://sbk.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wyn.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hon.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://den.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://quq.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iex.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vxv.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://yel.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ywu.iojbl.cn

================================================================================
来源：http://blg.daxiang520.top

F. 文件与目录
来源：http://krh.yj20258.top

================================================================================
来源：http://iqv.snrcjt.cn

[F01] 读取整个文件
来源：http://zij.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pqj.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://aki.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lre.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jcj.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xea.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lhd.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://qzm.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://fzn.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://wms.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://szc.sufxvd.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dgw.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhc.yj202588.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxr.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://szf.xuanzx.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rdf.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://izq.tarul.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nnr.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://ivw.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jaq.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lpp.yfazqb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epe.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xme.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jfe.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvb.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://rwh.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lmw.yj202588.top

[F04] 追加写入文件
来源：http://ykn.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgb.zhongyouzk.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vka.yanxiufei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bfb.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kts.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mjj.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fnp.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hvz.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yqh.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://xdr.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hyg.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://hws.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://frg.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://xgr.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sak.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://orx.meibo888.top

Ruby: File.exist?("a.txt")
来源：http://czw.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://brk.zhixingplan.top

[F06] 删除文件
来源：http://nhu.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://gpb.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://auk.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://kqh.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hay.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://khf.cashguo.top

Go:   os.Remove("a.txt")
来源：http://gjd.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://xlx.redwolf501.top

C#:   File.Delete("a.txt");
来源：http://fvo.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://cqv.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wzx.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mas.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yox.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vzo.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cwn.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fpx.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xxk.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aca.yueranfly.top

[F08] 遍历目录
来源：http://nqh.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vwl.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vvi.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://pnt.xingfuxueyuan.xyz

TS:   fs.readdirSync("dir")
来源：http://prp.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://igy.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fnj.pycfn.com

Ruby: Dir.children("dir")
来源：http://qjf.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://efj.cqqwz.cn

[F09] 获取文件大小
来源：http://byk.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://kuj.epnwcf.com

PHP:  filesize("a.txt");
来源：http://pry.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://hyf.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://cwx.xuanzx.com

Java: Files.size(Path.of("a.txt"))
来源：http://fjj.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://itr.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://gxl.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://hue.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://tht.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://udq.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tlr.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qjy.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://zxh.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rwv.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bpk.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://srs.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://omj.gotoacloud.top

[F11] 复制与移动文件
来源：http://dxp.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ixr.mhx1999.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uli.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gbr.zhijiandao.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ndc.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xfs.zycfv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://inv.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sxq.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://llv.zhixingplan.top

[F12] CSV 读写
来源：http://fxm.xziqi.cn


<!-- 参考信息 -->