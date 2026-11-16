代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uij.daxiang520.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vcu.zdbjq.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ksw.sysykeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://prr.ywan-chungtsiang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fqg.vehdjk.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://stb.wangshuangyany.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jnu.zdbjq.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xlr.vehdjk.com

[E02] 重复字符串
来源：http://udo.jianghu66.top

Py:   "ab" * 3
来源：http://yil.ywan-chungtsiang.top

PHP:  str_repeat("ab", 3);
来源：http://xfm.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://yje.xinyue.icu

TS:   "ab".repeat(3)
来源：http://osm.chenlongwang.top

Java: "ab".repeat(3)
来源：http://fxk.hnqzz.top

Go:   strings.Repeat("ab", 3)
来源：http://xiq.jinqigufen.top

Ruby: "ab" * 3
来源：http://smm.0kj1m.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ber.xylfe.cn

[E03] 截取子串
来源：http://sxh.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zbn.jinqigufen.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://npo.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gnd.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://mxq.aibaodan.cn

Java: s.substring(1, 4)
来源：http://jxr.ppjwa.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pkq.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://shk.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://cjj.hywenlv.cn

[E04] 查找子串位置
来源：http://lfu.ctjpmb.com

Py:   s.find("x");  s.index("x")
来源：http://krt.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://gvm.hfpthk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vze.zdqjudy.top

TS:   s.indexOf("x")
来源：http://bsm.gaohongyu789.top

Java: s.indexOf("x")
来源：http://pyw.chenlongwang.top

Go:   strings.Index(s, "x")
来源：http://wyh.gaohongyu789.top

Ruby: s.index("x")
来源：http://psh.tianlin.xyz

C#:   s.IndexOf("x")
来源：http://lie.aibaodan.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cmo.zdqjudy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cht.hnxiangtu.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ola.vqdsnc.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjr.nwbrower.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mou.zhongyouzk.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yge.ehwqpu.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://itg.316326.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cwb.vehdjk.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kso.ctjpmb.com

[E06] 替换子串
来源：http://yuu.jyoumei.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tnd.aibaodan.cn

PHP:  str_replace("a", "b", $s);
来源：http://osg.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qrf.jqgufenzy.top

TS:   s.replaceAll("a", "b")
来源：http://vbw.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ehs.ctjpmb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://inf.cqqwz.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nkz.zhiwuduotai.top

C#:   s.Replace("a", "b")
来源：http://pzz.wangdashe.top

[E07] 按分隔符拆分
来源：http://wjd.zhiwuduotai.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vfk.yangfankeji.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://shr.gzhubu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gff.sxryk.cn

TS:   s.split(",")
来源：http://xzv.0kj1m.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sxe.yj202588.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tzr.tanke756.top

Ruby: s.split(",");  s.split
来源：http://phq.jyoumei.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yzh.haohaochexian.top

[E08] 数组按分隔符合并
来源：http://vbi.nwbrower.top

Py:   ",".join(items)
来源：http://pbh.ybcxt.top

PHP:  implode(",", $items);
来源：http://ssf.zhaomingkeji.xyz

JS:   items.join(",")
来源：http://ypx.zhixingplan.top

TS:   items.join(",")
来源：http://dqc.hesvh.cn

Java: String.join(",", items)
来源：http://xdt.pycfn.com

Go:   strings.Join(items, ",")
来源：http://cdb.hywenlv.cn

Ruby: items.join(",")
来源：http://taq.jinghuilouyu.cn

C#:   string.Join(",", items)
来源：http://ulm.sweek.top

[E09] 去除所有空白字符
来源：http://ibn.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pzn.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jlm.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://xuo.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://twr.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://xqk.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://yev.aizwys.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kfa.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwi.sweek.top

[E10] 左侧补零 / 定长填充
来源：http://dim.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tgn.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zfo.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://pdc.xuanzx.com

TS:   "7".padStart(3, "0")
来源：http://bhg.quarkkingdee.top

Java: String.format("%03d", 7)
来源：http://slo.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lzv.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bmn.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nbd.meibo888.top

[E11] 反转字符串
来源：http://qxc.redwolf501.top

Py:   s[::-1]
来源：http://tpm.cheryme.top

PHP:  strrev($s);
来源：http://iux.xylfe.cn

JS:   [...s].reverse().join("")
来源：http://abl.ehwqpu.com

TS:   [...s].reverse().join("")
来源：http://vnz.dianchejie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dpz.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://mpo.yj202588.top

Ruby: s.reverse
来源：http://pxr.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://wid.jyoumei.cn

[E12] 统计某字符出现次数
来源：http://mdj.jinqigfzy.top

Py:   s.count("a")
来源：http://xcd.guowangkeji.top

PHP:  substr_count($s, "a");
来源：http://vqb.gaohongyu789.top

JS:   s.split("a").length - 1
来源：http://zov.c1oappe.top

TS:   s.split("a").length - 1
来源：http://eii.gogol.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fgw.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://dlx.kuanghao11.cn

Ruby: s.count("a")
来源：http://evc.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://ucr.guannengcc.top

[E13] 逐字符遍历
来源：http://tfr.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://gzq.c1oappe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kit.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ivr.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ftu.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndu.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ipr.wangshuangyany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hyn.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://miy.shuidangran.top

[E14] URL 编码与 Base64
来源：http://gur.jinqigfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbz.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://cxz.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://etv.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cnw.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jox.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ika.jlsjyb.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kfq.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fxb.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://itr.yvedp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wfl.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hmy.mhx1999.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fsa.cashguo.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fus.jinqigufen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vmf.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pbt.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ivl.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://klf.cqqwz.cn

[E16] 数字千分位
来源：http://yrm.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://cvs.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://wsw.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qbe.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://rra.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hpu.zhiwuduotai.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fse.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zwc.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://gmc.hfpthk.cn

[E17] 首字母大写
来源：http://fvi.zhiwuduotai.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wbm.yj20258888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ytd.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pph.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ogy.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fzz.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sem.hnxiangtu.top

Ruby: s.capitalize
来源：http://hfw.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wxz.zhoulong.xyz

[E18] 模板占位符替换
来源：http://qzv.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yrn.jinqigfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://idt.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xvb.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://rco.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://psx.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cam.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://upg.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sfk.zdqjudy.top

[E19] 多行文本按行拆分
来源：http://ebq.jlsjyb.cn

Py:   s.splitlines()
来源：http://dpt.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://flq.hesvh.cn

JS:   s.split(/\r?\n/)
来源：http://tni.kuanghao11.cn

TS:   s.split(/\r?\n/)
来源：http://cns.yueranfly.top

Java: s.lines().toList()
来源：http://whc.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://owh.shuidangran.top

Ruby: s.lines
来源：http://rvz.uphjek.com

C#:   s.Split('\n')
来源：http://akb.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://ams.52xcode.cn

Py:   if not s:
来源：http://qvb.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mha.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gzt.feifeiyinyue.top

TS:   if (s === "") {}
来源：http://uzt.xylfe.cn

Java: if (s.isEmpty()) {}
来源：http://hda.sysykeji.top

Go:   if s == "" {}
来源：http://zkl.tanke756.top

Ruby: if s.empty?
来源：http://jnq.ivvv.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://voi.ydzc1.top

[E21] 超长截断加省略号
来源：http://wqi.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uit.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rgj.316326.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cro.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cln.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fnh.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://bmq.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rzq.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dab.guowangkeji.top

[E22] 字节长度与字符长度
来源：http://dtt.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kqb.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dvg.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fjf.hywenlv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wik.daxiang520.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hgw.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://voh.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://lly.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ahd.yuxming.cn

================================================================================
来源：http://fje.guowangkeji.top

F. 文件与目录
来源：http://mvu.yj20258888.top

================================================================================
来源：http://bjr.guowangkeji.top

[F01] 读取整个文件
来源：http://hvx.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wsa.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://jlu.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qrr.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hvn.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kbz.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uqe.zycfv.cn

Ruby: File.read("a.txt")
来源：http://wtd.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://oyv.9152youxi.cn

[F02] 逐行读取文件
来源：http://tgl.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tjj.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ntq.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eqs.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvo.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gba.mhx1999.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dkt.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mja.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://avz.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://zym.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jet.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hoa.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkn.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wmg.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rfy.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ibi.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://mgi.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mcc.haohaochexian.top

[F04] 追加写入文件
来源：http://xkv.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sog.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xei.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qel.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kwr.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wxt.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ndf.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://stw.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ofg.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://sew.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://khh.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://kno.havefunace.top

JS:   fs.existsSync("a.txt")
来源：http://sed.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://dav.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wll.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hkc.chenzaomai.com

Ruby: File.exist?("a.txt")
来源：http://onr.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://aqx.hesvh.cn

[F06] 删除文件
来源：http://wok.pycfn.com

Py:   os.remove("a.txt")
来源：http://myk.smart0.xyz

PHP:  unlink("a.txt");
来源：http://syb.wangdashe.top

JS:   fs.unlinkSync("a.txt")
来源：http://qmk.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://ixa.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://suw.xuanzx.com

Go:   os.Remove("a.txt")
来源：http://yyi.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://kjz.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://bik.yfazqb.com

[F07] 创建目录（含多级）
来源：http://iit.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://puz.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kqb.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://chw.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owj.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qtp.hammf.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://idp.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://muw.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sto.c1oappe.top

[F08] 遍历目录
来源：http://fud.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://alj.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ohu.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://stc.ywan-chungtsiang.top

TS:   fs.readdirSync("dir")
来源：http://hgb.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://doq.haohaochexian.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jcc.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://mct.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://jnt.yj20258.top

[F09] 获取文件大小
来源：http://wtv.tianlin.xyz

Py:   os.path.getsize("a.txt")
来源：http://kbx.wangdashe.top

PHP:  filesize("a.txt");
来源：http://agc.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://zjw.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://zki.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hva.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtn.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://yif.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://qnu.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://gpr.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zqd.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ncm.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qdi.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://cve.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uei.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://btc.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rbd.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ytw.pengpengdd.cyou

[F11] 复制与移动文件
来源：http://tkz.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wof.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ohx.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ond.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymt.9152youxi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://whr.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ihb.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hob.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mzo.hongshengwenyu.top

[F12] CSV 读写
来源：http://mgt.bjfxy.top


<!-- 参考信息 -->