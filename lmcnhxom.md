代发 wailian999

PHP:  strpos($s, "x");
来源：http://ldy.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://spx.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://xtd.gzhubu.top

Java: s.indexOf("x")
来源：http://pgu.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://mcg.hysaishi.cn

Ruby: s.index("x")
来源：http://fju.gaohongyu789.top

C#:   s.IndexOf("x")
来源：http://yqd.jianghu66.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yla.bjfxy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vap.wangshuangyany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lga.dashuyun.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fhc.jqgufenzy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://zhn.shanyushiyangkeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sqy.xuanzx.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://nby.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wat.svipenyu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gen.zycfv.cn

[E06] 替换子串
来源：http://hvx.zhongyouzk.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lwj.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://lnb.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xce.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://cws.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yis.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhn.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iks.jlsjyb.cn

C#:   s.Replace("a", "b")
来源：http://hzz.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://wxb.yuanzhike.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jzt.uphjek.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://pga.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ypw.haohaochexian.top

TS:   s.split(",")
来源：http://wol.yvedp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mlq.hnxiangtu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hyk.vehdjk.com

Ruby: s.split(",");  s.split
来源：http://nkw.zhijiandao.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://olt.jianghu66.top

[E08] 数组按分隔符合并
来源：http://gfi.hfpthk.cn

Py:   ",".join(items)
来源：http://wpx.cucudq.cn

PHP:  implode(",", $items);
来源：http://zce.zhiwuduotai.top

JS:   items.join(",")
来源：http://zpb.cqqwz.cn

TS:   items.join(",")
来源：http://vxc.haohaochexian.top

Java: String.join(",", items)
来源：http://rwx.cqqwz.cn

Go:   strings.Join(items, ",")
来源：http://otp.sysykeji.top

Ruby: items.join(",")
来源：http://qhd.zdbjq.cn

C#:   string.Join(",", items)
来源：http://bks.dashuyun.cn

[E09] 去除所有空白字符
来源：http://rkt.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rzn.ehwqpu.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ech.zdbjq.cn

JS:   s.replace(/\s+/g, "")
来源：http://qlq.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://isl.xziqi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ayk.hongshengwenyu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://hrz.andypj.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://qjy.nanxinkj.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tfx.zycfv.cn

[E10] 左侧补零 / 定长填充
来源：http://pun.vehdjk.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://opx.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dsw.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://kcc.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://yaf.bbcook.cn

Java: String.format("%03d", 7)
来源：http://ngj.fanxiaobao.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://hxx.chenzaomai.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ymu.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baf.sxryk.cn

[E11] 反转字符串
来源：http://jis.ywan-chungtsiang.top

Py:   s[::-1]
来源：http://tff.zdbjq.cn

PHP:  strrev($s);
来源：http://nqd.zhaomingkeji.xyz

JS:   [...s].reverse().join("")
来源：http://lkm.smart0.xyz

TS:   [...s].reverse().join("")
来源：http://hii.hesvh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wlt.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fdz.cheryme.top

Ruby: s.reverse
来源：http://iow.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ehw.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://kbu.aibaodan.cn

Py:   s.count("a")
来源：http://dgn.ydjk.org.cn

PHP:  substr_count($s, "a");
来源：http://yfm.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://mkg.aizwys.cn

TS:   s.split("a").length - 1
来源：http://gxg.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fro.zycfv.cn

Go:   strings.Count(s, "a")
来源：http://cpb.birdmap.top

Ruby: s.count("a")
来源：http://fsh.shuidangran.top

C#:   s.Count(c => c == 'a')
来源：http://pli.pycfn.com

[E13] 逐字符遍历
来源：http://vyy.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://pht.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://muc.daria6918.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qzd.jqgufenzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oyo.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blz.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kvk.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vkw.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hri.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://iat.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qcs.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://caj.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qor.hnqzz.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sgj.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bgv.daria6918.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://puw.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dam.sjlbkw.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bza.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://skq.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nex.xingfuxueyuan.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydm.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pma.zhoulong.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://vjs.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yuk.ivvv.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qym.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wvx.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uso.ydjk.org.cn

[E16] 数字千分位
来源：http://hbg.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://nys.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://knq.kuanghao11.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aal.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://prw.fktsv.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zgz.sweek.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uoo.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cci.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://fox.zhengqikj.top

[E17] 首字母大写
来源：http://rbl.pycfn.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://php.daria6918.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nnk.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gmz.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yjz.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hjh.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dnf.yueranfly.top

Ruby: s.capitalize
来源：http://cmq.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://njy.zhixingplan.top

[E18] 模板占位符替换
来源：http://kre.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jus.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lul.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bja.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xem.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bla.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lkc.zdqjudy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bhf.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ssb.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://rls.52xcode.cn

Py:   s.splitlines()
来源：http://che.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rma.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://lgd.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://sjz.shangyingyoupin.top

Java: s.lines().toList()
来源：http://vvs.zhoulong.xyz

Go:   strings.Split(s, "\n")
来源：http://qah.hfpthk.cn

Ruby: s.lines
来源：http://oyf.ybcxt.top

C#:   s.Split('\n')
来源：http://snl.sysykeji.top

[E20] 判断字符串是否为空
来源：http://ogk.zhiwuduotai.top

Py:   if not s:
来源：http://gza.c1oappe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kio.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xms.hesvh.cn

TS:   if (s === "") {}
来源：http://koq.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://vcr.zdbjq.cn

Go:   if s == "" {}
来源：http://kqj.ppjwa.cn

Ruby: if s.empty?
来源：http://txu.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eeq.zhixingplan.top

[E21] 超长截断加省略号
来源：http://ken.jyoumei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://phi.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fxq.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdt.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tdo.cqqwz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dam.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://cli.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wpp.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tqt.jinqigufen.top

[E22] 字节长度与字符长度
来源：http://csz.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://etv.wangshuangyany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ooy.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iye.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wfs.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://roq.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pdc.ctjpmb.com

Ruby: s.bytesize;  s.length
来源：http://qon.yuxming.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ywz.chenlongwang.top

================================================================================
来源：http://yxi.sufxvd.cn

F. 文件与目录
来源：http://khd.dashuyun.cn

================================================================================
来源：http://uqi.xingfuxueyuan.xyz

[F01] 读取整个文件
来源：http://aax.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aws.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://xio.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://agm.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ojm.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kmz.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qif.iojbl.cn

Ruby: File.read("a.txt")
来源：http://mdx.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://oub.tian-w.cn

[F02] 逐行读取文件
来源：http://pdh.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pxn.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yrl.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://haw.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wmf.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yew.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fhh.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wla.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kyo.316326.xyz

[F03] 写入文件（覆盖）
来源：http://ppw.cdnleiting.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jhw.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bkz.xziqi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ihi.gzhubu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qev.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://upd.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tct.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://pii.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oxt.daria6918.cn

[F04] 追加写入文件
来源：http://mun.shanyushiyangtech.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xrj.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nif.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjf.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aus.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://egn.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lzc.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://htj.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xjc.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://ztb.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zmb.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://usg.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://vqk.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://xgp.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://imd.dashuyun.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gej.hywenlv.cn

Ruby: File.exist?("a.txt")
来源：http://sfz.redwolf501.top

C#:   File.Exists("a.txt")
来源：http://rzt.ehwqpu.com

[F06] 删除文件
来源：http://exw.havefunace.top

Py:   os.remove("a.txt")
来源：http://gty.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://qsg.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://wwn.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qdp.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://amt.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://hzg.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://xzp.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://lgm.xylfe.cn

[F07] 创建目录（含多级）
来源：http://yld.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://arb.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dog.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tux.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdp.fzhhl.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vgw.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://txm.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dvx.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gjl.ydjk.org.cn

[F08] 遍历目录
来源：http://mnh.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://sqp.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gas.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://mgv.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://gcz.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ann.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://fcg.hammf.cn

Ruby: Dir.children("dir")
来源：http://hqn.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://umm.gzhubu.top

[F09] 获取文件大小
来源：http://pay.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://yzc.tarul.cn

PHP:  filesize("a.txt");
来源：http://lwz.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://btb.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://esf.zhaomingkeji.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dyn.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lkc.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://zat.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://pdl.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://qqo.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ffd.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dtu.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dji.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://gqm.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ncb.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nhd.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://her.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lwy.sjlbkw.cn

[F11] 复制与移动文件
来源：http://fuw.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qxj.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qqo.svipenyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rzj.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zch.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://phn.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://okl.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cnc.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kmv.yanxiufei.cn

[F12] CSV 读写
来源：http://dxv.zdbjq.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rlc.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kra.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xld.jyoumei.cn

TS:   // 同上
来源：http://zmy.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://suj.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://btw.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nve.shanyushiyangtech.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iiu.epnwcf.com

================================================================================
来源：http://irp.ybcxt.top

G. 面向对象
来源：http://axw.yangfankeji.com

================================================================================
来源：http://juy.guannengcc.top

[G01] 定义类
来源：http://zgx.aizwys.cn

Py:   class User: pass
来源：http://rrn.fktsv.cn

PHP:  class User {}
来源：http://npi.feifeiyinyue.top

JS:   class User {}
来源：http://xye.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://nto.yfazqb.com

Java: class User {}
来源：http://qbx.gogol.net.cn

Go:   type User struct { Name string }
来源：http://heo.zdbjq.cn

Ruby: class User; end
来源：http://fkt.ybcxt.top

C#:   class User {}
来源：http://lai.cashguo.top

[G02] 构造函数
来源：http://xzf.sweek.top

Py:   def __init__(self, name): self.name = name
来源：http://nhw.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://shn.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://tkh.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://bed.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://axz.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://arq.gzhubu.top

Ruby: def initialize(name); @name = name; end
来源：http://ile.yueranfly.top


<!-- 参考信息 -->