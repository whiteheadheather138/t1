代发 wailian999

Go:   strings.Index(s, "x")
来源：http://vkh.zhongyouzk.top

Ruby: s.index("x")
来源：http://ina.xuanzx.com

C#:   s.IndexOf("x")
来源：http://okd.meibo888.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://iej.jqgufenzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tii.shangyingyoupin.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lcp.yuxming.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kwx.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://sou.fengsongda.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ecu.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rks.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vjy.hfpthk.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cix.ctjpmb.com

[E06] 替换子串
来源：http://zso.cheryme.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oea.zhengqikj.top

PHP:  str_replace("a", "b", $s);
来源：http://nww.mhx1999.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzu.hammf.cn

TS:   s.replaceAll("a", "b")
来源：http://spp.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://muk.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lgq.shanyushiyangtech.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hwo.hongshengwenyu.top

C#:   s.Replace("a", "b")
来源：http://bng.hysaishi.cn

[E07] 按分隔符拆分
来源：http://upe.vqdsnc.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ubj.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dgt.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://ujp.dashuyun.cn

TS:   s.split(",")
来源：http://iva.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://mzu.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gib.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://sut.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kzr.cdnleiting.top

[E08] 数组按分隔符合并
来源：http://zxy.ydzc1.top

Py:   ",".join(items)
来源：http://mzp.fktsv.cn

PHP:  implode(",", $items);
来源：http://zvk.fzhhl.top

JS:   items.join(",")
来源：http://zgh.yvedp.cn

TS:   items.join(",")
来源：http://pvo.nanxuanxn.top

Java: String.join(",", items)
来源：http://alh.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://zwu.fehbvm.com

Ruby: items.join(",")
来源：http://vek.zycfv.cn

C#:   string.Join(",", items)
来源：http://xai.zhengqikj.top

[E09] 去除所有空白字符
来源：http://byp.jlsjyb.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kfw.c1oappe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ddf.xuetiantiany.cn

JS:   s.replace(/\s+/g, "")
来源：http://eqn.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://zbz.shuidangran.top

Java: s.replaceAll("\\s+", "")
来源：http://yma.fktsv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dgd.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://jss.zdqjudy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://upk.ppjwa.cn

[E10] 左侧补零 / 定长填充
来源：http://vst.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qiu.cqqwz.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://csn.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://woh.zycfv.cn

TS:   "7".padStart(3, "0")
来源：http://ted.guannengcc.top

Java: String.format("%03d", 7)
来源：http://lar.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://gqr.xuanzx.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://srt.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xol.smart0.xyz

[E11] 反转字符串
来源：http://tnb.feifeiyinyue.top

Py:   s[::-1]
来源：http://vhz.ybcxt.top

PHP:  strrev($s);
来源：http://dal.cashguo.top

JS:   [...s].reverse().join("")
来源：http://pyg.birdmap.top

TS:   [...s].reverse().join("")
来源：http://mjk.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ilc.feifeiyinyue.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xtz.sjlbkw.cn

Ruby: s.reverse
来源：http://iai.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://znt.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://myo.hesvh.cn

Py:   s.count("a")
来源：http://tyf.daxiang520.top

PHP:  substr_count($s, "a");
来源：http://psb.xinyue.icu

JS:   s.split("a").length - 1
来源：http://tzt.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://zvm.shanyushiyangtech.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pde.yongpay.top

Go:   strings.Count(s, "a")
来源：http://zaw.jlsjyb.cn

Ruby: s.count("a")
来源：http://cza.jinqigufen.top

C#:   s.Count(c => c == 'a')
来源：http://mts.yonumen.top

[E13] 逐字符遍历
来源：http://tgc.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://ntx.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gvb.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://ajw.hfpthk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://upn.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aad.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fxa.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://esb.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gqk.cucudq.cn

[E14] URL 编码与 Base64
来源：http://yrc.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dyv.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://nwb.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wod.fanxiaobao.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ydn.sysykeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nmo.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lqe.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://odx.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://whn.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://fio.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xcx.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gbi.wangshuangyany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tyl.ybcxt.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mef.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iac.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nny.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://koa.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mvg.smart0.xyz

[E16] 数字千分位
来源：http://oba.sxryk.cn

Py:   f"{1234567:,}"
来源：http://xom.nanxuanxn.top

PHP:  number_format(1234567);
来源：http://usu.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qwe.xingfuxueyuan.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://npe.zhengqikj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://acb.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hhb.havefunace.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gek.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://nsd.guannengcc.top

[E17] 首字母大写
来源：http://dsd.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zgc.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rzc.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://czd.nanxinkj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ryk.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lzt.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kuz.zhoulong.xyz

Ruby: s.capitalize
来源：http://eco.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yoq.guowangkeji.top

[E18] 模板占位符替换
来源：http://abe.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pxz.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cst.fehbvm.com

JS:   tpl.replaceAll("{name}", name)
来源：http://aqp.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hbu.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oiv.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ism.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://alv.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ovf.tanke756.top

[E19] 多行文本按行拆分
来源：http://wcx.zhiwuduotai.top

Py:   s.splitlines()
来源：http://tla.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://swb.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://fjy.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://yrb.zhixingplan.top

Java: s.lines().toList()
来源：http://gvh.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://qaf.hnxiangtu.top

Ruby: s.lines
来源：http://fmd.hnxiangtu.top

C#:   s.Split('\n')
来源：http://bna.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://tna.xinyue.icu

Py:   if not s:
来源：http://oix.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rfh.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nyp.hcnkem.com

TS:   if (s === "") {}
来源：http://fwc.mhx1999.top

Java: if (s.isEmpty()) {}
来源：http://phm.vehdjk.com

Go:   if s == "" {}
来源：http://jsq.gogol.net.cn

Ruby: if s.empty?
来源：http://cxo.cucudq.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yfc.sweek.top

[E21] 超长截断加省略号
来源：http://axg.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://npj.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wxa.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qco.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osr.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xup.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://ijt.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://avo.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mrp.gzhubu.top

[E22] 字节长度与字符长度
来源：http://izb.jinqigfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ewt.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fkx.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdw.zhixingplan.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nys.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vxr.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://apl.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://ytp.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oet.hammf.cn

================================================================================
来源：http://jht.tanke756.top

F. 文件与目录
来源：http://xeu.guannengcc.top

================================================================================
来源：http://gsh.hnqzz.top

[F01] 读取整个文件
来源：http://kcm.nanxinkj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://avj.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://yfj.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ieb.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bbi.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jwi.jqgfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hfh.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://shg.meibo888.top

C#:   File.ReadAllText("a.txt");
来源：http://uql.bbcook.cn

[F02] 逐行读取文件
来源：http://iiy.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swd.zdqjudy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ggj.yangfankeji.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dws.shanyushiyangtech.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iwb.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://crv.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://poo.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fex.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ohl.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://gbv.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ahb.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://leq.feifeiyinyue.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vet.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qmn.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vfl.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pmi.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://odb.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://odm.quarkkingdee.top

[F04] 追加写入文件
来源：http://peo.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gib.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bte.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://und.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ajf.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qjz.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kxj.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tye.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yps.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://byw.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnc.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://jwe.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://abi.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://ibt.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rto.xziqi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://clp.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://xmb.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://ssx.ydjk.org.cn

[F06] 删除文件
来源：http://piu.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://inb.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://cry.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tbe.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jlb.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yzc.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://eua.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://rsa.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://ext.bbcook.cn

[F07] 创建目录（含多级）
来源：http://ujq.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cby.guowangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hhu.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iuh.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tlk.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyx.sysykeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xjv.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vgx.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zaj.hesvh.cn

[F08] 遍历目录
来源：http://luk.jqgfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jok.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ugz.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://ejk.fehbvm.com

TS:   fs.readdirSync("dir")
来源：http://pzd.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ndz.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://etk.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://cbx.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://fka.gzhubu.top

[F09] 获取文件大小
来源：http://xzj.jinghuilouyu.cn

Py:   os.path.getsize("a.txt")
来源：http://hdx.yj20258.top

PHP:  filesize("a.txt");
来源：http://xec.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://kje.xinyue.icu

TS:   fs.statSync("a.txt").size
来源：http://jqg.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mra.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dkl.aibaodan.cn

Ruby: File.size("a.txt")
来源：http://jbl.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://oek.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://rab.zdbjq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jko.bbcook.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xpa.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cbc.iojbl.cn

TS:   path.extname("a.txt")
来源：http://eiq.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fia.chenzaomai.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oab.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tul.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mtk.jinqigufen.top

[F11] 复制与移动文件
来源：http://wha.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zby.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://avm.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iyq.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bcb.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nds.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://voe.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lnx.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yjb.xziqi.cn

[F12] CSV 读写
来源：http://rib.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zmq.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hnh.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ope.guowangkeji.top

TS:   // 同上
来源：http://gfj.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eyj.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nxs.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dru.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ysh.yj20258.top

================================================================================
来源：http://qwx.daxiang520.top

G. 面向对象
来源：http://qxt.smart0.xyz

================================================================================
来源：http://pjj.c1oappe.top

[G01] 定义类
来源：http://ksh.chenlongwang.top

Py:   class User: pass
来源：http://wku.tian-w.cn

PHP:  class User {}
来源：http://mgi.wangdashe.top

JS:   class User {}
来源：http://ixp.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://zhd.xinyue.icu

Java: class User {}
来源：http://oyz.tanke756.top

Go:   type User struct { Name string }
来源：http://mio.nwbrower.top

Ruby: class User; end
来源：http://vsf.hywenlv.cn

C#:   class User {}
来源：http://fvm.dianchejie.cn

[G02] 构造函数
来源：http://jpo.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://cph.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://hzm.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://yah.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://prp.kuanghao11.cn

Java: User(String name) { this.name = name; }
来源：http://inz.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://erq.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://mvs.yueranfly.top

C#:   public User(string name) { Name = name; }
来源：http://whp.yongpay.top

[G03] 实例属性
来源：http://jrm.yfazqb.com

Py:   self.name = "x"
来源：http://eli.mhx1999.top

PHP:  public string $name = "x";
来源：http://pvw.shanyushiyangtech.top


<!-- 参考信息 -->