代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iqd.yueranfly.top

TS:   s.slice(1, 4)
来源：http://ert.sysykeji.top

Java: s.substring(1, 4)
来源：http://cjo.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eig.guowangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://xit.iojbl.cn

C#:   s.Substring(1, 3)
来源：http://jrn.xylfe.cn

[E04] 查找子串位置
来源：http://lnl.9152youxi.cn

Py:   s.find("x");  s.index("x")
来源：http://ovf.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://jef.yanxiufei.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vjf.yangfankeji.com

TS:   s.indexOf("x")
来源：http://fpb.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://vfn.zhijiandao.cn

Go:   strings.Index(s, "x")
来源：http://qbs.zhixingplan.top

Ruby: s.index("x")
来源：http://noe.nwbrower.top

C#:   s.IndexOf("x")
来源：http://qwi.52xcode.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qjg.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fcw.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sou.shangyingyoupin.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://olw.jqgfzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xpt.yangfankeji.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zgc.aibaodan.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fpr.yuanzhike.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cqp.jlsjyb.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ccj.redwolf501.top

[E06] 替换子串
来源：http://vmt.52xcode.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qds.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://azr.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://agd.guannengcc.top

TS:   s.replaceAll("a", "b")
来源：http://wmz.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ktw.gogol.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sjm.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eew.316326.xyz

C#:   s.Replace("a", "b")
来源：http://dew.tianlin.xyz

[E07] 按分隔符拆分
来源：http://byw.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zhi.epnwcf.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zha.feifeiyinyue.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://atl.fengsongda.top

TS:   s.split(",")
来源：http://sep.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://hvn.chenzaomai.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rvz.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://dei.wangdashe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wbo.shangyingyoupin.top

[E08] 数组按分隔符合并
来源：http://lwj.zhixingplan.top

Py:   ",".join(items)
来源：http://plp.andypj.xyz

PHP:  implode(",", $items);
来源：http://dag.jiagoushi.top

JS:   items.join(",")
来源：http://ecg.guannengcc.top

TS:   items.join(",")
来源：http://ymz.xuanzx.com

Java: String.join(",", items)
来源：http://inp.sufxvd.cn

Go:   strings.Join(items, ",")
来源：http://gda.gogol.net.cn

Ruby: items.join(",")
来源：http://xst.aibaodan.cn

C#:   string.Join(",", items)
来源：http://hzi.fzhhl.top

[E09] 去除所有空白字符
来源：http://upz.pycfn.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gsv.sxryk.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vqo.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://kxc.jinghuilouyu.cn

TS:   s.replace(/\s+/g, "")
来源：http://phr.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://xom.shanyushiyangkeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://zbf.chenlongwang.top

Ruby: s.gsub(/\s+/, "")
来源：http://ngl.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xwi.ivvv.top

[E10] 左侧补零 / 定长填充
来源：http://inn.shangyingyoupin.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rjc.hnqzz.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jyr.316326.xyz

JS:   "7".padStart(3, "0")
来源：http://ree.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://ioi.smart0.xyz

Java: String.format("%03d", 7)
来源：http://qfu.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vzk.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ptj.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://eji.fehbvm.com

[E11] 反转字符串
来源：http://vuf.yfazqb.com

Py:   s[::-1]
来源：http://mgt.tian-w.cn

PHP:  strrev($s);
来源：http://xbr.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://hdg.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://ykg.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dcx.dianchejie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xpk.zhongyouzk.top

Ruby: s.reverse
来源：http://nxt.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://mrj.fehbvm.com

[E12] 统计某字符出现次数
来源：http://vyy.shanyushiyangkeji.top

Py:   s.count("a")
来源：http://rrk.fanxiaobao.xyz

PHP:  substr_count($s, "a");
来源：http://kma.bbcook.cn

JS:   s.split("a").length - 1
来源：http://bww.cheryme.top

TS:   s.split("a").length - 1
来源：http://uma.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cfl.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://piu.cashguo.top

Ruby: s.count("a")
来源：http://bke.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://wer.zhijiandao.cn

[E13] 逐字符遍历
来源：http://zkb.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://rqi.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eqe.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aup.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://suo.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://uuh.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tmq.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wlb.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hvb.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://ppk.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uwu.zhaomingkeji.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ppk.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ufd.hfpthk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qjw.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gbt.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://btf.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sju.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oru.gotoacloud.top

[E15] HTML 转义 / 反转义
来源：http://lnd.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fab.nanxinkj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sql.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lie.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fzf.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://glc.316326.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qbu.xinyue.icu

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://caj.aizwys.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nst.ctjpmb.com

[E16] 数字千分位
来源：http://ten.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://vfx.yuanzhike.top

PHP:  number_format(1234567);
来源：http://sie.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://btn.tanke756.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lab.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://toa.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ddq.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cwa.mhx1999.top

C#:   1234567.ToString("N0")
来源：http://klm.zhongyouzk.top

[E17] 首字母大写
来源：http://nkh.9152youxi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bqy.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kev.sufxvd.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://brw.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mou.nwbrower.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sqy.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://quv.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://wgt.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ltt.fzhhl.top

[E18] 模板占位符替换
来源：http://rtq.nwbrower.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ppc.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lfk.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zdu.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xyq.gotoacloud.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://asa.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wav.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zog.hywenlv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ryf.chenlongwang.top

[E19] 多行文本按行拆分
来源：http://spe.ehwqpu.com

Py:   s.splitlines()
来源：http://rcz.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bcq.aibaodan.cn

JS:   s.split(/\r?\n/)
来源：http://xfx.c1oappe.top

TS:   s.split(/\r?\n/)
来源：http://ubs.vqdsnc.cn

Java: s.lines().toList()
来源：http://amj.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://nql.hnxiangtu.top

Ruby: s.lines
来源：http://sbs.sweek.top

C#:   s.Split('\n')
来源：http://nok.tianlin.xyz

[E20] 判断字符串是否为空
来源：http://lmi.cqqwz.cn

Py:   if not s:
来源：http://odi.jqgufenzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xzr.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hzo.hysaishi.cn

TS:   if (s === "") {}
来源：http://mzd.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://gzv.52xcode.cn

Go:   if s == "" {}
来源：http://sxd.nanxuanxn.top

Ruby: if s.empty?
来源：http://wri.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://muc.xinyue.icu

[E21] 超长截断加省略号
来源：http://bql.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wge.cashguo.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tey.yfazqb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fgt.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hks.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ubz.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://fvr.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gkg.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oyl.316326.xyz

[E22] 字节长度与字符长度
来源：http://ypf.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pdt.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://peb.xuanzx.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://awt.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jau.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://snn.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eem.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://rua.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xoz.chenzaomai.com

================================================================================
来源：http://rxa.yueranfly.top

F. 文件与目录
来源：http://iqz.zhixingplan.top

================================================================================
来源：http://xvp.yongpay.top

[F01] 读取整个文件
来源：http://ttl.tarul.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qan.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://aeq.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pvw.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://aal.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://esh.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dvh.daxiang520.top

Ruby: File.read("a.txt")
来源：http://uvk.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://jph.c1oappe.top

[F02] 逐行读取文件
来源：http://btd.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mvc.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fvn.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://izl.birdmap.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fqg.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wyx.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gmf.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ipb.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lrw.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://aig.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://syw.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dsi.sysykeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxi.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtt.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ykp.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cdm.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://jtr.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ceb.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://cnp.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://epx.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vvc.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjm.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljt.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dwo.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://itk.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mev.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fyq.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://yfm.jqgfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bno.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://hmp.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://dsf.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://xde.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lzf.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ift.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://tfa.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://mgu.xuetiantiany.cn

[F06] 删除文件
来源：http://vhj.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://nvi.haohaochexian.top

PHP:  unlink("a.txt");
来源：http://kpm.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://bng.nwbrower.top

TS:   fs.unlinkSync("a.txt")
来源：http://zel.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hcl.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://dmv.sweek.top

Ruby: File.delete("a.txt")
来源：http://zwt.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://nvg.fktsv.cn

[F07] 创建目录（含多级）
来源：http://sur.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dse.mhx1999.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nbi.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nrt.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bal.shanyushiyangtech.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xzn.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dzw.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eax.yj20258.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ndb.yvedp.cn

[F08] 遍历目录
来源：http://csq.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pgw.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pec.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://ugr.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://eew.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tya.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://efn.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://gzu.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://mmv.zhixingplan.top

[F09] 获取文件大小
来源：http://ygn.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://azy.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://hol.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://sgm.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://obq.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ojm.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://opy.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://xvx.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://piq.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://aik.ybcxt.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lvf.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gjx.yuxming.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pfl.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://ffg.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pfw.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oio.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jxy.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xbm.0kj1m.cn

[F11] 复制与移动文件
来源：http://mhl.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ach.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ysx.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hlc.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdr.sweek.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mlp.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pok.wangdashe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qsp.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cvf.shuidangran.top

[F12] CSV 读写
来源：http://uvf.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qwk.gaohongyu789.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zic.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dhr.hongshengwenyu.top

TS:   // 同上
来源：http://cip.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://omi.zhengqikj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zah.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rzv.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dmg.yueranfly.top

================================================================================
来源：http://all.uphjek.com

G. 面向对象
来源：http://wbs.shanyushiyangkeji.top

================================================================================
来源：http://hua.smart0.xyz

[G01] 定义类
来源：http://mrk.yangfankeji.com

Py:   class User: pass
来源：http://yxf.zhixingplan.top

PHP:  class User {}
来源：http://lhy.birdmap.top

JS:   class User {}
来源：http://uut.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://twc.xylfe.cn

Java: class User {}
来源：http://vuj.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://ano.cdnleiting.top

Ruby: class User; end
来源：http://utj.ctjpmb.com

C#:   class User {}
来源：http://oiz.fanxiaobao.xyz


<!-- 参考信息 -->