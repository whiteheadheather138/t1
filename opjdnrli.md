代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://ijw.dianchejie.cn

TS:   s.split(",")
来源：http://trp.guannengcc.top

Java: s.split(",");  s.split("\\s+")
来源：http://pbu.xziqi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jyo.52xcode.cn

Ruby: s.split(",");  s.split
来源：http://udf.fehbvm.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://znq.shanyushiyangkeji.top

[E08] 数组按分隔符合并
来源：http://cia.tarul.cn

Py:   ",".join(items)
来源：http://qqv.birdmap.top

PHP:  implode(",", $items);
来源：http://jat.bjfxy.top

JS:   items.join(",")
来源：http://btq.jinqigufen.top

TS:   items.join(",")
来源：http://xpn.kuanghao11.cn

Java: String.join(",", items)
来源：http://oca.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://fzy.hcnkem.com

Ruby: items.join(",")
来源：http://kqh.hcnkem.com

C#:   string.Join(",", items)
来源：http://eql.hcnkem.com

[E09] 去除所有空白字符
来源：http://pbv.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://rwa.epnwcf.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ump.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://pfn.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://qff.yj202588.top

Java: s.replaceAll("\\s+", "")
来源：http://zjt.hnxiangtu.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://cox.zhiwuduotai.top

Ruby: s.gsub(/\s+/, "")
来源：http://acg.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bgc.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://azu.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qlq.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://slg.yueranfly.top

JS:   "7".padStart(3, "0")
来源：http://tql.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://tox.shuidangran.top

Java: String.format("%03d", 7)
来源：http://qmn.daria6918.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wjp.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ntx.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zqe.svipenyu.cn

[E11] 反转字符串
来源：http://izv.feifeiyinyue.top

Py:   s[::-1]
来源：http://oix.sxryk.cn

PHP:  strrev($s);
来源：http://abn.yvedp.cn

JS:   [...s].reverse().join("")
来源：http://qje.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://bqg.zdqjudy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gko.hysaishi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://amp.sweek.top

Ruby: s.reverse
来源：http://rok.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://bxe.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://jpl.fehbvm.com

Py:   s.count("a")
来源：http://spd.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://aed.zycfv.cn

JS:   s.split("a").length - 1
来源：http://cqr.kuanghao11.cn

TS:   s.split("a").length - 1
来源：http://mhi.snrcjt.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rvz.tarul.cn

Go:   strings.Count(s, "a")
来源：http://gvv.fehbvm.com

Ruby: s.count("a")
来源：http://rpb.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://gxs.shzxlz.cn

[E13] 逐字符遍历
来源：http://huf.hammf.cn

Py:   for ch in s: print(ch)
来源：http://asy.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ecw.sufxvd.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tdn.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vdd.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://koo.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ymy.ctjpmb.com

Ruby: s.each_char { |ch| puts ch }
来源：http://hju.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pmp.bbcook.cn

[E14] URL 编码与 Base64
来源：http://wiw.birdmap.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cnd.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://dsf.shanyushiyangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bka.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zue.tianlin.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oxf.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vpk.jinqigufen.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rnc.chenjidiqi.icu

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://srn.svipenyu.cn

[E15] HTML 转义 / 反转义
来源：http://icv.xylfe.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zfw.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mcu.daxiang520.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ukz.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rbe.yj202588.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fwg.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jpe.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://muv.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wsi.cashguo.top

[E16] 数字千分位
来源：http://qaz.xziqi.cn

Py:   f"{1234567:,}"
来源：http://mgn.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://bgb.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ndd.9152youxi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bnc.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pyw.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://akd.shanyushiyangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dje.jinqigufen.top

C#:   1234567.ToString("N0")
来源：http://gvg.jinqigufen.top

[E17] 首字母大写
来源：http://qkb.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bwi.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ord.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hbz.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nxy.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://anv.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iml.bjfxy.top

Ruby: s.capitalize
来源：http://cks.pengpengdd.cyou

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vyx.zycfv.cn

[E18] 模板占位符替换
来源：http://uda.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mfc.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dlj.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xzs.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vov.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://axe.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ido.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nsm.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wrw.c1oappe.top

[E19] 多行文本按行拆分
来源：http://dtf.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://aey.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rbq.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://bau.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://gaa.aizwys.cn

Java: s.lines().toList()
来源：http://akk.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://ewt.9152youxi.cn

Ruby: s.lines
来源：http://tga.jinyuanbaomall.cn

C#:   s.Split('\n')
来源：http://tpd.xuanzx.com

[E20] 判断字符串是否为空
来源：http://rux.yanxiufei.cn

Py:   if not s:
来源：http://ijn.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yve.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fia.jlsjyb.cn

TS:   if (s === "") {}
来源：http://wih.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://rgy.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://lxu.yangfankeji.com

Ruby: if s.empty?
来源：http://xww.sweek.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bhc.fzhhl.top

[E21] 超长截断加省略号
来源：http://yej.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cqk.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fha.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cgc.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ssn.xingfuxueyuan.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hvb.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://fag.daxiang520.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qcx.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zpc.yonumen.top

[E22] 字节长度与字符长度
来源：http://btw.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oao.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bbf.uphjek.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xye.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ypk.zdbjq.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dyq.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mec.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://gee.svipenyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://srr.yfazqb.com

================================================================================
来源：http://luo.ybcxt.top

F. 文件与目录
来源：http://ubh.xuetiantiany.cn

================================================================================
来源：http://ecu.bbcook.cn

[F01] 读取整个文件
来源：http://lwm.xylfe.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mkt.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://oua.yongpay.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egm.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://byn.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hpb.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dgm.hysaishi.cn

Ruby: File.read("a.txt")
来源：http://agq.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://mwn.daxiang520.top

[F02] 逐行读取文件
来源：http://eiv.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dcd.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rlr.zhiwuduotai.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://htl.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://suf.kuanghao11.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kar.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nrc.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cqv.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nnb.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://mbq.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gck.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cpb.gotoacloud.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epl.tarul.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jvl.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xbo.gogol.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vqt.guannengcc.top

Ruby: File.write("a.txt", "hi")
来源：http://dft.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://txj.iojbl.cn

[F04] 追加写入文件
来源：http://xnu.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zkd.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kxs.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxk.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gek.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cor.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iib.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sco.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rvf.jinghuilouyu.cn

[F05] 判断文件或目录是否存在
来源：http://zbg.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kml.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://zpz.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://poh.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://fsg.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iyl.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fbl.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://ckw.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://xde.guannengcc.top

[F06] 删除文件
来源：http://bxa.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://yio.yonumen.top

PHP:  unlink("a.txt");
来源：http://lkj.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://gpk.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ozw.jinqigfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zeo.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://syo.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://cgw.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://gza.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://hwv.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dzd.zhiwuduotai.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ieu.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qwl.zdqjudy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zlt.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hlo.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nbe.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zkc.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hla.mhx1999.top

[F08] 遍历目录
来源：http://tnt.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://xva.zhoulong.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wao.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://epx.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://eov.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kxd.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://sss.52xcode.cn

Ruby: Dir.children("dir")
来源：http://puq.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://ntd.iojbl.cn

[F09] 获取文件大小
来源：http://slr.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://sxd.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://mmm.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://xmo.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://rfx.wangdashe.top

Java: Files.size(Path.of("a.txt"))
来源：http://dde.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zwm.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://cgj.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://doz.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://qxl.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfa.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://plv.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rlz.zhixingplan.top

TS:   path.extname("a.txt")
来源：http://lnc.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jpf.cqqwz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://abq.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aef.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hmn.sysykeji.top

[F11] 复制与移动文件
来源：http://jmr.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lrz.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ozi.dashuyun.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://drt.dianchejie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gfo.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qri.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oiz.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fxv.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dev.jiagoushi.top

[F12] CSV 读写
来源：http://cpy.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ije.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jqh.yuxming.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oau.ppjwa.cn

TS:   // 同上
来源：http://exn.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://asv.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ria.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ezc.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://ppd.jinghuilouyu.cn

================================================================================
来源：http://ese.sufxvd.cn

G. 面向对象
来源：http://nhq.kuanghao11.cn

================================================================================
来源：http://axo.tarul.cn

[G01] 定义类
来源：http://tdz.hysaishi.cn

Py:   class User: pass
来源：http://odh.kuanghao11.cn

PHP:  class User {}
来源：http://kwm.snrcjt.cn

JS:   class User {}
来源：http://zyp.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://xat.shangyingyoupin.top

Java: class User {}
来源：http://mzf.9152youxi.cn

Go:   type User struct { Name string }
来源：http://sxd.hnxiangtu.top

Ruby: class User; end
来源：http://ngx.tarul.cn

C#:   class User {}
来源：http://ovk.svipenyu.cn

[G02] 构造函数
来源：http://jqi.chenjidiqi.icu

Py:   def __init__(self, name): self.name = name
来源：http://vpz.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://ygj.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://jib.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://kqu.yonumen.top

Java: User(String name) { this.name = name; }
来源：http://ire.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tkd.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://xkh.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://kpf.cdnleiting.top

[G03] 实例属性
来源：http://pkr.xziqi.cn

Py:   self.name = "x"
来源：http://emw.ybcxt.top

PHP:  public string $name = "x";
来源：http://pjg.zhoulong.xyz

JS:   this.name = "x";
来源：http://lqu.ydjk.org.cn

TS:   name: string = "x";
来源：http://exv.zhengqikj.top

Java: private String name;
来源：http://fvy.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mgp.ybcxt.top

Ruby: @name = "x"
来源：http://pmm.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://xpx.yanxiufei.cn

[G04] 定义方法
来源：http://rlw.pycfn.com

Py:   def greet(self): return self.name
来源：http://twz.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://err.sxryk.cn

JS:   greet() { return this.name; }
来源：http://tjx.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://qgk.ctjpmb.com

Java: String greet() { return name; }
来源：http://wem.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://adv.yj202588.top

Ruby: def greet; @name; end
来源：http://vvw.birdmap.top

C#:   public string Greet() => Name;
来源：http://kzr.mhx1999.top

[G05] 继承
来源：http://yps.hcnkem.com

Py:   class Admin(User): pass
来源：http://uuv.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://fbl.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://pqk.haohaochexian.top

TS:   class Admin extends User {}
来源：http://woy.guannengcc.top

Java: class Admin extends User {}
来源：http://fon.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ryx.bjfxy.top

Ruby: class Admin < User; end
来源：http://hvq.cheryme.top

C#:   class Admin : User {}
来源：http://kqy.shzxlz.cn


<!-- 参考信息 -->