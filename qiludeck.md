代发 wailian999

PHP:  strpos($s, "x");
来源：http://hux.redwolf501.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://csf.zdbjq.cn

TS:   s.indexOf("x")
来源：http://hdu.ybcxt.top

Java: s.indexOf("x")
来源：http://jav.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://xjs.xziqi.cn

Ruby: s.index("x")
来源：http://ate.shuidangran.top

C#:   s.IndexOf("x")
来源：http://yif.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://dye.vqdsnc.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tvh.bjfxy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rae.haohaochexian.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qln.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hfo.jinyuanbaomall.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yau.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://exq.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qra.yuxming.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cyp.zhaomingkeji.xyz

[E06] 替换子串
来源：http://njx.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nmt.yuanzhike.top

PHP:  str_replace("a", "b", $s);
来源：http://zcu.jyoumei.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xhr.cdnleiting.top

TS:   s.replaceAll("a", "b")
来源：http://mtp.hnqzz.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rdp.kuanghao11.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://eed.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gpo.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://ctd.yueranfly.top

[E07] 按分隔符拆分
来源：http://tme.zhengqikj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lgw.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://buv.tanke756.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://pax.yfazqb.com

TS:   s.split(",")
来源：http://udb.feifeiyinyue.top

Java: s.split(",");  s.split("\\s+")
来源：http://cuk.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uic.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://vio.uphjek.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gvi.yueranfly.top

[E08] 数组按分隔符合并
来源：http://iem.cqqwz.cn

Py:   ",".join(items)
来源：http://nsb.9152youxi.cn

PHP:  implode(",", $items);
来源：http://pwr.ydzc1.top

JS:   items.join(",")
来源：http://mao.zhengqikj.top

TS:   items.join(",")
来源：http://ynk.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://bmc.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://nlj.cashguo.top

Ruby: items.join(",")
来源：http://los.jlsjyb.cn

C#:   string.Join(",", items)
来源：http://rbv.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://nfd.iojbl.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://feo.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://abv.ydjk.org.cn

JS:   s.replace(/\s+/g, "")
来源：http://azl.gogol.net.cn

TS:   s.replace(/\s+/g, "")
来源：http://rqk.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://ztl.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fxz.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://loh.tian-w.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nwh.snrcjt.cn

[E10] 左侧补零 / 定长填充
来源：http://hwg.ivvv.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kwo.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kjn.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://efm.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://idl.yonumen.top

Java: String.format("%03d", 7)
来源：http://oye.birdmap.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tjq.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ldy.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bzx.havefunace.top

[E11] 反转字符串
来源：http://pvb.gotoacloud.top

Py:   s[::-1]
来源：http://rgy.jyoumei.cn

PHP:  strrev($s);
来源：http://awv.tianlin.xyz

JS:   [...s].reverse().join("")
来源：http://klu.hcnkem.com

TS:   [...s].reverse().join("")
来源：http://fkf.jinqigufen.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zhl.zycfv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://moi.wangdashe.top

Ruby: s.reverse
来源：http://oti.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yeh.sxryk.cn

[E12] 统计某字符出现次数
来源：http://tpx.chenzaomai.com

Py:   s.count("a")
来源：http://efm.pycfn.com

PHP:  substr_count($s, "a");
来源：http://gto.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://kay.shzxlz.cn

TS:   s.split("a").length - 1
来源：http://oqt.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ril.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://mke.hnxiangtu.top

Ruby: s.count("a")
来源：http://flh.316326.xyz

C#:   s.Count(c => c == 'a')
来源：http://itj.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://viu.havefunace.top

Py:   for ch in s: print(ch)
来源：http://wyu.ydzc1.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kzt.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://htn.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kke.quarkkingdee.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ttx.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qit.jinghuilouyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qlk.0kj1m.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tro.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://loj.xuanzx.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fgb.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rns.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://htr.zhaomingkeji.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uzi.zhiwuduotai.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lrj.hysaishi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ubg.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nsg.yongpay.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://you.shanyushiyangtech.top

[E15] HTML 转义 / 反转义
来源：http://iga.haohaochexian.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sly.hcnkem.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyu.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://apm.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kqj.cashguo.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqy.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rgp.gaohongyu789.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tqw.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ght.xinyue.icu

[E16] 数字千分位
来源：http://hbw.sweek.top

Py:   f"{1234567:,}"
来源：http://uzs.ydzc1.top

PHP:  number_format(1234567);
来源：http://ldd.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rjh.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xbc.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fws.ehwqpu.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oeh.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dqv.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://pzn.cdnleiting.top

[E17] 首字母大写
来源：http://qap.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jle.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://kgj.tian-w.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mer.chenzaomai.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xei.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dfc.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nwq.fehbvm.com

Ruby: s.capitalize
来源：http://hkl.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pbe.aibaodan.cn

[E18] 模板占位符替换
来源：http://tjg.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ysh.hnxiangtu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ghb.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xbc.jiagoushi.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jhu.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yog.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vkn.ehwqpu.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mzi.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://axw.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://keg.ctjpmb.com

Py:   s.splitlines()
来源：http://cwo.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://itr.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://zew.gotoacloud.top

TS:   s.split(/\r?\n/)
来源：http://znz.ppjwa.cn

Java: s.lines().toList()
来源：http://loh.ydjk.org.cn

Go:   strings.Split(s, "\n")
来源：http://fzg.xylfe.cn

Ruby: s.lines
来源：http://cbg.mhx1999.top

C#:   s.Split('\n')
来源：http://gah.xuanzx.com

[E20] 判断字符串是否为空
来源：http://iuq.yonumen.top

Py:   if not s:
来源：http://rhb.tanke756.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nio.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nkp.shanyushiyangkeji.top

TS:   if (s === "") {}
来源：http://ugo.chenjidiqi.icu

Java: if (s.isEmpty()) {}
来源：http://ywa.vehdjk.com

Go:   if s == "" {}
来源：http://qbi.snrcjt.cn

Ruby: if s.empty?
来源：http://ltx.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sov.bjfxy.top

[E21] 超长截断加省略号
来源：http://huz.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bga.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wqc.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cuj.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://soa.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ljg.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://tdf.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fzv.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ban.316326.xyz

[E22] 字节长度与字符长度
来源：http://vze.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iwc.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkx.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://emf.cdnleiting.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rgx.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uxk.9152youxi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ypt.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://zxc.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://smk.sufxvd.cn

================================================================================
来源：http://imc.fehbvm.com

F. 文件与目录
来源：http://aqg.yj20258.top

================================================================================
来源：http://cgb.ivvv.top

[F01] 读取整个文件
来源：http://jvi.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bdz.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://ibl.shanyushiyangtech.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://efx.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zlt.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://udv.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhf.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://ugi.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://xaq.zhoulong.xyz

[F02] 逐行读取文件
来源：http://cpm.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mwh.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ycr.jqgufenzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qfl.hammf.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ihz.jianghu66.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://khk.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://apx.fehbvm.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vym.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jgr.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://inn.feifeiyinyue.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blr.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bsl.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qym.yonumen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wzx.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ozh.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hva.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://had.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jhp.smart0.xyz

[F04] 追加写入文件
来源：http://uic.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jph.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hdk.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqj.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://phv.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fas.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gyn.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mns.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://djz.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://kkk.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kph.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://eso.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://ahy.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://bvz.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zmx.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://amk.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://ubv.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://pzt.chenzaomai.com

[F06] 删除文件
来源：http://ngc.316326.xyz

Py:   os.remove("a.txt")
来源：http://fti.sxryk.cn

PHP:  unlink("a.txt");
来源：http://tor.hammf.cn

JS:   fs.unlinkSync("a.txt")
来源：http://waf.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://dnq.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yem.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://roe.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://gmm.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://hvp.yonumen.top

[F07] 创建目录（含多级）
来源：http://yba.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://btb.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qbq.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hmm.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tbx.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mer.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mid.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ohq.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mxd.fengsongda.top

[F08] 遍历目录
来源：http://plq.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jwg.zhiwuduotai.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kpx.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://uyx.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://nja.bjfxy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cwc.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://wsm.yonumen.top

Ruby: Dir.children("dir")
来源：http://iwc.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://hfj.cqqwz.cn

[F09] 获取文件大小
来源：http://zkz.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://qzo.hammf.cn

PHP:  filesize("a.txt");
来源：http://iga.52xcode.cn

JS:   fs.statSync("a.txt").size
来源：http://eql.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://sac.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://wxw.yanxiufei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pen.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://kut.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://seg.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://cyj.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://buh.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ggf.guannengcc.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fwq.epnwcf.com

TS:   path.extname("a.txt")
来源：http://fja.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hrh.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ywl.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tbo.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bvb.nanxuanxn.top

[F11] 复制与移动文件
来源：http://nvs.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ixz.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://frr.shanyushiyangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zbp.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bvi.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uhi.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cay.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jim.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wef.bbcook.cn

[F12] CSV 读写
来源：http://pwq.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ljd.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gft.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qen.zdqjudy.top

TS:   // 同上
来源：http://ues.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hjl.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wel.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tsr.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ewa.shangyingyoupin.top

================================================================================
来源：http://qrm.chenlongwang.top

G. 面向对象
来源：http://zxl.tanke756.top

================================================================================
来源：http://fzq.aizwys.cn

[G01] 定义类
来源：http://jui.yueranfly.top

Py:   class User: pass
来源：http://lgb.dashuyun.cn

PHP:  class User {}
来源：http://dqd.vqdsnc.cn

JS:   class User {}
来源：http://rua.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://zbm.yfazqb.com

Java: class User {}
来源：http://nau.wangdashe.top

Go:   type User struct { Name string }
来源：http://mtl.ivvv.top

Ruby: class User; end
来源：http://zio.yj20258.top

C#:   class User {}
来源：http://skk.cheryme.top

[G02] 构造函数
来源：http://qhn.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://ifh.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://vor.hesvh.cn

JS:   constructor(name) { this.name = name; }
来源：http://boi.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://cpb.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://owx.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mcf.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://jax.jlsjyb.cn


<!-- 参考信息 -->