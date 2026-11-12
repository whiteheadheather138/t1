代发 wailian999

[E06] 替换子串
来源：http://rnm.dianchejie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rhp.yj202588.top

PHP:  str_replace("a", "b", $s);
来源：http://fiv.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pcw.52xcode.cn

TS:   s.replaceAll("a", "b")
来源：http://lmj.xuetiantiany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvw.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mvb.hammf.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ewr.jianghu66.top

C#:   s.Replace("a", "b")
来源：http://pjw.316326.xyz

[E07] 按分隔符拆分
来源：http://uhd.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://auv.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rcs.smart0.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://kkl.sysykeji.top

TS:   s.split(",")
来源：http://xuf.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cam.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://age.zhixingplan.top

Ruby: s.split(",");  s.split
来源：http://znv.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qpu.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://lry.snrcjt.cn

Py:   ",".join(items)
来源：http://umf.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://lvo.nwbrower.top

JS:   items.join(",")
来源：http://sbv.jinyuanbaomall.cn

TS:   items.join(",")
来源：http://ejk.fengsongda.top

Java: String.join(",", items)
来源：http://rgo.0kj1m.cn

Go:   strings.Join(items, ",")
来源：http://hrs.vqdsnc.cn

Ruby: items.join(",")
来源：http://ova.jiagoushi.top

C#:   string.Join(",", items)
来源：http://dkm.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://jij.yuxming.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jaj.hysaishi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pqt.bbcook.cn

JS:   s.replace(/\s+/g, "")
来源：http://hgc.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://jdv.snrcjt.cn

Java: s.replaceAll("\\s+", "")
来源：http://uru.yfazqb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://ede.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://cmk.cqqwz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cws.wangshuangyany.cn

[E10] 左侧补零 / 定长填充
来源：http://xcv.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xjy.yanxiufei.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://syf.jinghuilouyu.cn

JS:   "7".padStart(3, "0")
来源：http://zes.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://juu.bjfxy.top

Java: String.format("%03d", 7)
来源：http://bei.hongshengwenyu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ghf.ywan-chungtsiang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fep.ppjwa.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sbg.smart0.xyz

[E11] 反转字符串
来源：http://qmj.zhixingplan.top

Py:   s[::-1]
来源：http://wtm.nanxinkj.top

PHP:  strrev($s);
来源：http://bze.iojbl.cn

JS:   [...s].reverse().join("")
来源：http://bxg.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://dtk.zhaomingkeji.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://aje.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://umw.uphjek.com

Ruby: s.reverse
来源：http://obg.dashuyun.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hkq.aibaodan.cn

[E12] 统计某字符出现次数
来源：http://sna.tarul.cn

Py:   s.count("a")
来源：http://kbj.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://ghc.epnwcf.com

JS:   s.split("a").length - 1
来源：http://gfn.xziqi.cn

TS:   s.split("a").length - 1
来源：http://ycp.shangyingyoupin.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://igv.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://rbb.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://vxu.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://qzf.aizwys.cn

[E13] 逐字符遍历
来源：http://qnm.dashuyun.cn

Py:   for ch in s: print(ch)
来源：http://zhh.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ryq.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vve.316326.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wkm.guowangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wca.chenjidiqi.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jex.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rns.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://szf.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://ufc.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yuf.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bbq.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://clt.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gbt.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oeg.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zku.hywenlv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://toc.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zvz.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://vix.c1oappe.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ptx.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iun.xziqi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tfe.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://acx.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eci.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gzf.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uft.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jao.tianlin.xyz

[E16] 数字千分位
来源：http://jdh.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://cdu.epnwcf.com

PHP:  number_format(1234567);
来源：http://tdh.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://goy.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nhw.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://twb.fzhhl.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uwd.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://att.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://gtr.nanxuanxn.top

[E17] 首字母大写
来源：http://tdp.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bxd.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bri.xziqi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oba.pengpengdd.cyou

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pir.sjlbkw.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ynv.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kbu.jlsjyb.cn

Ruby: s.capitalize
来源：http://zkp.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fdu.sxryk.cn

[E18] 模板占位符替换
来源：http://ybn.jinyuanbaomall.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://koh.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fgx.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jkg.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wgu.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ouz.zdqjudy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://egf.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://htp.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://twa.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://zlb.iojbl.cn

Py:   s.splitlines()
来源：http://ehy.guowangkeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pfg.ivvv.top

JS:   s.split(/\r?\n/)
来源：http://two.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://nqo.c1oappe.top

Java: s.lines().toList()
来源：http://ohw.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://dcu.nanxuanxn.top

Ruby: s.lines
来源：http://fus.yfazqb.com

C#:   s.Split('\n')
来源：http://vad.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://hry.pycfn.com

Py:   if not s:
来源：http://bdn.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://syf.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tdp.mhx1999.top

TS:   if (s === "") {}
来源：http://nwg.hesvh.cn

Java: if (s.isEmpty()) {}
来源：http://ine.fktsv.cn

Go:   if s == "" {}
来源：http://qxo.gaohongyu789.top

Ruby: if s.empty?
来源：http://eeu.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hpe.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://dns.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oyu.yj202588.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gwl.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ozl.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://los.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wos.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://uwq.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oqr.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qyu.mhx1999.top

[E22] 字节长度与字符长度
来源：http://rte.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhu.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bqj.ivvv.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jmo.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nut.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jlv.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xys.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://vti.52xcode.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://owc.ppjwa.cn

================================================================================
来源：http://yds.snrcjt.cn

F. 文件与目录
来源：http://whz.pycfn.com

================================================================================
来源：http://xgc.fktsv.cn

[F01] 读取整个文件
来源：http://bck.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wmj.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://kdf.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hro.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xse.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bxl.shangyingyoupin.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lfi.kuanghao11.cn

Ruby: File.read("a.txt")
来源：http://jrc.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://fxe.pycfn.com

[F02] 逐行读取文件
来源：http://lah.yuxming.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rvn.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hjn.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hli.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gyp.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gfr.iojbl.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mgm.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://viu.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ywi.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://zsv.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fay.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qiv.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zoz.gotoacloud.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ajn.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pvh.ctjpmb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eqc.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://fxw.yj20258888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pdf.bbcook.cn

[F04] 追加写入文件
来源：http://vxe.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gfp.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yxt.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqm.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eho.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aex.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jgi.jqgufenzy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lhp.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hqd.zycfv.cn

[F05] 判断文件或目录是否存在
来源：http://ewu.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hyj.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://vje.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://hjs.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://qbd.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ecu.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xxq.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://eii.yonumen.top

C#:   File.Exists("a.txt")
来源：http://dvf.daria6918.cn

[F06] 删除文件
来源：http://srp.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://sqv.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://gif.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://ffy.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oji.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oon.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://eko.yj202588.top

Ruby: File.delete("a.txt")
来源：http://acb.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://pyg.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://wax.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kjn.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hie.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ksj.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eeu.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xov.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uum.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cuq.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lwg.andypj.xyz

[F08] 遍历目录
来源：http://cwi.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://afm.tarul.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://joe.chenjidiqi.icu

JS:   fs.readdirSync("dir")
来源：http://duw.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://hxg.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qyw.andypj.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://yho.tian-w.cn

Ruby: Dir.children("dir")
来源：http://wao.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://khr.meibo888.top

[F09] 获取文件大小
来源：http://bjw.yanxiufei.cn

Py:   os.path.getsize("a.txt")
来源：http://jyz.yvedp.cn

PHP:  filesize("a.txt");
来源：http://zis.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://gdg.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://xgt.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://rxq.zhixingplan.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uyy.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://cjr.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://ezv.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://lba.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mmx.guannengcc.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kjs.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://esg.yonumen.top

TS:   path.extname("a.txt")
来源：http://oka.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gsu.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zeg.c1oappe.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qeo.svipenyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jns.gaohongyu789.top

[F11] 复制与移动文件
来源：http://arp.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tkc.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pvb.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hbd.jinqigufen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gbp.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rsq.dashuyun.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tql.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mrt.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mmi.tanke756.top

[F12] CSV 读写
来源：http://djz.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wqt.zhijiandao.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tpm.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rsa.hywenlv.cn

TS:   // 同上
来源：http://ihl.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pfm.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://had.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://skd.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jtl.hnxiangtu.top

================================================================================
来源：http://ztn.jyoumei.cn

G. 面向对象
来源：http://efn.zhixingplan.top

================================================================================
来源：http://dnp.sysykeji.top

[G01] 定义类
来源：http://xlx.zdqjudy.top

Py:   class User: pass
来源：http://dof.svipenyu.cn

PHP:  class User {}
来源：http://ilm.yanxiufei.cn

JS:   class User {}
来源：http://qac.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://uii.tianlin.xyz

Java: class User {}
来源：http://kod.yueranfly.top

Go:   type User struct { Name string }
来源：http://xph.aizwys.cn

Ruby: class User; end
来源：http://ehw.yfazqb.com

C#:   class User {}
来源：http://oyo.jqgufenzy.top

[G02] 构造函数
来源：http://omu.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://qwr.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://psy.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://dbb.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://cut.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://vna.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nxk.ybcxt.top

Ruby: def initialize(name); @name = name; end
来源：http://jga.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://mma.nanxinkj.top

[G03] 实例属性
来源：http://ekh.ybcxt.top

Py:   self.name = "x"
来源：http://etk.jinqigufen.top

PHP:  public string $name = "x";
来源：http://nqf.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://jus.yuxming.cn

TS:   name: string = "x";
来源：http://oop.zhoulong.xyz

Java: private String name;
来源：http://cuu.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mza.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://nae.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://fpi.sweek.top

[G04] 定义方法
来源：http://uei.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://pdd.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://yra.fktsv.cn

JS:   greet() { return this.name; }
来源：http://qig.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://wgc.zhijiandao.cn

Java: String greet() { return name; }
来源：http://ozj.hnxiangtu.top


<!-- 参考信息 -->