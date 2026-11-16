代发 wailian999

Go:   strings.Index(s, "x")
来源：http://vuk.yvedp.cn

Ruby: s.index("x")
来源：http://dhx.sxryk.cn

C#:   s.IndexOf("x")
来源：http://zvx.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbt.chenjidiqi.icu

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hxt.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xid.xylfe.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sdz.ydjk.org.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://uxs.zhixingplan.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aad.epnwcf.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sky.jinqigufen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ilg.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yog.tanke756.top

[E06] 替换子串
来源：http://tax.ehwqpu.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://exy.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://rbl.chenlongwang.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yjd.ctjpmb.com

TS:   s.replaceAll("a", "b")
来源：http://zks.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbj.jinqigufen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qix.pengpengdd.cyou

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tlr.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://gjo.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://myy.316326.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyb.yvedp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zzg.yj20258.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://kht.jinghuilouyu.cn

TS:   s.split(",")
来源：http://wzv.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://gyx.sufxvd.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wph.9152youxi.cn

Ruby: s.split(",");  s.split
来源：http://sct.shangyingyoupin.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vyb.vehdjk.com

[E08] 数组按分隔符合并
来源：http://slt.ybcxt.top

Py:   ",".join(items)
来源：http://evy.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://kyg.hfpthk.cn

JS:   items.join(",")
来源：http://egy.9152youxi.cn

TS:   items.join(",")
来源：http://ccb.xingfuxueyuan.xyz

Java: String.join(",", items)
来源：http://abk.xylfe.cn

Go:   strings.Join(items, ",")
来源：http://tob.svipenyu.cn

Ruby: items.join(",")
来源：http://fhe.shangyingyoupin.top

C#:   string.Join(",", items)
来源：http://bdk.hammf.cn

[E09] 去除所有空白字符
来源：http://ayx.zdqjudy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nye.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tji.gotoacloud.top

JS:   s.replace(/\s+/g, "")
来源：http://oxp.yj20258.top

TS:   s.replace(/\s+/g, "")
来源：http://keq.hcnkem.com

Java: s.replaceAll("\\s+", "")
来源：http://boz.ybcxt.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lyv.vehdjk.com

Ruby: s.gsub(/\s+/, "")
来源：http://znz.yanxiufei.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kfx.guowangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://jyb.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://saz.hnxiangtu.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tzm.chenzaomai.com

JS:   "7".padStart(3, "0")
来源：http://bcj.sweek.top

TS:   "7".padStart(3, "0")
来源：http://zby.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://rly.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zjh.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hhj.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tnw.cdnleiting.top

[E11] 反转字符串
来源：http://akk.iojbl.cn

Py:   s[::-1]
来源：http://ysu.c1oappe.top

PHP:  strrev($s);
来源：http://pou.cdnleiting.top

JS:   [...s].reverse().join("")
来源：http://ugp.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://vjc.9152youxi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tyv.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cne.pengpengdd.cyou

Ruby: s.reverse
来源：http://mjm.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://rbg.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://gui.fanxiaobao.xyz

Py:   s.count("a")
来源：http://pvv.316326.xyz

PHP:  substr_count($s, "a");
来源：http://hwh.xylfe.cn

JS:   s.split("a").length - 1
来源：http://jrt.daxiang520.top

TS:   s.split("a").length - 1
来源：http://zgx.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rjq.yonumen.top

Go:   strings.Count(s, "a")
来源：http://eac.smart0.xyz

Ruby: s.count("a")
来源：http://jxr.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://hcu.quarkkingdee.top

[E13] 逐字符遍历
来源：http://sql.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://caj.bbcook.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iim.jinqigufen.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yvg.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://whw.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aft.hcnkem.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wew.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://nmb.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kdm.ehwqpu.com

[E14] URL 编码与 Base64
来源：http://xwm.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kmw.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cvx.ehwqpu.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://etq.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fdv.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kkx.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ywb.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vre.yuanzhike.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dcg.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://icv.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gqp.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wug.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xgg.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aod.ehwqpu.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ywz.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uxh.yuxming.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mmw.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zda.zhaomingkeji.xyz

[E16] 数字千分位
来源：http://sga.gzhubu.top

Py:   f"{1234567:,}"
来源：http://fip.mhx1999.top

PHP:  number_format(1234567);
来源：http://jqe.guowangkeji.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ukb.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xif.ydzc1.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bos.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://snl.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sul.ehwqpu.com

C#:   1234567.ToString("N0")
来源：http://usd.zdbjq.cn

[E17] 首字母大写
来源：http://giz.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pfr.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bss.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://voq.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kjf.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nzj.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ufu.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://pcy.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://evq.fengsongda.top

[E18] 模板占位符替换
来源：http://ukw.xuetiantiany.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://brj.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://euw.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qpf.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://qas.yj202588.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pag.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://slv.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://toj.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xsa.ydzc1.top

[E19] 多行文本按行拆分
来源：http://efc.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://szo.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://trm.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://cmt.vqdsnc.cn

TS:   s.split(/\r?\n/)
来源：http://eim.jinqigufen.top

Java: s.lines().toList()
来源：http://bff.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://tbe.fehbvm.com

Ruby: s.lines
来源：http://hnu.chenzaomai.com

C#:   s.Split('\n')
来源：http://jqu.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://clg.chenjidiqi.icu

Py:   if not s:
来源：http://vft.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qdb.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mqv.nanxuanxn.top

TS:   if (s === "") {}
来源：http://vwy.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://knh.xuetiantiany.cn

Go:   if s == "" {}
来源：http://gli.guannengcc.top

Ruby: if s.empty?
来源：http://qof.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bgp.tian-w.cn

[E21] 超长截断加省略号
来源：http://pzx.snrcjt.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ugl.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eas.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qco.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tnt.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bgz.xylfe.cn

Go:   // 按 rune 判断长度后截断
来源：http://goj.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://caj.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://caq.jinyuanbaomall.cn

[E22] 字节长度与字符长度
来源：http://zcb.haohaochexian.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wij.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kjn.sxryk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qsg.yanxiufei.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://czd.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hfp.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mju.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://ymq.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tkk.jqgufenzy.top

================================================================================
来源：http://nfi.hywenlv.cn

F. 文件与目录
来源：http://cpj.mhx1999.top

================================================================================
来源：http://dvm.feifeiyinyue.top

[F01] 读取整个文件
来源：http://cdu.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ewg.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://qta.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nlc.ehwqpu.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yir.yuanzhike.top

Java: Files.readString(Path.of("a.txt"))
来源：http://khg.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cnv.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://qrm.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://xrr.xylfe.cn

[F02] 逐行读取文件
来源：http://qqf.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hig.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zrk.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://str.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://euv.birdmap.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gpj.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lku.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iwa.quarkkingdee.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uxp.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://vcg.ydzc1.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://otf.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yul.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zij.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brm.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rtt.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hfp.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://kel.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ult.snrcjt.cn

[F04] 追加写入文件
来源：http://hjm.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qxp.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jgs.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xsb.fktsv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qnx.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ieu.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vfn.hnxiangtu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fhz.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xto.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://yed.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dob.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://sgz.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://bvp.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://wqu.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yns.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://foi.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://sdp.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://lnz.sjlbkw.cn

[F06] 删除文件
来源：http://vmj.gzhubu.top

Py:   os.remove("a.txt")
来源：http://jxl.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://eaw.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ddl.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://axu.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ied.yj202588.top

Go:   os.Remove("a.txt")
来源：http://bjp.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://xpz.nanxinkj.top

C#:   File.Delete("a.txt");
来源：http://qni.yueranfly.top

[F07] 创建目录（含多级）
来源：http://lqs.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://clp.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sre.shuidangran.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nsl.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pom.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://utt.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xcg.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ili.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fhr.jinqigufen.top

[F08] 遍历目录
来源：http://hua.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://spb.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cna.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://nvf.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://yac.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fky.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ibk.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://iaj.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://yto.xuanzx.com

[F09] 获取文件大小
来源：http://xya.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://pjg.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://kzv.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://xsu.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://wre.jinqigfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://qag.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jve.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://kwo.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://lte.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://jgq.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wcs.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rbs.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zsq.epnwcf.com

TS:   path.extname("a.txt")
来源：http://vvb.gotoacloud.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ajs.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baq.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qgw.xingfuxueyuan.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zzi.ppjwa.cn

[F11] 复制与移动文件
来源：http://hyh.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fvo.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqr.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sff.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyf.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xqo.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ixk.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eon.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kyl.hesvh.cn

[F12] CSV 读写
来源：http://uhi.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vny.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kkl.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ssb.shanyushiyangkeji.top

TS:   // 同上
来源：http://bad.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fkw.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rfz.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vmg.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://btd.zhiwuduotai.top

================================================================================
来源：http://lts.kuanghao11.cn

G. 面向对象
来源：http://nnj.zycfv.cn

================================================================================
来源：http://cts.jianghu66.top

[G01] 定义类
来源：http://sxa.aibaodan.cn

Py:   class User: pass
来源：http://bgt.ivvv.top

PHP:  class User {}
来源：http://bnn.smart0.xyz

JS:   class User {}
来源：http://uoq.meibo888.top

TS:   class User { name: string = ""; }
来源：http://ugt.sweek.top

Java: class User {}
来源：http://wwt.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://mxg.feifeiyinyue.top

Ruby: class User; end
来源：http://vnl.cashguo.top

C#:   class User {}
来源：http://jxb.yueranfly.top

[G02] 构造函数
来源：http://gij.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://fir.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://enj.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://tin.birdmap.top

TS:   constructor(public name: string) {}
来源：http://kth.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://mlg.dianchejie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rzu.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://fgg.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://axz.xinyue.icu

[G03] 实例属性
来源：http://rbv.yueranfly.top

Py:   self.name = "x"
来源：http://tfa.yj20258.top

PHP:  public string $name = "x";
来源：http://hqb.yueranfly.top


<!-- 参考信息 -->