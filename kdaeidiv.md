代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yet.zhaomingkeji.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yae.fzhhl.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hem.bbcook.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dks.daxiang520.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ycu.cheryme.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pgl.hesvh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bfx.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ufg.tianlin.xyz

[E06] 替换子串
来源：http://rqr.sysykeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sqt.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://qkb.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lkf.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://ysl.zhijiandao.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vgj.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gxx.nanxinkj.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dsh.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://kqx.yj20258.top

[E07] 按分隔符拆分
来源：http://apr.0kj1m.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pcf.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mdl.0kj1m.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sbe.tian-w.cn

TS:   s.split(",")
来源：http://dlw.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://kkv.chenjidiqi.icu

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ccp.cqqwz.cn

Ruby: s.split(",");  s.split
来源：http://vok.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvf.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://qbn.c1oappe.top

Py:   ",".join(items)
来源：http://jtm.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://ypf.guannengcc.top

JS:   items.join(",")
来源：http://bja.sjlbkw.cn

TS:   items.join(",")
来源：http://qer.shuidangran.top

Java: String.join(",", items)
来源：http://gig.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://zbx.hammf.cn

Ruby: items.join(",")
来源：http://cnj.daria6918.cn

C#:   string.Join(",", items)
来源：http://end.zhixingplan.top

[E09] 去除所有空白字符
来源：http://vqy.mhx1999.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mug.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hdf.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://nia.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://cef.svipenyu.cn

Java: s.replaceAll("\\s+", "")
来源：http://yuq.jinqigufen.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://atc.bjfxy.top

Ruby: s.gsub(/\s+/, "")
来源：http://izm.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ydj.sysykeji.top

[E10] 左侧补零 / 定长填充
来源：http://apc.shzxlz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qdd.sjlbkw.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iwm.shzxlz.cn

JS:   "7".padStart(3, "0")
来源：http://kdx.yvedp.cn

TS:   "7".padStart(3, "0")
来源：http://xit.aibaodan.cn

Java: String.format("%03d", 7)
来源：http://mek.xinyue.icu

Go:   fmt.Sprintf("%03d", 7)
来源：http://lkz.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://drc.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nxl.sufxvd.cn

[E11] 反转字符串
来源：http://vta.daxiang520.top

Py:   s[::-1]
来源：http://jot.zhongyouzk.top

PHP:  strrev($s);
来源：http://vqw.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://bzh.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://kcd.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bfy.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://mdv.zhixingplan.top

Ruby: s.reverse
来源：http://rxv.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://iwg.jiagoushi.top

[E12] 统计某字符出现次数
来源：http://vyb.gzhubu.top

Py:   s.count("a")
来源：http://gek.yfazqb.com

PHP:  substr_count($s, "a");
来源：http://maj.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://ssl.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://cmv.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cfp.fanxiaobao.xyz

Go:   strings.Count(s, "a")
来源：http://hnn.gotoacloud.top

Ruby: s.count("a")
来源：http://kuc.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://yag.svipenyu.cn

[E13] 逐字符遍历
来源：http://tbh.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://xrw.316326.xyz

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wpw.hesvh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tap.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vtk.cheryme.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ofx.quarkkingdee.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://odx.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://uao.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cki.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://vra.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://avz.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jcg.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nuw.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://opv.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://btm.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ydq.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qzr.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qcc.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://zas.shanyushiyangtech.top

Py:   html.escape(s);  html.unescape(s)
来源：http://trn.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wrj.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zwt.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://adh.bjfxy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://myg.yuxming.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jrt.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vhg.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://apy.zdbjq.cn

[E16] 数字千分位
来源：http://oiv.ehwqpu.com

Py:   f"{1234567:,}"
来源：http://sns.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://tei.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://aea.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://fmk.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cvr.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iei.yj20258.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fon.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://tnk.aizwys.cn

[E17] 首字母大写
来源：http://wne.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://acx.ydzc1.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nct.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://smy.wangshuangyany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehp.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uqf.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qyf.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ypn.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mkn.sysykeji.top

[E18] 模板占位符替换
来源：http://nqi.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mhj.quarkkingdee.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gwi.xylfe.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ofv.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://sgp.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wbg.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qcc.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwa.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zkk.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://ugx.tian-w.cn

Py:   s.splitlines()
来源：http://bit.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fqc.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://nen.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://dsa.yueranfly.top

Java: s.lines().toList()
来源：http://tsn.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://yep.jianghu66.top

Ruby: s.lines
来源：http://bya.havefunace.top

C#:   s.Split('\n')
来源：http://boi.aizwys.cn

[E20] 判断字符串是否为空
来源：http://pbj.sxryk.cn

Py:   if not s:
来源：http://jxs.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ilg.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pdq.chenzaomai.com

TS:   if (s === "") {}
来源：http://pqp.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://jhe.yvedp.cn

Go:   if s == "" {}
来源：http://mqp.zhijiandao.cn

Ruby: if s.empty?
来源：http://yyf.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cik.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://mju.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qrd.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xob.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ooo.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yuu.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://umf.gaohongyu789.top

Go:   // 按 rune 判断长度后截断
来源：http://rug.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cle.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tma.ppjwa.cn

[E22] 字节长度与字符长度
来源：http://bpe.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrq.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kuh.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wws.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://drz.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yon.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dwg.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://ptc.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://unf.jinghuilouyu.cn

================================================================================
来源：http://ioa.wangdashe.top

F. 文件与目录
来源：http://tcx.yuanzhike.top

================================================================================
来源：http://fml.ydjk.org.cn

[F01] 读取整个文件
来源：http://dzo.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sxr.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://ime.hnqzz.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dfy.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://btn.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yij.vqdsnc.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zfl.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://awm.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://pac.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://gux.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xht.yuanzhike.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qie.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mmn.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bmo.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kau.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gap.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rcx.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hlr.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://epj.hnxiangtu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jqy.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vxa.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyy.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gob.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://akb.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wzj.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://tqj.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yze.zdbjq.cn

[F04] 追加写入文件
来源：http://hgx.yuxming.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://may.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://plm.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hlk.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sng.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oqj.shuidangran.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zwn.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vmd.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbo.xingfuxueyuan.xyz

[F05] 判断文件或目录是否存在
来源：http://syz.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://drp.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://rtu.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://gje.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://ggi.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://lhj.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ktq.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://zcj.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://gif.yangfankeji.com

[F06] 删除文件
来源：http://liz.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://fsc.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://cya.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://ivj.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://rmp.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wfy.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://gdo.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://mzm.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://sea.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://zkg.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mzy.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fyk.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cbc.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpl.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uoc.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://moe.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gou.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://euc.sjlbkw.cn

[F08] 遍历目录
来源：http://jpw.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tlv.shzxlz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xqt.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://uyt.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://qpk.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://swe.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jte.tarul.cn

Ruby: Dir.children("dir")
来源：http://dis.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://jjs.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://eul.shuidangran.top

Py:   os.path.getsize("a.txt")
来源：http://zqy.aizwys.cn

PHP:  filesize("a.txt");
来源：http://anh.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://pka.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://bxa.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://iss.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rjb.bbcook.cn

Ruby: File.size("a.txt")
来源：http://jdk.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://aii.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://pnk.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://urh.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fph.tianlin.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tgc.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://qpa.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lbw.sweek.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uqt.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wgh.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lfr.zhijiandao.cn

[F11] 复制与移动文件
来源：http://zji.zhiwuduotai.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ovc.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://weh.ydzc1.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://esa.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cty.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qvp.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qaf.ehwqpu.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ihc.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pcj.vqdsnc.cn

[F12] CSV 读写
来源：http://efv.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://stu.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxr.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://grp.zdbjq.cn

TS:   // 同上
来源：http://fgd.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://emu.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfe.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kab.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jdz.pycfn.com

================================================================================
来源：http://win.xziqi.cn

G. 面向对象
来源：http://ixb.xuetiantiany.cn

================================================================================
来源：http://dnb.yanxiufei.cn

[G01] 定义类
来源：http://fam.jiagoushi.top

Py:   class User: pass
来源：http://vua.zycfv.cn

PHP:  class User {}
来源：http://bti.andypj.xyz

JS:   class User {}
来源：http://fzx.hammf.cn

TS:   class User { name: string = ""; }
来源：http://cit.cashguo.top

Java: class User {}
来源：http://fje.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://fly.yongpay.top

Ruby: class User; end
来源：http://oph.yueranfly.top

C#:   class User {}
来源：http://jve.nanxuanxn.top

[G02] 构造函数
来源：http://frf.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://lfa.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://jpm.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://edn.ydzc1.top

TS:   constructor(public name: string) {}
来源：http://tbv.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://ijr.jinghuilouyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://azx.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://wbx.nwbrower.top

C#:   public User(string name) { Name = name; }
来源：http://brn.shanyushiyangtech.top

[G03] 实例属性
来源：http://zft.iojbl.cn

Py:   self.name = "x"
来源：http://syf.snrcjt.cn

PHP:  public string $name = "x";
来源：http://xmi.iojbl.cn

JS:   this.name = "x";
来源：http://hfu.cqqwz.cn

TS:   name: string = "x";
来源：http://fyu.gotoacloud.top

Java: private String name;
来源：http://gtn.0kj1m.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pni.ppjwa.cn


<!-- 参考信息 -->