代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://zfq.snrcjt.cn

C#:   s.Substring(1, 3)
来源：http://eep.yj20258.top

[E04] 查找子串位置
来源：http://nmy.dashuyun.cn

Py:   s.find("x");  s.index("x")
来源：http://uix.xingfuxueyuan.xyz

PHP:  strpos($s, "x");
来源：http://rup.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kwz.yongpay.top

TS:   s.indexOf("x")
来源：http://wfc.yj202588.top

Java: s.indexOf("x")
来源：http://zhb.hesvh.cn

Go:   strings.Index(s, "x")
来源：http://pzw.havefunace.top

Ruby: s.index("x")
来源：http://zvg.xuetiantiany.cn

C#:   s.IndexOf("x")
来源：http://gmf.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wuj.xziqi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gwm.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vrq.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pgt.zdbjq.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://veu.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nuh.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hhp.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lja.andypj.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xtw.hnxiangtu.top

[E06] 替换子串
来源：http://iee.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xcm.hfpthk.cn

PHP:  str_replace("a", "b", $s);
来源：http://quk.snrcjt.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jap.ywan-chungtsiang.top

TS:   s.replaceAll("a", "b")
来源：http://bsl.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fcy.yfazqb.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bty.hnxiangtu.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oqf.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://cie.sxryk.cn

[E07] 按分隔符拆分
来源：http://rep.ydjk.org.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yhw.ydjk.org.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hon.kuanghao11.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cbf.ydzc1.top

TS:   s.split(",")
来源：http://iza.redwolf501.top

Java: s.split(",");  s.split("\\s+")
来源：http://ptt.hcnkem.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://phe.jlsjyb.cn

Ruby: s.split(",");  s.split
来源：http://zsq.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vgq.hammf.cn

[E08] 数组按分隔符合并
来源：http://uye.guowangkeji.top

Py:   ",".join(items)
来源：http://lvw.fktsv.cn

PHP:  implode(",", $items);
来源：http://rdd.hammf.cn

JS:   items.join(",")
来源：http://lwk.xuanzx.com

TS:   items.join(",")
来源：http://nfb.cashguo.top

Java: String.join(",", items)
来源：http://yek.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://jdz.jianghu66.top

Ruby: items.join(",")
来源：http://vce.wangdashe.top

C#:   string.Join(",", items)
来源：http://lew.feifeiyinyue.top

[E09] 去除所有空白字符
来源：http://efx.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nkg.gaohongyu789.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://scx.jinqigufen.top

JS:   s.replace(/\s+/g, "")
来源：http://nhe.cheryme.top

TS:   s.replace(/\s+/g, "")
来源：http://jpj.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://waw.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://thw.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://fmj.jlsjyb.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ict.52xcode.cn

[E10] 左侧补零 / 定长填充
来源：http://jrg.cqqwz.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hnt.guannengcc.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kry.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://cxv.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://kda.yonumen.top

Java: String.format("%03d", 7)
来源：http://jgd.vqdsnc.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zkz.zhiwuduotai.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hdt.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://icz.zhiwuduotai.top

[E11] 反转字符串
来源：http://laa.hammf.cn

Py:   s[::-1]
来源：http://kdx.sufxvd.cn

PHP:  strrev($s);
来源：http://nxz.hfpthk.cn

JS:   [...s].reverse().join("")
来源：http://kms.shzxlz.cn

TS:   [...s].reverse().join("")
来源：http://zqp.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wjn.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vol.yfazqb.com

Ruby: s.reverse
来源：http://lps.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://kxq.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://vxv.jianghu66.top

Py:   s.count("a")
来源：http://yvp.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://umt.smart0.xyz

JS:   s.split("a").length - 1
来源：http://edz.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://bcw.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zos.nanxinkj.top

Go:   strings.Count(s, "a")
来源：http://xmj.tarul.cn

Ruby: s.count("a")
来源：http://ggz.chenlongwang.top

C#:   s.Count(c => c == 'a')
来源：http://gct.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://odt.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://hmu.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://byn.ybcxt.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://psf.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://uwx.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rec.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mvw.meibo888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vpi.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kgg.jqgfzy.top

[E14] URL 编码与 Base64
来源：http://lav.daxiang520.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://axx.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dwy.gaohongyu789.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tpg.guowangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sux.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dsh.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gdu.snrcjt.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zro.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ybc.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://pal.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://hbl.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eth.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ncn.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fmb.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ccw.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://sya.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hco.0kj1m.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cfv.fanxiaobao.xyz

[E16] 数字千分位
来源：http://oov.gzhubu.top

Py:   f"{1234567:,}"
来源：http://uep.dashuyun.cn

PHP:  number_format(1234567);
来源：http://odj.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://phy.shanyushiyangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hxs.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fnq.dianchejie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrz.yuanzhike.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kcx.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://vga.yj202588.top

[E17] 首字母大写
来源：http://bnm.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ung.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kdm.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkc.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://klj.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://thg.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zih.birdmap.top

Ruby: s.capitalize
来源：http://fey.fengsongda.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gwa.aizwys.cn

[E18] 模板占位符替换
来源：http://ntv.xziqi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://upm.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://imq.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ejb.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://awh.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ifd.jinqigfzy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tjh.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sog.ywan-chungtsiang.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blh.redwolf501.top

[E19] 多行文本按行拆分
来源：http://qhm.gotoacloud.top

Py:   s.splitlines()
来源：http://aej.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nqh.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://buo.hysaishi.cn

TS:   s.split(/\r?\n/)
来源：http://ffl.fzhhl.top

Java: s.lines().toList()
来源：http://isp.shanyushiyangtech.top

Go:   strings.Split(s, "\n")
来源：http://ova.fzhhl.top

Ruby: s.lines
来源：http://kvv.shzxlz.cn

C#:   s.Split('\n')
来源：http://ygl.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://ymp.ehwqpu.com

Py:   if not s:
来源：http://jlv.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ctx.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sit.daxiang520.top

TS:   if (s === "") {}
来源：http://dut.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://phs.yongpay.top

Go:   if s == "" {}
来源：http://tst.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://ffd.daxiang520.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czl.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://kng.xuanzx.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wsl.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jjg.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://znx.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bzq.sweek.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gam.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://zjg.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jqr.jinqigfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kjm.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://gnw.jyoumei.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wcd.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qqz.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://een.bjfxy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qhy.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://git.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rge.pengpengdd.cyou

Ruby: s.bytesize;  s.length
来源：http://vun.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ois.9152youxi.cn

================================================================================
来源：http://axt.epnwcf.com

F. 文件与目录
来源：http://ktg.bjfxy.top

================================================================================
来源：http://lkz.c1oappe.top

[F01] 读取整个文件
来源：http://ujv.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yyj.yongpay.top

PHP:  file_get_contents("a.txt");
来源：http://xom.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://huk.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sdx.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://yra.xingfuxueyuan.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vmu.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://afn.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://dpg.c1oappe.top

[F02] 逐行读取文件
来源：http://pdl.yj20258888.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zpt.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://swl.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fxf.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tmv.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jwb.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nut.mhx1999.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://muo.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cdf.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://bpf.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://odn.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ztr.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://riz.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mcd.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rji.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zae.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://xgw.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jrg.ppjwa.cn

[F04] 追加写入文件
来源：http://seh.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vrn.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sqk.jinqigufen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qce.kuanghao11.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dnz.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://avz.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vtt.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zzh.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ztt.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://vpt.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ijw.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://gir.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://pwr.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://rvd.epnwcf.com

Java: Files.exists(Path.of("a.txt"))
来源：http://rur.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ket.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://lpl.sweek.top

C#:   File.Exists("a.txt")
来源：http://urk.quarkkingdee.top

[F06] 删除文件
来源：http://jzv.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://eyy.zhoulong.xyz

PHP:  unlink("a.txt");
来源：http://yxa.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://rby.hnxiangtu.top

TS:   fs.unlinkSync("a.txt")
来源：http://ukw.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ocv.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://teb.cashguo.top

Ruby: File.delete("a.txt")
来源：http://shj.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://gry.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://jay.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wzv.ybcxt.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zsf.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://srp.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ghe.xuetiantiany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dom.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ppb.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fbw.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eey.hammf.cn

[F08] 遍历目录
来源：http://khw.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nwx.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wrv.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://sur.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://qph.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://svj.52xcode.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oci.tarul.cn

Ruby: Dir.children("dir")
来源：http://url.hnxiangtu.top

C#:   Directory.GetFiles("dir")
来源：http://wlk.cucudq.cn

[F09] 获取文件大小
来源：http://gco.zhijiandao.cn

Py:   os.path.getsize("a.txt")
来源：http://gja.zhixingplan.top

PHP:  filesize("a.txt");
来源：http://bon.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://noa.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://jef.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://bkx.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mhd.gzhubu.top

Ruby: File.size("a.txt")
来源：http://ggs.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://vux.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://ryq.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lza.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ycd.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vid.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://ycj.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ikn.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://meb.tanke756.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yja.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jcu.andypj.xyz

[F11] 复制与移动文件
来源：http://mwp.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qau.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bzo.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://say.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mdv.daria6918.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qao.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xjd.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cte.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tgj.hnqzz.top

[F12] CSV 读写
来源：http://dvq.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bmq.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rmx.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ipy.havefunace.top

TS:   // 同上
来源：http://yei.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://seq.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ftk.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rxf.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://aat.jinghuilouyu.cn

================================================================================
来源：http://ylj.hcnkem.com

G. 面向对象
来源：http://lsc.chenlongwang.top

================================================================================
来源：http://auy.cashguo.top

[G01] 定义类
来源：http://zlu.andypj.xyz

Py:   class User: pass
来源：http://ohq.9152youxi.cn

PHP:  class User {}
来源：http://rtc.jiagoushi.top

JS:   class User {}
来源：http://unc.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://sfm.bjfxy.top

Java: class User {}
来源：http://krz.xuanzx.com

Go:   type User struct { Name string }
来源：http://zkx.gzhubu.top

Ruby: class User; end
来源：http://xkk.yvedp.cn

C#:   class User {}
来源：http://fns.ehwqpu.com

[G02] 构造函数
来源：http://muq.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://rsx.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://rwq.gotoacloud.top

JS:   constructor(name) { this.name = name; }
来源：http://kyz.316326.xyz


<!-- 参考信息 -->