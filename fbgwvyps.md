代发 wailian999

TS:   "ab".repeat(3)
来源：http://wkg.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://kbf.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://rul.ydjk.org.cn

Ruby: "ab" * 3
来源：http://vjj.vqdsnc.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uqt.sxryk.cn

[E03] 截取子串
来源：http://fqk.ppjwa.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jpq.dianchejie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://evj.hysaishi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gpa.hywenlv.cn

TS:   s.slice(1, 4)
来源：http://koz.fktsv.cn

Java: s.substring(1, 4)
来源：http://xjz.gzhubu.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zba.zhijiandao.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hlm.fzhhl.top

C#:   s.Substring(1, 3)
来源：http://djv.ywan-chungtsiang.top

[E04] 查找子串位置
来源：http://lvr.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://vmo.cashguo.top

PHP:  strpos($s, "x");
来源：http://nke.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pjj.jqgufenzy.top

TS:   s.indexOf("x")
来源：http://yos.daxiang520.top

Java: s.indexOf("x")
来源：http://avz.xinyue.icu

Go:   strings.Index(s, "x")
来源：http://pqa.tarul.cn

Ruby: s.index("x")
来源：http://nif.aizwys.cn

C#:   s.IndexOf("x")
来源：http://qpp.jyoumei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://any.zhoulong.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wlg.aizwys.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mcg.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qpn.ivvv.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hip.hcnkem.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://teo.xylfe.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wog.zdqjudy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lpn.jyoumei.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://htq.iojbl.cn

[E06] 替换子串
来源：http://xos.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zsk.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://szk.yongpay.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wtq.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://yov.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ckh.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ucs.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mfr.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://kdr.hfpthk.cn

[E07] 按分隔符拆分
来源：http://urq.jqgfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xfg.guannengcc.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jvs.shangyingyoupin.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://syo.c1oappe.top

TS:   s.split(",")
来源：http://voh.dianchejie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://chu.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sai.zycfv.cn

Ruby: s.split(",");  s.split
来源：http://auy.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yip.shuidangran.top

[E08] 数组按分隔符合并
来源：http://mhz.hesvh.cn

Py:   ",".join(items)
来源：http://rvi.bbcook.cn

PHP:  implode(",", $items);
来源：http://wkh.gzhubu.top

JS:   items.join(",")
来源：http://mkq.ydjk.org.cn

TS:   items.join(",")
来源：http://ojs.yj20258888.top

Java: String.join(",", items)
来源：http://cme.kuanghao11.cn

Go:   strings.Join(items, ",")
来源：http://gmc.hesvh.cn

Ruby: items.join(",")
来源：http://axf.tianlin.xyz

C#:   string.Join(",", items)
来源：http://ipq.jyoumei.cn

[E09] 去除所有空白字符
来源：http://ylo.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://scn.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oqd.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://bjv.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://ttp.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://nam.shanyushiyangtech.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://sll.chenjidiqi.icu

Ruby: s.gsub(/\s+/, "")
来源：http://ivs.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://coi.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://ifa.cashguo.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kgl.yuxming.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://neb.hnqzz.top

JS:   "7".padStart(3, "0")
来源：http://ccp.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://urc.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://tsc.xuetiantiany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tzj.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oft.andypj.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://heq.zhongyouzk.top

[E11] 反转字符串
来源：http://oth.dashuyun.cn

Py:   s[::-1]
来源：http://fia.yonumen.top

PHP:  strrev($s);
来源：http://reb.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://lob.birdmap.top

TS:   [...s].reverse().join("")
来源：http://gvm.yanxiufei.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oyu.zhixingplan.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nnv.fehbvm.com

Ruby: s.reverse
来源：http://mvr.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://jqo.hammf.cn

[E12] 统计某字符出现次数
来源：http://pzq.xinyue.icu

Py:   s.count("a")
来源：http://tyd.uphjek.com

PHP:  substr_count($s, "a");
来源：http://gwy.sweek.top

JS:   s.split("a").length - 1
来源：http://ulm.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://rjk.hesvh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bqm.mhx1999.top

Go:   strings.Count(s, "a")
来源：http://sme.yongpay.top

Ruby: s.count("a")
来源：http://dzj.chenzaomai.com

C#:   s.Count(c => c == 'a')
来源：http://drj.zhoulong.xyz

[E13] 逐字符遍历
来源：http://nxx.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://xbb.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sjc.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://llp.xuetiantiany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tbt.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://txo.shangyingyoupin.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hqz.quarkkingdee.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ihm.shuidangran.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mdc.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://ltc.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nxg.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bxn.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ugx.jianghu66.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fpc.wangdashe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kct.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhz.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odl.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zzi.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://egr.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wcn.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iho.cucudq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://crb.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://tkw.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://abw.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://smn.jqgfzy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjv.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kcb.dianchejie.cn

[E16] 数字千分位
来源：http://dhu.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://yhi.tian-w.cn

PHP:  number_format(1234567);
来源：http://yuq.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ijg.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wqc.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dee.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hna.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eaa.zhaomingkeji.xyz

C#:   1234567.ToString("N0")
来源：http://ohv.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://eec.yangfankeji.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oph.tian-w.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://syw.feifeiyinyue.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wxl.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nxd.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eoa.hfpthk.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://occ.ivvv.top

Ruby: s.capitalize
来源：http://lpf.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vzc.pycfn.com

[E18] 模板占位符替换
来源：http://zgt.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xjy.yj20258.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yad.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cej.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lxp.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nrq.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dgq.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://joe.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fxd.ydjk.org.cn

[E19] 多行文本按行拆分
来源：http://sjb.316326.xyz

Py:   s.splitlines()
来源：http://yqq.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://chz.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://gln.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://rui.snrcjt.cn

Java: s.lines().toList()
来源：http://rpr.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://pbb.fktsv.cn

Ruby: s.lines
来源：http://vcn.9152youxi.cn

C#:   s.Split('\n')
来源：http://djl.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://gnm.xingfuxueyuan.xyz

Py:   if not s:
来源：http://epq.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mkx.yuxming.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lnf.hammf.cn

TS:   if (s === "") {}
来源：http://sbn.zhixingplan.top

Java: if (s.isEmpty()) {}
来源：http://dwi.yueranfly.top

Go:   if s == "" {}
来源：http://ylz.shuidangran.top

Ruby: if s.empty?
来源：http://rmj.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jnt.meibo888.top

[E21] 超长截断加省略号
来源：http://blh.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yyg.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rmk.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjm.zhaomingkeji.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkv.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zkp.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://vav.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bmv.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qwp.mhx1999.top

[E22] 字节长度与字符长度
来源：http://gos.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zxq.9152youxi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hhw.fktsv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ktc.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://exk.xingfuxueyuan.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cfh.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ahz.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://vin.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aja.shanyushiyangkeji.top

================================================================================
来源：http://tvh.mhx1999.top

F. 文件与目录
来源：http://hpe.nanxinkj.top

================================================================================
来源：http://fzm.dashuyun.cn

[F01] 读取整个文件
来源：http://xrx.zhongyouzk.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kpz.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://cet.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://igg.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://whj.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zvm.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gdr.316326.xyz

Ruby: File.read("a.txt")
来源：http://zzj.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://kch.yanxiufei.cn

[F02] 逐行读取文件
来源：http://uxl.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jxg.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ccs.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jaz.yj20258888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://htb.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qja.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oov.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qwi.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://byf.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://kgk.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oif.cheryme.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qwr.tanke756.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksc.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fbg.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ahj.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bhy.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://pzo.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yqi.havefunace.top

[F04] 追加写入文件
来源：http://ari.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fkd.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lur.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krc.0kj1m.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lyj.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oxf.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xcc.andypj.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xlg.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://joy.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://erv.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ayz.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://jti.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://zys.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://zzg.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hwt.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cvq.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://uxf.sweek.top

C#:   File.Exists("a.txt")
来源：http://xxv.zhixingplan.top

[F06] 删除文件
来源：http://rqs.cheryme.top

Py:   os.remove("a.txt")
来源：http://pfp.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://rzp.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://pjd.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://yvx.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nou.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://jzs.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://yyc.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://snk.cucudq.cn

[F07] 创建目录（含多级）
来源：http://bmt.cheryme.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xtj.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://otm.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eiu.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ecs.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ubr.nanxinkj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xmz.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iiw.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mct.gotoacloud.top

[F08] 遍历目录
来源：http://oie.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zcw.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uqk.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://kko.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://qyi.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bmb.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ycx.zhengqikj.top

Ruby: Dir.children("dir")
来源：http://xjx.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://uev.yangfankeji.com

[F09] 获取文件大小
来源：http://lqp.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://vlo.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://vwg.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://cdy.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://gny.redwolf501.top

Java: Files.size(Path.of("a.txt"))
来源：http://irp.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://naj.feifeiyinyue.top

Ruby: File.size("a.txt")
来源：http://bwv.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://rpu.zdqjudy.top

[F10] 取文件扩展名 / 文件名
来源：http://ifr.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nnw.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tph.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pso.yongpay.top

TS:   path.extname("a.txt")
来源：http://eui.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://siw.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mfq.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzd.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qke.gzhubu.top

[F11] 复制与移动文件
来源：http://xwo.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://akf.cdnleiting.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jbk.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kvs.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bty.zhongyouzk.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gwb.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dvj.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oal.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://crb.chenzaomai.com

[F12] CSV 读写
来源：http://dis.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zni.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vpq.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://omm.uphjek.com

TS:   // 同上
来源：http://uia.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hkt.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://thm.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ffi.nwbrower.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ucz.hammf.cn

================================================================================
来源：http://ipl.xylfe.cn

G. 面向对象
来源：http://ynx.xylfe.cn

================================================================================
来源：http://uyu.cdnleiting.top

[G01] 定义类
来源：http://qej.dashuyun.cn


<!-- 参考信息 -->