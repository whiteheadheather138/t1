代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wuu.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ryq.ctjpmb.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vtx.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zxf.ywan-chungtsiang.top

[E02] 重复字符串
来源：http://ihn.haohaochexian.top

Py:   "ab" * 3
来源：http://jxw.zdqjudy.top

PHP:  str_repeat("ab", 3);
来源：http://mkd.chenzaomai.com

JS:   "ab".repeat(3)
来源：http://iho.jianghu66.top

TS:   "ab".repeat(3)
来源：http://yck.pycfn.com

Java: "ab".repeat(3)
来源：http://msv.shanyushiyangtech.top

Go:   strings.Repeat("ab", 3)
来源：http://idp.yueranfly.top

Ruby: "ab" * 3
来源：http://ncl.fzhhl.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rwv.jinqigfzy.top

[E03] 截取子串
来源：http://mvz.pengpengdd.cyou

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lrr.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cwx.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lrw.tian-w.cn

TS:   s.slice(1, 4)
来源：http://jxb.nwbrower.top

Java: s.substring(1, 4)
来源：http://hns.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wek.zhoulong.xyz

Ruby: s[1, 3];  s[1..3]
来源：http://afm.ybcxt.top

C#:   s.Substring(1, 3)
来源：http://gmn.xziqi.cn

[E04] 查找子串位置
来源：http://jvg.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://ieb.fktsv.cn

PHP:  strpos($s, "x");
来源：http://vmr.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iro.hnxiangtu.top

TS:   s.indexOf("x")
来源：http://qku.jiagoushi.top

Java: s.indexOf("x")
来源：http://kol.quarkkingdee.top

Go:   strings.Index(s, "x")
来源：http://vql.yj20258888.top

Ruby: s.index("x")
来源：http://cvk.zhaomingkeji.xyz

C#:   s.IndexOf("x")
来源：http://nrr.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://jlf.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gnq.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://biq.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://trf.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ebi.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://phu.nanxuanxn.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bzc.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jnc.jqgfzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tbn.hywenlv.cn

[E06] 替换子串
来源：http://ufk.zycfv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qyx.xuanzx.com

PHP:  str_replace("a", "b", $s);
来源：http://zkk.hywenlv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cmf.zhixingplan.top

TS:   s.replaceAll("a", "b")
来源：http://jeu.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjp.dashuyun.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ysv.havefunace.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cvs.xziqi.cn

C#:   s.Replace("a", "b")
来源：http://ols.nanxuanxn.top

[E07] 按分隔符拆分
来源：http://nnh.yj20258888.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nyz.jqgufenzy.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vrv.hnqzz.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kgw.0kj1m.cn

TS:   s.split(",")
来源：http://ahw.jqgfzy.top

Java: s.split(",");  s.split("\\s+")
来源：http://ecw.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gig.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://kss.zhoulong.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wuz.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://hlz.shanyushiyangtech.top

Py:   ",".join(items)
来源：http://ikq.yuanzhike.top

PHP:  implode(",", $items);
来源：http://pcy.gotoacloud.top

JS:   items.join(",")
来源：http://czu.tian-w.cn

TS:   items.join(",")
来源：http://mpr.iojbl.cn

Java: String.join(",", items)
来源：http://joz.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://fse.yuxming.cn

Ruby: items.join(",")
来源：http://cpg.jyoumei.cn

C#:   string.Join(",", items)
来源：http://nos.fengsongda.top

[E09] 去除所有空白字符
来源：http://fec.hywenlv.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vba.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pbk.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://gra.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://roy.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://xdk.xuanzx.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ajh.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zxo.316326.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vri.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://frd.iojbl.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ild.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zne.jinqigfzy.top

JS:   "7".padStart(3, "0")
来源：http://rje.9152youxi.cn

TS:   "7".padStart(3, "0")
来源：http://eun.guowangkeji.top

Java: String.format("%03d", 7)
来源：http://uhz.nwbrower.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zsh.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rjc.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sjo.uphjek.com

[E11] 反转字符串
来源：http://pvy.hywenlv.cn

Py:   s[::-1]
来源：http://ohq.zhengqikj.top

PHP:  strrev($s);
来源：http://vhd.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://swt.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://zti.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://lmv.hesvh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://apy.0kj1m.cn

Ruby: s.reverse
来源：http://nyp.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vjg.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://zkx.dianchejie.cn

Py:   s.count("a")
来源：http://iec.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://gfq.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://fnj.sweek.top

TS:   s.split("a").length - 1
来源：http://znn.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jyy.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://pia.jqgufenzy.top

Ruby: s.count("a")
来源：http://dzg.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://kjf.xziqi.cn

[E13] 逐字符遍历
来源：http://dwm.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://smr.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cxb.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uhp.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vsv.sysykeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ctz.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ify.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yhc.cheryme.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://frj.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://vso.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nfm.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fvy.fehbvm.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uky.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ewv.xziqi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://edc.dashuyun.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sti.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nnr.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hgo.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://ojq.zhixingplan.top

Py:   html.escape(s);  html.unescape(s)
来源：http://anv.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qox.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ckg.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aev.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xmx.jqgufenzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kax.cucudq.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dmh.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hym.gaohongyu789.top

[E16] 数字千分位
来源：http://pyz.yvedp.cn

Py:   f"{1234567:,}"
来源：http://qis.316326.xyz

PHP:  number_format(1234567);
来源：http://fwn.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nup.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://hxl.shuidangran.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rxl.wangshuangyany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fwg.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qif.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://ocj.fktsv.cn

[E17] 首字母大写
来源：http://rso.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gpe.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://twx.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gqk.zhaomingkeji.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xvp.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zrv.vqdsnc.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zcw.ydzc1.top

Ruby: s.capitalize
来源：http://esa.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rqa.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://ykq.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eyo.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tdj.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oun.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dqc.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vuo.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kcz.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fhm.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mkd.sweek.top

[E19] 多行文本按行拆分
来源：http://ozo.hongshengwenyu.top

Py:   s.splitlines()
来源：http://jcz.316326.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xyw.redwolf501.top

JS:   s.split(/\r?\n/)
来源：http://qwo.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://zim.fehbvm.com

Java: s.lines().toList()
来源：http://hqs.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://xvc.ywan-chungtsiang.top

Ruby: s.lines
来源：http://pyo.zycfv.cn

C#:   s.Split('\n')
来源：http://sqy.ywan-chungtsiang.top

[E20] 判断字符串是否为空
来源：http://izg.316326.xyz

Py:   if not s:
来源：http://kye.bbcook.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mre.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vzo.jyoumei.cn

TS:   if (s === "") {}
来源：http://hhl.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://cvk.svipenyu.cn

Go:   if s == "" {}
来源：http://kbj.cucudq.cn

Ruby: if s.empty?
来源：http://biq.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ewt.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://lhr.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://paz.yuanzhike.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xyq.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://chj.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://odl.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ftx.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://wsv.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qir.fktsv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mtl.ydzc1.top

[E22] 字节长度与字符长度
来源：http://xsu.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vmv.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rkm.yonumen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfh.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wjn.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ukw.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ovh.mhx1999.top

Ruby: s.bytesize;  s.length
来源：http://tzz.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://awc.ctjpmb.com

================================================================================
来源：http://vzx.jianghu66.top

F. 文件与目录
来源：http://rws.ydjk.org.cn

================================================================================
来源：http://ysn.nanxinkj.top

[F01] 读取整个文件
来源：http://zji.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hrr.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://qwr.hesvh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bll.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bpj.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://snl.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cti.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://eww.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://frb.chenlongwang.top

[F02] 逐行读取文件
来源：http://pij.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wju.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jbi.zhijiandao.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uxq.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pzk.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qcm.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nwf.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://drg.fengsongda.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kgw.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://ghk.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dsi.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://afr.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvf.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fap.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wbv.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://saw.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://afq.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pxr.mhx1999.top

[F04] 追加写入文件
来源：http://mwj.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://une.redwolf501.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ikj.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ily.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ukh.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kcx.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rvk.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qqt.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://afe.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://ceq.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nyl.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://smo.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://xom.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://ilq.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ejx.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bcq.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://nxe.fktsv.cn

C#:   File.Exists("a.txt")
来源：http://jkm.hnxiangtu.top

[F06] 删除文件
来源：http://saw.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://sys.aibaodan.cn

PHP:  unlink("a.txt");
来源：http://hve.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://yjv.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lmm.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bow.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://gng.0kj1m.cn

Ruby: File.delete("a.txt")
来源：http://nvy.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://lei.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://cyt.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uin.smart0.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ycs.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tkq.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfr.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://arn.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tvi.vehdjk.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eop.iojbl.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uwr.nanxinkj.top

[F08] 遍历目录
来源：http://jpl.hnqzz.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hol.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://otf.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://pxn.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://xkx.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dvm.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sov.yj20258.top

Ruby: Dir.children("dir")
来源：http://mvj.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://pzp.jqgfzy.top

[F09] 获取文件大小
来源：http://rsj.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://cyk.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://jpf.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://ano.yanxiufei.cn

TS:   fs.statSync("a.txt").size
来源：http://tew.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://hpx.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oel.yfazqb.com

Ruby: File.size("a.txt")
来源：http://gtx.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://akb.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ata.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://clm.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://von.shangyingyoupin.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lfq.chenlongwang.top

TS:   path.extname("a.txt")
来源：http://pyx.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://caa.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oud.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://imv.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sno.aibaodan.cn

[F11] 复制与移动文件
来源：http://hby.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ewh.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://isu.shanyushiyangtech.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qbi.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vxn.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kqw.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fpp.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://buc.9152youxi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wgu.cashguo.top

[F12] CSV 读写
来源：http://rqm.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gnu.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://liw.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fbx.52xcode.cn

TS:   // 同上
来源：http://mqb.ctjpmb.com


<!-- 参考信息 -->