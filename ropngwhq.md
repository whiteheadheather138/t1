代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pkn.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://swr.0kj1m.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wee.yfazqb.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gud.yj20258.top

[E06] 替换子串
来源：http://ism.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://str.gaohongyu789.top

PHP:  str_replace("a", "b", $s);
来源：http://nmo.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yrs.zdqjudy.top

TS:   s.replaceAll("a", "b")
来源：http://nvl.shanyushiyangtech.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cww.pengpengdd.cyou

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://phv.fengsongda.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eya.zhixingplan.top

C#:   s.Replace("a", "b")
来源：http://fxm.chenzaomai.com

[E07] 按分隔符拆分
来源：http://kyq.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ryz.tianlin.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpt.jqgufenzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vix.jqgfzy.top

TS:   s.split(",")
来源：http://uoe.fehbvm.com

Java: s.split(",");  s.split("\\s+")
来源：http://bbw.fktsv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eaz.shuidangran.top

Ruby: s.split(",");  s.split
来源：http://tti.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mxq.xylfe.cn

[E08] 数组按分隔符合并
来源：http://vcq.yongpay.top

Py:   ",".join(items)
来源：http://xpf.jiagoushi.top

PHP:  implode(",", $items);
来源：http://hwg.meibo888.top

JS:   items.join(",")
来源：http://fni.cdnleiting.top

TS:   items.join(",")
来源：http://ukd.havefunace.top

Java: String.join(",", items)
来源：http://qqc.gzhubu.top

Go:   strings.Join(items, ",")
来源：http://pge.zdqjudy.top

Ruby: items.join(",")
来源：http://nhe.52xcode.cn

C#:   string.Join(",", items)
来源：http://rym.svipenyu.cn

[E09] 去除所有空白字符
来源：http://jie.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ksn.gzhubu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lvm.sysykeji.top

JS:   s.replace(/\s+/g, "")
来源：http://exh.fanxiaobao.xyz

TS:   s.replace(/\s+/g, "")
来源：http://ekl.haohaochexian.top

Java: s.replaceAll("\\s+", "")
来源：http://ovv.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rrb.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://dql.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cwq.tarul.cn

[E10] 左侧补零 / 定长填充
来源：http://ome.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://aof.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lcc.wangshuangyany.cn

JS:   "7".padStart(3, "0")
来源：http://gqo.vqdsnc.cn

TS:   "7".padStart(3, "0")
来源：http://itl.shzxlz.cn

Java: String.format("%03d", 7)
来源：http://ncy.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zic.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tgr.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cqr.pengpengdd.cyou

[E11] 反转字符串
来源：http://tqa.ivvv.top

Py:   s[::-1]
来源：http://jsz.yongpay.top

PHP:  strrev($s);
来源：http://fgy.zhixingplan.top

JS:   [...s].reverse().join("")
来源：http://gwb.zdqjudy.top

TS:   [...s].reverse().join("")
来源：http://amm.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rdy.zhijiandao.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://txf.cheryme.top

Ruby: s.reverse
来源：http://wer.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://xeo.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://ckn.tarul.cn

Py:   s.count("a")
来源：http://kcy.yj202588.top

PHP:  substr_count($s, "a");
来源：http://qjx.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://tto.daxiang520.top

TS:   s.split("a").length - 1
来源：http://yyg.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fgu.hnxiangtu.top

Go:   strings.Count(s, "a")
来源：http://ufz.chenzaomai.com

Ruby: s.count("a")
来源：http://jto.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://ogn.fzhhl.top

[E13] 逐字符遍历
来源：http://veb.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://nlj.jianghu66.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hpv.52xcode.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dnm.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://toh.jqgfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pyk.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dhf.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://weu.jinqigfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vhe.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://djl.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aar.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://sjt.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dsj.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fxc.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wrt.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wvs.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wbw.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rwb.sweek.top

[E15] HTML 转义 / 反转义
来源：http://lid.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ujn.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iwy.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gnt.mhx1999.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ygx.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kyk.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://idv.hnxiangtu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://umg.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nhg.shzxlz.cn

[E16] 数字千分位
来源：http://pft.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://bet.gogol.net.cn

PHP:  number_format(1234567);
来源：http://hhv.zhiwuduotai.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tkn.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lew.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xre.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lso.daxiang520.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tkw.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://sic.316326.xyz

[E17] 首字母大写
来源：http://loc.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wfa.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://unn.birdmap.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evb.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xeq.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cyu.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zgc.sysykeji.top

Ruby: s.capitalize
来源：http://uxn.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aab.smart0.xyz

[E18] 模板占位符替换
来源：http://zpy.yj20258.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mmi.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kkk.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lgl.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://brj.vehdjk.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ssy.jqgfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gzq.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hle.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ihm.tianlin.xyz

[E19] 多行文本按行拆分
来源：http://umj.zhongyouzk.top

Py:   s.splitlines()
来源：http://mes.sxryk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xyk.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://qij.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://uie.yj20258.top

Java: s.lines().toList()
来源：http://kts.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://npn.xuetiantiany.cn

Ruby: s.lines
来源：http://kcu.ydjk.org.cn

C#:   s.Split('\n')
来源：http://tad.yanxiufei.cn

[E20] 判断字符串是否为空
来源：http://kwv.shanyushiyangkeji.top

Py:   if not s:
来源：http://nrf.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ssq.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pjw.yvedp.cn

TS:   if (s === "") {}
来源：http://pui.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://pdi.xuanzx.com

Go:   if s == "" {}
来源：http://mjb.cqqwz.cn

Ruby: if s.empty?
来源：http://jar.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ipa.guannengcc.top

[E21] 超长截断加省略号
来源：http://sbf.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mra.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wgo.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pkl.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mqn.jlsjyb.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jnq.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://cgi.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gag.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wpe.yfazqb.com

[E22] 字节长度与字符长度
来源：http://xii.fktsv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pqr.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bwd.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jta.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdm.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zvg.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hju.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://crp.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rfw.ehwqpu.com

================================================================================
来源：http://vuy.zhijiandao.cn

F. 文件与目录
来源：http://krp.yj20258888.top

================================================================================
来源：http://wbe.yangfankeji.com

[F01] 读取整个文件
来源：http://lfj.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://poy.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://ory.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mww.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ufb.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dij.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://naq.mhx1999.top

Ruby: File.read("a.txt")
来源：http://pxg.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://zoj.yfazqb.com

[F02] 逐行读取文件
来源：http://tik.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tow.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uzi.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nrh.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lsi.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hkg.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ycv.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lez.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fgg.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://zpr.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdr.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qwh.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nhj.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://czt.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dvk.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://giz.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://iyp.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xgv.sxryk.cn

[F04] 追加写入文件
来源：http://zam.yfazqb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kan.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mxu.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://snl.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oed.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sbx.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qyv.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dxk.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wju.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://gun.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cjc.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://ivb.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://whv.gzhubu.top

TS:   fs.existsSync("a.txt")
来源：http://cdu.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yxf.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sub.wangdashe.top

Ruby: File.exist?("a.txt")
来源：http://dmw.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://tyo.fehbvm.com

[F06] 删除文件
来源：http://wrg.yongpay.top

Py:   os.remove("a.txt")
来源：http://toc.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://xtb.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://dtn.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://poy.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://txu.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://eud.zhengqikj.top

Ruby: File.delete("a.txt")
来源：http://dmf.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://kfn.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://pta.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lny.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aom.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xms.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pja.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mpd.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ijy.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cui.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://edi.tarul.cn

[F08] 遍历目录
来源：http://eac.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dfh.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wnm.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://nik.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://jaz.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://apg.mhx1999.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sns.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://glk.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://jjm.sufxvd.cn

[F09] 获取文件大小
来源：http://jna.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://ccs.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://xgq.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://yeu.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://bme.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://gyd.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xpt.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://hdk.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://ysb.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://yan.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wdd.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qvm.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jzi.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://ydk.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://den.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://etc.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dli.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://msc.ctjpmb.com

[F11] 复制与移动文件
来源：http://ipk.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://idb.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ytf.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osu.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgt.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://awu.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xss.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://upp.nanxinkj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fyx.nanxinkj.top

[F12] CSV 读写
来源：http://xae.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kfw.yfazqb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgj.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gkk.yuxming.cn

TS:   // 同上
来源：http://cft.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhs.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://usx.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://azl.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zkw.52xcode.cn

================================================================================
来源：http://omr.52xcode.cn

G. 面向对象
来源：http://axb.ywan-chungtsiang.top

================================================================================
来源：http://uyh.zhixingplan.top

[G01] 定义类
来源：http://hds.chenlongwang.top

Py:   class User: pass
来源：http://kiv.tian-w.cn

PHP:  class User {}
来源：http://hye.yj20258888.top

JS:   class User {}
来源：http://bwh.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://zua.yonumen.top

Java: class User {}
来源：http://sft.zdqjudy.top

Go:   type User struct { Name string }
来源：http://nlk.jlsjyb.cn

Ruby: class User; end
来源：http://zrh.shangyingyoupin.top

C#:   class User {}
来源：http://jld.pycfn.com

[G02] 构造函数
来源：http://gzv.jianghu66.top

Py:   def __init__(self, name): self.name = name
来源：http://pge.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://nag.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://esn.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://ule.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://pjm.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vjn.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://riz.tanke756.top

C#:   public User(string name) { Name = name; }
来源：http://kgn.zhixingplan.top

[G03] 实例属性
来源：http://rjb.hongshengwenyu.top

Py:   self.name = "x"
来源：http://njr.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://tar.yonumen.top

JS:   this.name = "x";
来源：http://wip.chenlongwang.top

TS:   name: string = "x";
来源：http://goo.nanxuanxn.top

Java: private String name;
来源：http://cql.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dmz.sufxvd.cn

Ruby: @name = "x"
来源：http://lgb.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://pkz.hesvh.cn

[G04] 定义方法
来源：http://kfy.andypj.xyz

Py:   def greet(self): return self.name
来源：http://rpw.shanyushiyangkeji.top


<!-- 参考信息 -->