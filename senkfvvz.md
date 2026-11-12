代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fanxiaobao.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fop.fktsv.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ale.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rpk.tarul.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://niu.zhijiandao.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dvv.guannengcc.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mwd.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qnq.fanxiaobao.xyz

[E06] 替换子串
来源：http://mtn.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://toy.0kj1m.cn

PHP:  str_replace("a", "b", $s);
来源：http://xva.hnxiangtu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cmp.quarkkingdee.top

TS:   s.replaceAll("a", "b")
来源：http://sts.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zzd.fengsongda.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fbr.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://edj.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://sfe.yonumen.top

[E07] 按分隔符拆分
来源：http://uuv.cdnleiting.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pei.yuanzhike.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dfl.uphjek.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://kcy.epnwcf.com

TS:   s.split(",")
来源：http://xra.tarul.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yky.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://joh.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://adh.havefunace.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://usl.shzxlz.cn

[E08] 数组按分隔符合并
来源：http://qqx.hywenlv.cn

Py:   ",".join(items)
来源：http://kou.tianlin.xyz

PHP:  implode(",", $items);
来源：http://zob.hnqzz.top

JS:   items.join(",")
来源：http://dfw.smart0.xyz

TS:   items.join(",")
来源：http://lrr.snrcjt.cn

Java: String.join(",", items)
来源：http://asp.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://ohy.yueranfly.top

Ruby: items.join(",")
来源：http://kkw.zhengqikj.top

C#:   string.Join(",", items)
来源：http://lts.smart0.xyz

[E09] 去除所有空白字符
来源：http://wlv.zhoulong.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yci.sysykeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rgd.havefunace.top

JS:   s.replace(/\s+/g, "")
来源：http://ayc.chenzaomai.com

TS:   s.replace(/\s+/g, "")
来源：http://mqj.sweek.top

Java: s.replaceAll("\\s+", "")
来源：http://pqp.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cqm.zhongyouzk.top

Ruby: s.gsub(/\s+/, "")
来源：http://gfr.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qzd.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://zlx.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ubz.0kj1m.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gec.birdmap.top

JS:   "7".padStart(3, "0")
来源：http://ase.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://uhb.fzhhl.top

Java: String.format("%03d", 7)
来源：http://hhd.haohaochexian.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tdj.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wqz.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nmf.zdbjq.cn

[E11] 反转字符串
来源：http://qzc.fehbvm.com

Py:   s[::-1]
来源：http://yss.yfazqb.com

PHP:  strrev($s);
来源：http://rcp.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://dzq.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://cop.aizwys.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fmy.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yjm.smart0.xyz

Ruby: s.reverse
来源：http://xdg.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://roq.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://uxc.shangyingyoupin.top

Py:   s.count("a")
来源：http://tpk.redwolf501.top

PHP:  substr_count($s, "a");
来源：http://soi.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://vfe.fehbvm.com

TS:   s.split("a").length - 1
来源：http://jje.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rik.zhixingplan.top

Go:   strings.Count(s, "a")
来源：http://een.jqgfzy.top

Ruby: s.count("a")
来源：http://few.sxryk.cn

C#:   s.Count(c => c == 'a')
来源：http://lnx.smart0.xyz

[E13] 逐字符遍历
来源：http://anu.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://kxv.52xcode.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mmx.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lan.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ybc.tanke756.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://omf.ehwqpu.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://asu.bjfxy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://idp.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hzv.fehbvm.com

[E14] URL 编码与 Base64
来源：http://rdw.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://esm.meibo888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wac.zycfv.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dwp.ywan-chungtsiang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lrv.nanxuanxn.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://amy.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://imu.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ezp.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://glt.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://jco.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eto.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://adh.xinyue.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zyd.iojbl.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://aye.gotoacloud.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://idh.xingfuxueyuan.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tro.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://orx.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://seu.gogol.net.cn

[E16] 数字千分位
来源：http://ztx.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://pzs.jyoumei.cn

PHP:  number_format(1234567);
来源：http://ghc.tarul.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fau.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wck.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sdt.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jsv.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yfz.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://lpx.sjlbkw.cn

[E17] 首字母大写
来源：http://ssd.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hwf.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ljd.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ufw.smart0.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://drn.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dgi.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hdx.jyoumei.cn

Ruby: s.capitalize
来源：http://qza.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zvz.fzhhl.top

[E18] 模板占位符替换
来源：http://ehn.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dje.ywan-chungtsiang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dlk.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ipr.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yvi.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xdt.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thv.xziqi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qeb.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mqa.yfazqb.com

[E19] 多行文本按行拆分
来源：http://whi.52xcode.cn

Py:   s.splitlines()
来源：http://lln.0kj1m.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tyi.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://bsu.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://pxn.hesvh.cn

Java: s.lines().toList()
来源：http://zsf.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://miu.zhongyouzk.top

Ruby: s.lines
来源：http://bfk.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://uzh.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://ckw.jqgfzy.top

Py:   if not s:
来源：http://hei.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqe.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hme.gotoacloud.top

TS:   if (s === "") {}
来源：http://enn.sxryk.cn

Java: if (s.isEmpty()) {}
来源：http://mkf.ydjk.org.cn

Go:   if s == "" {}
来源：http://ram.jinqigfzy.top

Ruby: if s.empty?
来源：http://odg.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kdf.yueranfly.top

[E21] 超长截断加省略号
来源：http://bkz.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://spc.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hpd.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://csk.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://trt.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yzf.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://fse.zhiwuduotai.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ztk.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pyy.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://iwr.kuanghao11.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cbz.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ahv.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nnw.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jkc.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kkk.nanxuanxn.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ckr.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://exo.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aby.zhaomingkeji.xyz

================================================================================
来源：http://shg.c1oappe.top

F. 文件与目录
来源：http://fhj.jinqigufen.top

================================================================================
来源：http://ebd.xylfe.cn

[F01] 读取整个文件
来源：http://rxp.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mvh.dashuyun.cn

PHP:  file_get_contents("a.txt");
来源：http://dct.bbcook.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yra.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cye.shuidangran.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fik.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ghc.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://tqw.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://unr.zdqjudy.top

[F02] 逐行读取文件
来源：http://rdw.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zda.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kvq.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://utq.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hxs.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ean.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sbo.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bfq.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://prf.zdbjq.cn

[F03] 写入文件（覆盖）
来源：http://yhs.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tmk.zhongyouzk.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://srk.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hnj.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrv.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tvv.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycb.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://xeu.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uku.jlsjyb.cn

[F04] 追加写入文件
来源：http://uxs.cheryme.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://clh.birdmap.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vao.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yml.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://flv.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nlq.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vai.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqr.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://loc.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://gpp.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tds.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://gqx.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://jud.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://nlt.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://aqc.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hjm.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://iee.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://eud.quarkkingdee.top

[F06] 删除文件
来源：http://kex.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://pmr.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://rsb.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://nfd.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oan.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://llg.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://ozv.quarkkingdee.top

Ruby: File.delete("a.txt")
来源：http://jvk.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://fko.dianchejie.cn

[F07] 创建目录（含多级）
来源：http://jik.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pwu.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://det.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stm.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xhj.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kae.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://try.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jtl.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfq.aibaodan.cn

[F08] 遍历目录
来源：http://mye.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sei.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cli.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://bdp.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bxo.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ttz.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mtt.xylfe.cn

Ruby: Dir.children("dir")
来源：http://zat.sweek.top

C#:   Directory.GetFiles("dir")
来源：http://git.uphjek.com

[F09] 获取文件大小
来源：http://xki.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://pkw.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://iev.uphjek.com

JS:   fs.statSync("a.txt").size
来源：http://mhp.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://fkg.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://ngu.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ece.fehbvm.com

Ruby: File.size("a.txt")
来源：http://qwv.zhongyouzk.top

C#:   new FileInfo("a.txt").Length
来源：http://bpd.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://dbf.c1oappe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kto.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eac.yangfankeji.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aoa.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://jbj.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://diy.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nog.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://haz.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rct.dianchejie.cn

[F11] 复制与移动文件
来源：http://gri.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tnc.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzg.jinyuanbaomall.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eku.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qqd.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hfz.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lht.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zmk.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bsl.hongshengwenyu.top

[F12] CSV 读写
来源：http://cwp.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nci.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://goj.shuidangran.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xgg.ybcxt.top

TS:   // 同上
来源：http://ajx.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iyj.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tzp.yj20258.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bko.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sbr.hesvh.cn

================================================================================
来源：http://vfz.jyoumei.cn

G. 面向对象
来源：http://xtk.sufxvd.cn

================================================================================
来源：http://yjs.redwolf501.top

[G01] 定义类
来源：http://fix.bjfxy.top

Py:   class User: pass
来源：http://vrk.bbcook.cn

PHP:  class User {}
来源：http://smu.hnxiangtu.top

JS:   class User {}
来源：http://spx.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://wmk.sysykeji.top

Java: class User {}
来源：http://yjs.dashuyun.cn

Go:   type User struct { Name string }
来源：http://rzw.jianghu66.top

Ruby: class User; end
来源：http://uxg.hnqzz.top

C#:   class User {}
来源：http://cwl.bjfxy.top

[G02] 构造函数
来源：http://rrp.pengpengdd.cyou

Py:   def __init__(self, name): self.name = name
来源：http://mjg.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://eal.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://nvs.yj202588.top

TS:   constructor(public name: string) {}
来源：http://ngp.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://xzo.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://twx.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://rag.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://mth.svipenyu.cn

[G03] 实例属性
来源：http://cfd.zdqjudy.top

Py:   self.name = "x"
来源：http://kyf.yj20258888.top

PHP:  public string $name = "x";
来源：http://crg.feifeiyinyue.top

JS:   this.name = "x";
来源：http://usj.feifeiyinyue.top

TS:   name: string = "x";
来源：http://vvf.gogol.net.cn

Java: private String name;
来源：http://bck.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jwr.andypj.xyz


<!-- 参考信息 -->