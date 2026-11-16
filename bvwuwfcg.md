代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://ubs.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://dps.zhoulong.xyz

[E04] 查找子串位置
来源：http://jpc.smart0.xyz

Py:   s.find("x");  s.index("x")
来源：http://mxp.smart0.xyz

PHP:  strpos($s, "x");
来源：http://gtg.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xth.sysykeji.top

TS:   s.indexOf("x")
来源：http://lnm.ctjpmb.com

Java: s.indexOf("x")
来源：http://zfs.jianghu66.top

Go:   strings.Index(s, "x")
来源：http://itp.wangdashe.top

Ruby: s.index("x")
来源：http://fbe.zycfv.cn

C#:   s.IndexOf("x")
来源：http://knn.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://dmq.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://trl.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dce.jlsjyb.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tal.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vyk.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qmw.cashguo.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aln.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cms.yonumen.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fxk.smart0.xyz

[E06] 替换子串
来源：http://rlj.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hxd.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://srq.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zwb.jinqigufen.top

TS:   s.replaceAll("a", "b")
来源：http://kcz.xingfuxueyuan.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bho.chenzaomai.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://elj.yueranfly.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lwj.shangyingyoupin.top

C#:   s.Replace("a", "b")
来源：http://hpx.tanke756.top

[E07] 按分隔符拆分
来源：http://pnw.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://joo.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aiq.jqgfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://xpf.ydzc1.top

TS:   s.split(",")
来源：http://lbc.sufxvd.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ytt.zhengqikj.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pud.sweek.top

Ruby: s.split(",");  s.split
来源：http://xrd.yongpay.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uuu.sxryk.cn

[E08] 数组按分隔符合并
来源：http://muc.hysaishi.cn

Py:   ",".join(items)
来源：http://iyy.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://hwb.vehdjk.com

JS:   items.join(",")
来源：http://kpx.guannengcc.top

TS:   items.join(",")
来源：http://tli.hysaishi.cn

Java: String.join(",", items)
来源：http://tgx.jinyuanbaomall.cn

Go:   strings.Join(items, ",")
来源：http://snm.tian-w.cn

Ruby: items.join(",")
来源：http://vwe.zhoulong.xyz

C#:   string.Join(",", items)
来源：http://cxr.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://qgl.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fch.chenzaomai.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yfm.yonumen.top

JS:   s.replace(/\s+/g, "")
来源：http://oxr.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://auv.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://bvw.0kj1m.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cfn.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://pih.cdnleiting.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dwu.hcnkem.com

[E10] 左侧补零 / 定长填充
来源：http://cbj.nwbrower.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hub.sweek.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ekl.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://ghr.fanxiaobao.xyz

TS:   "7".padStart(3, "0")
来源：http://wdb.jyoumei.cn

Java: String.format("%03d", 7)
来源：http://smf.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bgt.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lqz.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zce.iojbl.cn

[E11] 反转字符串
来源：http://tri.yfazqb.com

Py:   s[::-1]
来源：http://ohy.havefunace.top

PHP:  strrev($s);
来源：http://hrs.sweek.top

JS:   [...s].reverse().join("")
来源：http://xzm.yanxiufei.cn

TS:   [...s].reverse().join("")
来源：http://sqh.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ekh.cheryme.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://slr.fzhhl.top

Ruby: s.reverse
来源：http://jtp.ydzc1.top

C#:   new string(s.Reverse().ToArray())
来源：http://yge.ybcxt.top

[E12] 统计某字符出现次数
来源：http://mzp.shuidangran.top

Py:   s.count("a")
来源：http://fpr.ydzc1.top

PHP:  substr_count($s, "a");
来源：http://nyj.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://mqd.tarul.cn

TS:   s.split("a").length - 1
来源：http://hkf.yanxiufei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cga.316326.xyz

Go:   strings.Count(s, "a")
来源：http://aiq.yj20258888.top

Ruby: s.count("a")
来源：http://nxo.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://pud.vehdjk.com

[E13] 逐字符遍历
来源：http://omz.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://nuz.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tnf.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://hiw.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://twe.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pum.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jkz.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rrb.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://poa.hesvh.cn

[E14] URL 编码与 Base64
来源：http://ste.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oda.jiagoushi.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vve.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bjc.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eyt.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://khm.havefunace.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dun.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dwd.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://doc.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://bkq.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://knz.gzhubu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nys.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cfq.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zly.xuanzx.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ofe.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uac.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://evn.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://chh.shanyushiyangtech.top

[E16] 数字千分位
来源：http://jbp.hnxiangtu.top

Py:   f"{1234567:,}"
来源：http://dsh.sufxvd.cn

PHP:  number_format(1234567);
来源：http://nsv.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nyp.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://ejj.gaohongyu789.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zgb.shzxlz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qvb.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uwg.yongpay.top

C#:   1234567.ToString("N0")
来源：http://cdp.zdqjudy.top

[E17] 首字母大写
来源：http://mpn.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://koh.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ujm.jqgufenzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lkc.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qtm.feifeiyinyue.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zav.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xtg.sufxvd.cn

Ruby: s.capitalize
来源：http://zsm.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bsb.birdmap.top

[E18] 模板占位符替换
来源：http://ead.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rcg.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rkt.chenjidiqi.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://xqu.fehbvm.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gan.yuxming.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hmk.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lsx.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hub.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pjn.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://owl.yj20258888.top

Py:   s.splitlines()
来源：http://umz.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sel.feifeiyinyue.top

JS:   s.split(/\r?\n/)
来源：http://uve.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://yhi.cheryme.top

Java: s.lines().toList()
来源：http://yzh.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://ayg.hammf.cn

Ruby: s.lines
来源：http://frn.ivvv.top

C#:   s.Split('\n')
来源：http://bqq.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://rsv.316326.xyz

Py:   if not s:
来源：http://ymb.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://joz.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nfh.sufxvd.cn

TS:   if (s === "") {}
来源：http://ebx.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://zuc.tarul.cn

Go:   if s == "" {}
来源：http://dzy.yfazqb.com

Ruby: if s.empty?
来源：http://hgb.vqdsnc.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://heg.iojbl.cn

[E21] 超长截断加省略号
来源：http://drm.epnwcf.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jfm.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mik.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://alo.bbcook.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nhf.jyoumei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yvv.chenjidiqi.icu

Go:   // 按 rune 判断长度后截断
来源：http://mvo.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://taz.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ezq.quarkkingdee.top

[E22] 字节长度与字符长度
来源：http://evt.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zex.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xps.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyh.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gst.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://otc.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hjs.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://qtd.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xwh.yueranfly.top

================================================================================
来源：http://lmz.zhiwuduotai.top

F. 文件与目录
来源：http://nmy.shanyushiyangkeji.top

================================================================================
来源：http://heu.cashguo.top

[F01] 读取整个文件
来源：http://odi.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pmx.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://ksg.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cmz.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qrw.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kkc.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pdj.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://kva.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://wck.ydjk.org.cn

[F02] 逐行读取文件
来源：http://pdh.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dxq.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://abh.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mbj.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zpw.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uue.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vrn.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fme.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xea.yvedp.cn

[F03] 写入文件（覆盖）
来源：http://tse.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gxz.yanxiufei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qjx.pengpengdd.cyou

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cra.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gld.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rop.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qsg.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://vgl.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hkq.xuanzx.com

[F04] 追加写入文件
来源：http://xte.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ezg.yvedp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uvy.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lfg.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qtn.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fuy.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lna.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://seo.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oru.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://yqn.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hmz.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://zpk.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://rhi.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://twd.yangfankeji.com

Java: Files.exists(Path.of("a.txt"))
来源：http://obv.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rch.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://yaz.yonumen.top

C#:   File.Exists("a.txt")
来源：http://yib.yueranfly.top

[F06] 删除文件
来源：http://zrn.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://ohz.bjfxy.top

PHP:  unlink("a.txt");
来源：http://wxk.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lvi.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bap.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jzr.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://vaf.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://hup.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://vos.shanyushiyangkeji.top

[F07] 创建目录（含多级）
来源：http://cyj.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://adt.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ryg.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vtg.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nxw.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sog.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vpw.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://djd.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tjo.hfpthk.cn

[F08] 遍历目录
来源：http://jza.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://krr.xylfe.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ggv.jiagoushi.top

JS:   fs.readdirSync("dir")
来源：http://mjo.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://oiq.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vdg.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://bzs.sysykeji.top

Ruby: Dir.children("dir")
来源：http://ipy.fehbvm.com

C#:   Directory.GetFiles("dir")
来源：http://yym.haohaochexian.top

[F09] 获取文件大小
来源：http://hlj.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://nzr.smart0.xyz

PHP:  filesize("a.txt");
来源：http://icc.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://aua.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://ytv.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://azl.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ouw.yongpay.top

Ruby: File.size("a.txt")
来源：http://foi.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://sox.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://jqc.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lnp.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hwh.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gzl.hammf.cn

TS:   path.extname("a.txt")
来源：http://msj.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ftw.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://epk.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lax.aizwys.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://unw.c1oappe.top

[F11] 复制与移动文件
来源：http://vjv.hcnkem.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bpe.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://epv.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://flx.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ehd.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dej.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tqi.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yjb.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://koo.hnqzz.top

[F12] CSV 读写
来源：http://tsj.hnqzz.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://icp.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lwo.jinyuanbaomall.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mib.haohaochexian.top

TS:   // 同上
来源：http://woa.vehdjk.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://omv.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hcd.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ljh.jqgufenzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qig.9152youxi.cn

================================================================================
来源：http://ety.mhx1999.top

G. 面向对象
来源：http://kxl.hesvh.cn

================================================================================
来源：http://ikk.jianghu66.top

[G01] 定义类
来源：http://ntp.andypj.xyz

Py:   class User: pass
来源：http://oig.ctjpmb.com

PHP:  class User {}
来源：http://thk.haohaochexian.top

JS:   class User {}
来源：http://ndo.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://kij.jinqigfzy.top

Java: class User {}
来源：http://qyu.aizwys.cn

Go:   type User struct { Name string }
来源：http://kkc.daria6918.cn

Ruby: class User; end
来源：http://oys.zhijiandao.cn

C#:   class User {}
来源：http://tby.uphjek.com

[G02] 构造函数
来源：http://nbr.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://rup.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://kyt.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://okh.guannengcc.top


<!-- 参考信息 -->