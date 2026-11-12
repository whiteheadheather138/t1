代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://ujm.gzhubu.top

C#:   s.Substring(1, 3)
来源：http://eon.jqgfzy.top

[E04] 查找子串位置
来源：http://qrs.nanxuanxn.top

Py:   s.find("x");  s.index("x")
来源：http://qap.daria6918.cn

PHP:  strpos($s, "x");
来源：http://ddj.hysaishi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbn.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://hjb.zhijiandao.cn

Java: s.indexOf("x")
来源：http://awb.xuetiantiany.cn

Go:   strings.Index(s, "x")
来源：http://oql.tian-w.cn

Ruby: s.index("x")
来源：http://jyg.hnqzz.top

C#:   s.IndexOf("x")
来源：http://fwf.shanyushiyangtech.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mla.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gpo.daria6918.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xyx.hesvh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zcy.sufxvd.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cvl.fktsv.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ngj.fanxiaobao.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://luz.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rzg.xinyue.icu

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bvq.ywan-chungtsiang.top

[E06] 替换子串
来源：http://kws.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zbx.yuxming.cn

PHP:  str_replace("a", "b", $s);
来源：http://hqm.bjfxy.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ooe.gogol.net.cn

TS:   s.replaceAll("a", "b")
来源：http://hsw.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kjw.gotoacloud.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nbn.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bve.zhengqikj.top

C#:   s.Replace("a", "b")
来源：http://qsr.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://hbv.nanxuanxn.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pyt.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tup.tarul.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ois.sufxvd.cn

TS:   s.split(",")
来源：http://twp.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://cab.feifeiyinyue.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pqw.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://wol.sxryk.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://feb.bbcook.cn

[E08] 数组按分隔符合并
来源：http://ezz.kuanghao11.cn

Py:   ",".join(items)
来源：http://set.havefunace.top

PHP:  implode(",", $items);
来源：http://lwb.sweek.top

JS:   items.join(",")
来源：http://tax.jiagoushi.top

TS:   items.join(",")
来源：http://afi.ehwqpu.com

Java: String.join(",", items)
来源：http://glq.epnwcf.com

Go:   strings.Join(items, ",")
来源：http://mqt.yj202588.top

Ruby: items.join(",")
来源：http://wjc.ybcxt.top

C#:   string.Join(",", items)
来源：http://uaw.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://dzw.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ven.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jqz.yueranfly.top

JS:   s.replace(/\s+/g, "")
来源：http://aqj.aizwys.cn

TS:   s.replace(/\s+/g, "")
来源：http://plu.zhongyouzk.top

Java: s.replaceAll("\\s+", "")
来源：http://fom.kuanghao11.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://has.jqgfzy.top

Ruby: s.gsub(/\s+/, "")
来源：http://bbn.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ayi.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://kra.zhaomingkeji.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ssi.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kdy.dianchejie.cn

JS:   "7".padStart(3, "0")
来源：http://mnp.bbcook.cn

TS:   "7".padStart(3, "0")
来源：http://sor.xylfe.cn

Java: String.format("%03d", 7)
来源：http://jnc.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://pkd.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vre.zdqjudy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xpx.guannengcc.top

[E11] 反转字符串
来源：http://heg.redwolf501.top

Py:   s[::-1]
来源：http://ydo.shzxlz.cn

PHP:  strrev($s);
来源：http://mgy.yj20258.top

JS:   [...s].reverse().join("")
来源：http://vpv.0kj1m.cn

TS:   [...s].reverse().join("")
来源：http://xqu.wangshuangyany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iaq.sxryk.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uov.zhiwuduotai.top

Ruby: s.reverse
来源：http://hyc.bbcook.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jxe.fengsongda.top

[E12] 统计某字符出现次数
来源：http://xkj.guowangkeji.top

Py:   s.count("a")
来源：http://prs.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://zck.yuxming.cn

JS:   s.split("a").length - 1
来源：http://vgc.chenlongwang.top

TS:   s.split("a").length - 1
来源：http://bcd.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ytx.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://yco.bjfxy.top

Ruby: s.count("a")
来源：http://ted.jlsjyb.cn

C#:   s.Count(c => c == 'a')
来源：http://lku.daria6918.cn

[E13] 逐字符遍历
来源：http://ohl.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://rap.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hso.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hwo.redwolf501.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ald.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://cyk.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dpw.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://dst.yj20258.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://akt.wangdashe.top

[E14] URL 编码与 Base64
来源：http://aib.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mfv.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://ofc.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ofu.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oom.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dup.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://unm.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pmy.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yzx.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://aey.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lds.tarul.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iyi.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://avq.guowangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fwc.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xoa.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yma.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uok.sysykeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xdj.tarul.cn

[E16] 数字千分位
来源：http://wcj.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://jcx.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://nii.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tfy.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xka.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hui.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oft.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gzr.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://fzr.aizwys.cn

[E17] 首字母大写
来源：http://fpd.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pul.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zdm.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vyw.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vsz.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zbb.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vvz.jqgfzy.top

Ruby: s.capitalize
来源：http://kgk.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wgl.vehdjk.com

[E18] 模板占位符替换
来源：http://thh.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qes.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mjh.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xrk.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ayy.jianghu66.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://crz.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rww.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nfl.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://emr.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://yrk.zhixingplan.top

Py:   s.splitlines()
来源：http://aye.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xmz.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://fcx.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://glx.ybcxt.top

Java: s.lines().toList()
来源：http://ity.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://bqt.jqgufenzy.top

Ruby: s.lines
来源：http://dmt.jyoumei.cn

C#:   s.Split('\n')
来源：http://avp.yuxming.cn

[E20] 判断字符串是否为空
来源：http://nfa.tanke756.top

Py:   if not s:
来源：http://oaz.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zkh.shzxlz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gzr.cqqwz.cn

TS:   if (s === "") {}
来源：http://vzi.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://xup.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://acn.ppjwa.cn

Ruby: if s.empty?
来源：http://lru.bjfxy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://grx.c1oappe.top

[E21] 超长截断加省略号
来源：http://cxz.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pyf.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kyw.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xmc.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbb.zhongyouzk.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sfb.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://hfb.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iio.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rqm.iojbl.cn

[E22] 字节长度与字符长度
来源：http://ell.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bzi.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aac.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vjs.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iaj.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vjk.shanyushiyangtech.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fph.hcnkem.com

Ruby: s.bytesize;  s.length
来源：http://vdm.zhijiandao.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://klg.316326.xyz

================================================================================
来源：http://nfs.9152youxi.cn

F. 文件与目录
来源：http://buh.wangshuangyany.cn

================================================================================
来源：http://bqx.xinyue.icu

[F01] 读取整个文件
来源：http://nxy.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iwr.redwolf501.top

PHP:  file_get_contents("a.txt");
来源：http://vbw.xuanzx.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://htk.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://okb.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rka.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fvc.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://cor.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://tfw.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://nkw.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oxb.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bvd.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jpo.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfu.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ghc.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gyd.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tkf.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jkf.0kj1m.cn

[F03] 写入文件（覆盖）
来源：http://xiz.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://psw.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rry.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhh.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubb.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://toa.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://svi.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://gsq.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nqd.uphjek.com

[F04] 追加写入文件
来源：http://rrk.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wkz.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nfr.xuanzx.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aei.zhaomingkeji.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nij.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vow.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fcl.xinyue.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tlh.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tla.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://yet.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sff.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://dbj.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://agd.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://hbt.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xav.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xyn.havefunace.top

Ruby: File.exist?("a.txt")
来源：http://jjk.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://koy.52xcode.cn

[F06] 删除文件
来源：http://svm.redwolf501.top

Py:   os.remove("a.txt")
来源：http://poy.yonumen.top

PHP:  unlink("a.txt");
来源：http://ktp.zhengqikj.top

JS:   fs.unlinkSync("a.txt")
来源：http://kah.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aml.ctjpmb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtu.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://wul.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://sne.nwbrower.top

C#:   File.Delete("a.txt");
来源：http://wgu.quarkkingdee.top

[F07] 创建目录（含多级）
来源：http://syw.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyo.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nks.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nya.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ewp.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ntj.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qfz.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yoq.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ftv.zhiwuduotai.top

[F08] 遍历目录
来源：http://dhz.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xzo.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dkq.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://oii.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://lfq.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oez.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ohu.jiagoushi.top

Ruby: Dir.children("dir")
来源：http://gxv.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://jwn.cqqwz.cn

[F09] 获取文件大小
来源：http://sdy.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://bvc.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://jyf.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://uyi.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://kfn.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://rqu.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wpn.nanxinkj.top

Ruby: File.size("a.txt")
来源：http://wfp.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://ndh.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://bzl.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qcn.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zse.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sts.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://muo.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lvv.zhaomingkeji.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fgf.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ang.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fxe.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://gjv.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uyw.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nnh.sweek.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zoh.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://frz.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nzl.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yze.zhaomingkeji.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfb.zhengqikj.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wtq.kuanghao11.cn

[F12] CSV 读写
来源：http://him.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fwl.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qwx.xylfe.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hag.zhiwuduotai.top

TS:   // 同上
来源：http://rya.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hft.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kdo.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tyk.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ykp.svipenyu.cn

================================================================================
来源：http://cnz.52xcode.cn

G. 面向对象
来源：http://brl.jiagoushi.top

================================================================================
来源：http://lxr.yueranfly.top

[G01] 定义类
来源：http://chj.jinyuanbaomall.cn

Py:   class User: pass
来源：http://yfv.zhijiandao.cn

PHP:  class User {}
来源：http://orb.dashuyun.cn

JS:   class User {}
来源：http://wug.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://ypc.zhaomingkeji.xyz

Java: class User {}
来源：http://cpw.ctjpmb.com

Go:   type User struct { Name string }
来源：http://yiv.hfpthk.cn

Ruby: class User; end
来源：http://vky.bjfxy.top

C#:   class User {}
来源：http://boc.ywan-chungtsiang.top

[G02] 构造函数
来源：http://hdd.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://etg.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://vwf.iojbl.cn

JS:   constructor(name) { this.name = name; }
来源：http://tpp.zdqjudy.top


<!-- 参考信息 -->