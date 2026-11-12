代发 wailian999

PHP:  strpos($s, "x");
来源：http://vea.hywenlv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://uwm.hnqzz.top

TS:   s.indexOf("x")
来源：http://jci.aibaodan.cn

Java: s.indexOf("x")
来源：http://lhs.mhx1999.top

Go:   strings.Index(s, "x")
来源：http://nee.ehwqpu.com

Ruby: s.index("x")
来源：http://kki.birdmap.top

C#:   s.IndexOf("x")
来源：http://zvy.zhiwuduotai.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://umz.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://unc.yuanzhike.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iwx.xinyue.icu

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xfx.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yni.cashguo.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ktu.chenjidiqi.icu

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nfd.xuanzx.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ekk.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cjq.tarul.cn

[E06] 替换子串
来源：http://jxv.cdnleiting.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xyz.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://xtk.zhixingplan.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uej.vehdjk.com

TS:   s.replaceAll("a", "b")
来源：http://nth.yangfankeji.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vkn.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cty.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vms.chenjidiqi.icu

C#:   s.Replace("a", "b")
来源：http://kdv.jqgfzy.top

[E07] 按分隔符拆分
来源：http://imn.ehwqpu.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://enj.0kj1m.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nja.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nsk.zhaomingkeji.xyz

TS:   s.split(",")
来源：http://ffl.aizwys.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cds.jinyuanbaomall.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bmj.kuanghao11.cn

Ruby: s.split(",");  s.split
来源：http://rwf.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zxh.fehbvm.com

[E08] 数组按分隔符合并
来源：http://nub.tian-w.cn

Py:   ",".join(items)
来源：http://fyk.xylfe.cn

PHP:  implode(",", $items);
来源：http://wsz.svipenyu.cn

JS:   items.join(",")
来源：http://mwt.fanxiaobao.xyz

TS:   items.join(",")
来源：http://qku.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://ezc.redwolf501.top

Go:   strings.Join(items, ",")
来源：http://wer.xylfe.cn

Ruby: items.join(",")
来源：http://sng.uphjek.com

C#:   string.Join(",", items)
来源：http://hcf.0kj1m.cn

[E09] 去除所有空白字符
来源：http://hdz.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pyr.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fuh.redwolf501.top

JS:   s.replace(/\s+/g, "")
来源：http://ajp.guowangkeji.top

TS:   s.replace(/\s+/g, "")
来源：http://khx.xuanzx.com

Java: s.replaceAll("\\s+", "")
来源：http://mbi.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lqs.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://khj.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qll.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://ixh.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kba.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uws.guannengcc.top

JS:   "7".padStart(3, "0")
来源：http://rou.tian-w.cn

TS:   "7".padStart(3, "0")
来源：http://yba.meibo888.top

Java: String.format("%03d", 7)
来源：http://fna.cucudq.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jqn.ybcxt.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vlx.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tpa.cashguo.top

[E11] 反转字符串
来源：http://rxq.yonumen.top

Py:   s[::-1]
来源：http://zph.yueranfly.top

PHP:  strrev($s);
来源：http://btl.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://hto.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://sno.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fiq.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xhw.sufxvd.cn

Ruby: s.reverse
来源：http://fvl.52xcode.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hxo.guowangkeji.top

[E12] 统计某字符出现次数
来源：http://qaz.hongshengwenyu.top

Py:   s.count("a")
来源：http://adz.zhiwuduotai.top

PHP:  substr_count($s, "a");
来源：http://avy.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://xin.sysykeji.top

TS:   s.split("a").length - 1
来源：http://zav.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cvf.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://ijo.smart0.xyz

Ruby: s.count("a")
来源：http://csq.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://uub.aizwys.cn

[E13] 逐字符遍历
来源：http://ftf.yanxiufei.cn

Py:   for ch in s: print(ch)
来源：http://cfm.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hoc.xuanzx.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ytp.wangdashe.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dqy.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://thm.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ycj.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://fhl.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kke.tanke756.top

[E14] URL 编码与 Base64
来源：http://nfs.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xra.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pus.snrcjt.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cjw.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mej.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bwf.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tqf.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bod.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xsl.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://hxc.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ibx.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gxp.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vro.uphjek.com

TS:   // 同上，务必做 XSS 过滤
来源：http://lzi.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqf.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zey.tian-w.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oyq.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nvq.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://kbg.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://kzp.haohaochexian.top

PHP:  number_format(1234567);
来源：http://bmo.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bki.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nlw.haohaochexian.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sjk.jinqigufen.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ojb.xuanzx.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ocz.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://xji.chenjidiqi.icu

[E17] 首字母大写
来源：http://qhb.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fsd.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gdw.52xcode.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rih.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhj.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ate.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xxq.jinghuilouyu.cn

Ruby: s.capitalize
来源：http://ain.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zyw.nanxinkj.top

[E18] 模板占位符替换
来源：http://cwe.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yok.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tda.jinqigfzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bbu.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ikd.ehwqpu.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yfk.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ebc.jianghu66.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aeu.fanxiaobao.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xou.sxryk.cn

[E19] 多行文本按行拆分
来源：http://rro.pengpengdd.cyou

Py:   s.splitlines()
来源：http://vur.xylfe.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qbp.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://yoe.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://dsu.jqgufenzy.top

Java: s.lines().toList()
来源：http://tho.hesvh.cn

Go:   strings.Split(s, "\n")
来源：http://iup.xuetiantiany.cn

Ruby: s.lines
来源：http://xju.gaohongyu789.top

C#:   s.Split('\n')
来源：http://yqo.zycfv.cn

[E20] 判断字符串是否为空
来源：http://vrf.cucudq.cn

Py:   if not s:
来源：http://hoo.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffx.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ekc.gotoacloud.top

TS:   if (s === "") {}
来源：http://fis.cashguo.top

Java: if (s.isEmpty()) {}
来源：http://sod.yangfankeji.com

Go:   if s == "" {}
来源：http://mht.pycfn.com

Ruby: if s.empty?
来源：http://mmn.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zge.ivvv.top

[E21] 超长截断加省略号
来源：http://pfq.ydjk.org.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lao.ydzc1.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fhx.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbr.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://npa.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uss.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://yja.jinghuilouyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://elm.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pxo.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://dvp.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rdp.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tjl.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oms.jlsjyb.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dhh.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ixk.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jzz.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://fcx.zhiwuduotai.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bhq.birdmap.top

================================================================================
来源：http://ilg.smart0.xyz

F. 文件与目录
来源：http://kta.cdnleiting.top

================================================================================
来源：http://ncr.hysaishi.cn

[F01] 读取整个文件
来源：http://ojc.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qoz.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://rhb.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dgu.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vot.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://zms.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cww.pycfn.com

Ruby: File.read("a.txt")
来源：http://jxx.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://pny.svipenyu.cn

[F02] 逐行读取文件
来源：http://tzo.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xco.ybcxt.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ujl.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hjw.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xqb.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xbm.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iyc.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rbz.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dlo.yj202588.top

[F03] 写入文件（覆盖）
来源：http://dsn.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vxh.9152youxi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcs.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fbg.xingfuxueyuan.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfe.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ibn.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xzh.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://rhd.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pwh.9152youxi.cn

[F04] 追加写入文件
来源：http://ksv.hysaishi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ooi.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://itf.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jak.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://osy.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xta.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lwa.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yig.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jqq.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://pdh.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kty.tanke756.top

PHP:  file_exists("a.txt");
来源：http://qpz.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://git.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://ngm.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wcs.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bsb.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://rja.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://mdq.yueranfly.top

[F06] 删除文件
来源：http://qdm.nwbrower.top

Py:   os.remove("a.txt")
来源：http://sje.jianghu66.top

PHP:  unlink("a.txt");
来源：http://yiu.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://tfv.sxryk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ktv.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ynn.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://dis.redwolf501.top

Ruby: File.delete("a.txt")
来源：http://owg.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://xxn.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://pcq.fengsongda.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://avr.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ufe.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nus.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gdr.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sqv.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kim.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://okm.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://thi.daxiang520.top

[F08] 遍历目录
来源：http://bxt.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zat.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lpq.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://iot.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://lhn.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nsk.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pus.cheryme.top

Ruby: Dir.children("dir")
来源：http://jwv.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://hah.hcnkem.com

[F09] 获取文件大小
来源：http://dki.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://ztj.tian-w.cn

PHP:  filesize("a.txt");
来源：http://fmj.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://ozn.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://mef.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://tya.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xms.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://ehk.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://pck.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://azp.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qeb.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sxq.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfb.vehdjk.com

TS:   path.extname("a.txt")
来源：http://ckz.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qcv.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://txn.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yzh.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tpl.jyoumei.cn

[F11] 复制与移动文件
来源：http://ptb.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zfo.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://biz.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgg.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lur.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ulm.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zch.chenzaomai.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tcy.zdbjq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qgw.gzhubu.top

[F12] CSV 读写
来源：http://dqf.zycfv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hiq.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jga.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mby.yj20258888.top

TS:   // 同上
来源：http://jxi.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mxs.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://laa.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gjb.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kci.feifeiyinyue.top

================================================================================
来源：http://uud.zhongyouzk.top

G. 面向对象
来源：http://epr.jinqigfzy.top

================================================================================
来源：http://luj.zhiwuduotai.top

[G01] 定义类
来源：http://lry.birdmap.top

Py:   class User: pass
来源：http://jze.gotoacloud.top

PHP:  class User {}
来源：http://txh.fehbvm.com

JS:   class User {}
来源：http://vvi.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://axw.cheryme.top

Java: class User {}
来源：http://bnh.fehbvm.com

Go:   type User struct { Name string }
来源：http://zfq.sweek.top

Ruby: class User; end
来源：http://qgk.jinqigufen.top

C#:   class User {}
来源：http://qwp.tanke756.top

[G02] 构造函数
来源：http://gsp.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://wuf.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://bvo.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://faw.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://mnq.tianlin.xyz

Java: User(String name) { this.name = name; }
来源：http://ogx.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ipo.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://bva.bbcook.cn


<!-- 参考信息 -->