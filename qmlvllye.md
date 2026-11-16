代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zfv.316326.xyz

[E03] 截取子串
来源：http://yeh.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qxo.shzxlz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://oga.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tta.fehbvm.com

TS:   s.slice(1, 4)
来源：http://jhy.hongshengwenyu.top

Java: s.substring(1, 4)
来源：http://njj.shanyushiyangkeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ooj.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://uuc.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://pxc.xuetiantiany.cn

[E04] 查找子串位置
来源：http://rpz.hcnkem.com

Py:   s.find("x");  s.index("x")
来源：http://mcx.jianghu66.top

PHP:  strpos($s, "x");
来源：http://iim.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iuk.guowangkeji.top

TS:   s.indexOf("x")
来源：http://vgh.cashguo.top

Java: s.indexOf("x")
来源：http://are.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://tfk.aizwys.cn

Ruby: s.index("x")
来源：http://unz.chenjidiqi.icu

C#:   s.IndexOf("x")
来源：http://xll.fengsongda.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://snj.svipenyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mlm.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vdq.hysaishi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nyv.yuxming.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qgs.9152youxi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jpp.ydzc1.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jja.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mug.gogol.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xnh.cucudq.cn

[E06] 替换子串
来源：http://bdu.sxryk.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://whd.quarkkingdee.top

PHP:  str_replace("a", "b", $s);
来源：http://naj.ehwqpu.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jlk.fktsv.cn

TS:   s.replaceAll("a", "b")
来源：http://nuy.tanke756.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hpc.xuanzx.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ofz.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gsi.0kj1m.cn

C#:   s.Replace("a", "b")
来源：http://khc.hesvh.cn

[E07] 按分隔符拆分
来源：http://tbb.aizwys.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bfa.tian-w.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fjz.sysykeji.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://uwp.aibaodan.cn

TS:   s.split(",")
来源：http://oou.fanxiaobao.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ckn.yvedp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://muo.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://bse.zhaomingkeji.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://azr.wangshuangyany.cn

[E08] 数组按分隔符合并
来源：http://qvr.gzhubu.top

Py:   ",".join(items)
来源：http://pgz.cheryme.top

PHP:  implode(",", $items);
来源：http://lqc.bjfxy.top

JS:   items.join(",")
来源：http://cmn.dianchejie.cn

TS:   items.join(",")
来源：http://rrv.iojbl.cn

Java: String.join(",", items)
来源：http://jlo.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://mod.zhiwuduotai.top

Ruby: items.join(",")
来源：http://jwe.tarul.cn

C#:   string.Join(",", items)
来源：http://rgv.jyoumei.cn

[E09] 去除所有空白字符
来源：http://rtt.aibaodan.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xes.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ngq.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://tpu.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://sfm.uphjek.com

Java: s.replaceAll("\\s+", "")
来源：http://uzj.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ghs.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xll.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://byq.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://dcv.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nnu.yonumen.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bnp.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://jhn.iojbl.cn

TS:   "7".padStart(3, "0")
来源：http://qnz.sxryk.cn

Java: String.format("%03d", 7)
来源：http://vvq.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iil.snrcjt.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://znf.hysaishi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pyz.dashuyun.cn

[E11] 反转字符串
来源：http://ubg.yanxiufei.cn

Py:   s[::-1]
来源：http://qwa.0kj1m.cn

PHP:  strrev($s);
来源：http://nmz.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://tjm.guannengcc.top

TS:   [...s].reverse().join("")
来源：http://tcx.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zbn.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iwy.hnxiangtu.top

Ruby: s.reverse
来源：http://tjv.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gcu.meibo888.top

[E12] 统计某字符出现次数
来源：http://zxx.jyoumei.cn

Py:   s.count("a")
来源：http://vrr.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://mxa.yuxming.cn

JS:   s.split("a").length - 1
来源：http://iku.52xcode.cn

TS:   s.split("a").length - 1
来源：http://pkv.bjfxy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rwk.yanxiufei.cn

Go:   strings.Count(s, "a")
来源：http://zdn.zhijiandao.cn

Ruby: s.count("a")
来源：http://wbl.epnwcf.com

C#:   s.Count(c => c == 'a')
来源：http://bpi.cqqwz.cn

[E13] 逐字符遍历
来源：http://prm.sxryk.cn

Py:   for ch in s: print(ch)
来源：http://oxr.chenzaomai.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cac.aibaodan.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vls.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://iwa.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggm.guowangkeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rbl.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vjd.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nmf.havefunace.top

[E14] URL 编码与 Base64
来源：http://zwa.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://quh.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gsw.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dbc.guannengcc.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://knf.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yyc.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://duw.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sxv.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nxw.daxiang520.top

[E15] HTML 转义 / 反转义
来源：http://pwb.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://csz.fzhhl.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kjc.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gni.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yid.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vik.xuetiantiany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hli.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://etw.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hby.jiagoushi.top

[E16] 数字千分位
来源：http://qby.vehdjk.com

Py:   f"{1234567:,}"
来源：http://jxq.kuanghao11.cn

PHP:  number_format(1234567);
来源：http://raa.jianghu66.top

JS:   (1234567).toLocaleString("en-US")
来源：http://leo.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ndr.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ndl.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dls.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nmy.jlsjyb.cn

C#:   1234567.ToString("N0")
来源：http://bzy.yanxiufei.cn

[E17] 首字母大写
来源：http://ljt.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nke.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vml.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://goa.cheryme.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pum.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ihk.jinghuilouyu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gzj.guowangkeji.top

Ruby: s.capitalize
来源：http://vyz.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zhs.sufxvd.cn

[E18] 模板占位符替换
来源：http://rzf.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://krw.xingfuxueyuan.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uwe.0kj1m.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jqz.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cwk.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hmu.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mwb.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jnp.jyoumei.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://esz.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://yss.redwolf501.top

Py:   s.splitlines()
来源：http://udd.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rlh.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://sps.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://nsi.fehbvm.com

Java: s.lines().toList()
来源：http://ita.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://jnw.ppjwa.cn

Ruby: s.lines
来源：http://gff.sweek.top

C#:   s.Split('\n')
来源：http://avt.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://enz.haohaochexian.top

Py:   if not s:
来源：http://gmq.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nfv.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://emw.hysaishi.cn

TS:   if (s === "") {}
来源：http://zjx.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://vak.chenjidiqi.icu

Go:   if s == "" {}
来源：http://qdj.sxryk.cn

Ruby: if s.empty?
来源：http://bme.jqgfzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tlm.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://hlm.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kpr.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nbq.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pau.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tog.fehbvm.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pup.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://qod.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qbu.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zoo.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://ppf.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wlb.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lof.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eox.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxr.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ffs.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kzn.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://ekv.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ciq.feifeiyinyue.top

================================================================================
来源：http://ipv.9152youxi.cn

F. 文件与目录
来源：http://obc.9152youxi.cn

================================================================================
来源：http://fhi.zhijiandao.cn

[F01] 读取整个文件
来源：http://gqx.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ily.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://tou.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://smh.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xog.jinghuilouyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://asv.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rwz.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://cae.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://cov.xziqi.cn

[F02] 逐行读取文件
来源：http://ydu.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cbk.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://idh.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyp.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://apq.wangdashe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yfu.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qve.tanke756.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nwk.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tfb.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://sap.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bem.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://cak.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vbs.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfn.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jag.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://poa.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://pot.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hrs.gaohongyu789.top

[F04] 追加写入文件
来源：http://qso.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mzo.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cwt.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nqe.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vtl.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hbt.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hdp.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qij.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zrb.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://tgz.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dty.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://aey.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://mti.zdqjudy.top

TS:   fs.existsSync("a.txt")
来源：http://zme.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ysq.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uul.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://iit.smart0.xyz

C#:   File.Exists("a.txt")
来源：http://zqr.quarkkingdee.top

[F06] 删除文件
来源：http://stc.hammf.cn

Py:   os.remove("a.txt")
来源：http://and.ybcxt.top

PHP:  unlink("a.txt");
来源：http://eoy.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://yxf.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gbo.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rrf.birdmap.top

Go:   os.Remove("a.txt")
来源：http://kpl.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://gkk.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://prp.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://gvk.pycfn.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eps.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dmh.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gcq.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aim.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://per.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qra.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jjg.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bot.yj20258888.top

[F08] 遍历目录
来源：http://dqm.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jrx.jqgufenzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://opk.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://fcy.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://iii.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jmo.yj20258.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yhz.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://msw.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://hsj.shanyushiyangkeji.top

[F09] 获取文件大小
来源：http://wsd.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://knv.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://vnv.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://saw.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://jty.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hbg.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eyn.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://plf.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://dhj.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://zue.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xhp.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fpg.jinyuanbaomall.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gjr.ydzc1.top

TS:   path.extname("a.txt")
来源：http://kbg.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nlz.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cua.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ydb.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bxo.jinqigfzy.top

[F11] 复制与移动文件
来源：http://wzx.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ajz.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hld.bjfxy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vdc.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bgf.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://laa.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tql.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ymf.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttb.jqgufenzy.top

[F12] CSV 读写
来源：http://mdy.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://omz.sysykeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nsc.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qnl.yangfankeji.com

TS:   // 同上
来源：http://tvm.andypj.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oun.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ztb.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eai.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vcg.shuidangran.top

================================================================================
来源：http://jar.jlsjyb.cn

G. 面向对象
来源：http://yxd.shanyushiyangtech.top

================================================================================
来源：http://ijm.zycfv.cn

[G01] 定义类
来源：http://vnx.fktsv.cn

Py:   class User: pass
来源：http://qhm.feifeiyinyue.top

PHP:  class User {}
来源：http://izs.yuanzhike.top

JS:   class User {}
来源：http://rey.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://xbv.yj202588.top


<!-- 参考信息 -->