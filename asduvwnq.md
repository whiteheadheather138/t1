代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://oou.chenjidiqi.icu

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oqx.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cie.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ymb.xuetiantiany.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://via.sysykeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ndu.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oyh.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zul.chenjidiqi.icu

[E02] 重复字符串
来源：http://hyh.ctjpmb.com

Py:   "ab" * 3
来源：http://ujj.pengpengdd.cyou

PHP:  str_repeat("ab", 3);
来源：http://gyx.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://bdl.chenlongwang.top

TS:   "ab".repeat(3)
来源：http://bgp.pengpengdd.cyou

Java: "ab".repeat(3)
来源：http://izg.pengpengdd.cyou

Go:   strings.Repeat("ab", 3)
来源：http://ucj.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://fyc.sufxvd.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zjg.quarkkingdee.top

[E03] 截取子串
来源：http://pgy.ywan-chungtsiang.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nhm.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://odz.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ish.zdqjudy.top

TS:   s.slice(1, 4)
来源：http://lul.wangshuangyany.cn

Java: s.substring(1, 4)
来源：http://dxs.sufxvd.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vej.feifeiyinyue.top

Ruby: s[1, 3];  s[1..3]
来源：http://zvb.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://iek.zdbjq.cn

[E04] 查找子串位置
来源：http://fhb.xinyue.icu

Py:   s.find("x");  s.index("x")
来源：http://zqc.kuanghao11.cn

PHP:  strpos($s, "x");
来源：http://esd.aizwys.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://igg.mhx1999.top

TS:   s.indexOf("x")
来源：http://dly.chenzaomai.com

Java: s.indexOf("x")
来源：http://ffp.sweek.top

Go:   strings.Index(s, "x")
来源：http://umw.ydjk.org.cn

Ruby: s.index("x")
来源：http://vug.xziqi.cn

C#:   s.IndexOf("x")
来源：http://vvt.nanxuanxn.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://ysm.hcnkem.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xwh.hnqzz.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yuf.nanxuanxn.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yez.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mqn.yuxming.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rfs.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rbu.daria6918.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://smw.chenjidiqi.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fji.yanxiufei.cn

[E06] 替换子串
来源：http://khe.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ryb.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://jvm.hfpthk.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zgz.nanxinkj.top

TS:   s.replaceAll("a", "b")
来源：http://ouv.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ygo.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uyn.haohaochexian.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qrx.tianlin.xyz

C#:   s.Replace("a", "b")
来源：http://znj.vehdjk.com

[E07] 按分隔符拆分
来源：http://pbo.meibo888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jsj.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zjc.yonumen.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tky.yfazqb.com

TS:   s.split(",")
来源：http://bph.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://wse.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ylv.tarul.cn

Ruby: s.split(",");  s.split
来源：http://fmo.tian-w.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://owx.ydzc1.top

[E08] 数组按分隔符合并
来源：http://zjv.ivvv.top

Py:   ",".join(items)
来源：http://dpy.zhongyouzk.top

PHP:  implode(",", $items);
来源：http://xvx.yvedp.cn

JS:   items.join(",")
来源：http://aas.c1oappe.top

TS:   items.join(",")
来源：http://rqo.c1oappe.top

Java: String.join(",", items)
来源：http://owp.zhiwuduotai.top

Go:   strings.Join(items, ",")
来源：http://xay.fzhhl.top

Ruby: items.join(",")
来源：http://ghf.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://cps.sufxvd.cn

[E09] 去除所有空白字符
来源：http://qhj.wangshuangyany.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ead.ivvv.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rvv.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://nue.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://lmf.dashuyun.cn

Java: s.replaceAll("\\s+", "")
来源：http://trm.feifeiyinyue.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://aqa.zycfv.cn

Ruby: s.gsub(/\s+/, "")
来源：http://tsn.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usw.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://fzs.yvedp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://heo.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tpl.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://igh.birdmap.top

TS:   "7".padStart(3, "0")
来源：http://rhf.gzhubu.top

Java: String.format("%03d", 7)
来源：http://prn.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://est.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gjm.gogol.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yjh.sysykeji.top

[E11] 反转字符串
来源：http://jwq.aibaodan.cn

Py:   s[::-1]
来源：http://qwa.guannengcc.top

PHP:  strrev($s);
来源：http://fqr.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://wvy.xuetiantiany.cn

TS:   [...s].reverse().join("")
来源：http://atk.cashguo.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bka.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pez.vqdsnc.cn

Ruby: s.reverse
来源：http://kxe.ybcxt.top

C#:   new string(s.Reverse().ToArray())
来源：http://bfx.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://lcu.chenlongwang.top

Py:   s.count("a")
来源：http://dfz.yj202588.top

PHP:  substr_count($s, "a");
来源：http://atx.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://cdg.hammf.cn

TS:   s.split("a").length - 1
来源：http://ute.xylfe.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vpg.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://ldl.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://tys.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://efu.pengpengdd.cyou

[E13] 逐字符遍历
来源：http://pan.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://rzu.ydjk.org.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nhj.yonumen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rou.xziqi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vhe.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xcm.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dtu.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://izv.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bpw.ppjwa.cn

[E14] URL 编码与 Base64
来源：http://zty.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zhe.hywenlv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jdp.chenjidiqi.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://meg.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ypm.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kaz.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bzc.gotoacloud.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dlu.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qec.jinqigufen.top

[E15] HTML 转义 / 反转义
来源：http://rvh.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qti.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pqk.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hup.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nvr.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tyy.daria6918.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ykw.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://myx.chenlongwang.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xyu.mhx1999.top

[E16] 数字千分位
来源：http://dui.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://pqr.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://cqf.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ojx.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://xjs.pycfn.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ipc.sxryk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eqq.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lsp.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://qqo.shangyingyoupin.top

[E17] 首字母大写
来源：http://ruc.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zgz.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ukc.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ypk.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nid.hnxiangtu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://noj.zdqjudy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zjf.sxryk.cn

Ruby: s.capitalize
来源：http://eux.c1oappe.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lwf.vqdsnc.cn

[E18] 模板占位符替换
来源：http://kzo.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rog.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ydf.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jms.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://edz.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://twv.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kkv.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://byl.tian-w.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oge.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://kwl.yvedp.cn

Py:   s.splitlines()
来源：http://dxh.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mnd.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://kae.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://qka.yfazqb.com

Java: s.lines().toList()
来源：http://kuq.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://ulp.tian-w.cn

Ruby: s.lines
来源：http://zmi.jinqigfzy.top

C#:   s.Split('\n')
来源：http://aus.zycfv.cn

[E20] 判断字符串是否为空
来源：http://psf.316326.xyz

Py:   if not s:
来源：http://gst.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qah.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nlo.svipenyu.cn

TS:   if (s === "") {}
来源：http://yso.jiagoushi.top

Java: if (s.isEmpty()) {}
来源：http://etr.hammf.cn

Go:   if s == "" {}
来源：http://pac.ehwqpu.com

Ruby: if s.empty?
来源：http://wvs.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lce.gotoacloud.top

[E21] 超长截断加省略号
来源：http://wrw.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://obt.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zrg.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fyu.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zvb.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hix.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://xom.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nas.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hcn.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://rau.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xup.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pvd.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkx.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwy.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yiw.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lvc.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://gup.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cwy.nanxinkj.top

================================================================================
来源：http://aeq.kuanghao11.cn

F. 文件与目录
来源：http://wfn.chenlongwang.top

================================================================================
来源：http://drh.sxryk.cn

[F01] 读取整个文件
来源：http://mxw.iojbl.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lrd.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://rmd.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://htr.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ngx.pengpengdd.cyou

Java: Files.readString(Path.of("a.txt"))
来源：http://bld.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://upp.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://ryt.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://eva.yonumen.top

[F02] 逐行读取文件
来源：http://cbq.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://byk.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jfc.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcy.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aoz.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fbx.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hms.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xlt.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dna.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://okb.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rxg.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vxe.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqq.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sqc.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ucz.jinghuilouyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ezu.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://vpu.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gal.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://kzk.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vak.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vbc.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://smo.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qta.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pca.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vwi.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tpx.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ywk.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://ykg.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gku.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://pfc.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://xqt.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://hte.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zwo.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uae.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://bly.yuxming.cn

C#:   File.Exists("a.txt")
来源：http://dmz.zhongyouzk.top

[F06] 删除文件
来源：http://sie.cashguo.top

Py:   os.remove("a.txt")
来源：http://oxs.vehdjk.com

PHP:  unlink("a.txt");
来源：http://dfd.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jqb.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uge.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://teo.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://fin.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://ucu.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://tvo.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://tga.cdnleiting.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://diu.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fcd.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvo.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lkc.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ooi.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bwy.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sqw.yj202588.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://krz.dianchejie.cn

[F08] 遍历目录
来源：http://lai.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ksc.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nxs.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://ulq.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://vbh.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wsa.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ezm.gaohongyu789.top

Ruby: Dir.children("dir")
来源：http://fwf.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://tij.0kj1m.cn

[F09] 获取文件大小
来源：http://kwg.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://eaz.nwbrower.top

PHP:  filesize("a.txt");
来源：http://zxc.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://xgj.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://ywj.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://dth.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ktn.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://von.sxryk.cn

C#:   new FileInfo("a.txt").Length
来源：http://whj.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://kha.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ama.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fqv.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://imp.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://zvu.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wfu.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cgr.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://axe.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://djx.aibaodan.cn

[F11] 复制与移动文件
来源：http://ngc.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zre.yongpay.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://idr.yuanzhike.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cfg.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rwi.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cln.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iew.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sma.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccv.redwolf501.top

[F12] CSV 读写
来源：http://tfl.hnxiangtu.top


<!-- 参考信息 -->