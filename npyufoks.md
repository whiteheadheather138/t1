代发 wailian999

Go:   strings.Join(items, ",")
来源：http://zcf.zycfv.cn

Ruby: items.join(",")
来源：http://ysn.xziqi.cn

C#:   string.Join(",", items)
来源：http://lof.yj20258888.top

[E09] 去除所有空白字符
来源：http://dof.cdnleiting.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xnv.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hez.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://ohf.kuanghao11.cn

TS:   s.replace(/\s+/g, "")
来源：http://dnq.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://lsw.chenlongwang.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://usd.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://qpw.zdbjq.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ipd.sjlbkw.cn

[E10] 左侧补零 / 定长填充
来源：http://jop.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mga.sufxvd.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mdo.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://cng.cqqwz.cn

TS:   "7".padStart(3, "0")
来源：http://qed.316326.xyz

Java: String.format("%03d", 7)
来源：http://uqh.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ctw.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ggi.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rmz.zycfv.cn

[E11] 反转字符串
来源：http://mbk.bjfxy.top

Py:   s[::-1]
来源：http://pmi.jyoumei.cn

PHP:  strrev($s);
来源：http://efc.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://lds.gogol.net.cn

TS:   [...s].reverse().join("")
来源：http://dxi.zdbjq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qqm.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wdx.hcnkem.com

Ruby: s.reverse
来源：http://gxt.jinyuanbaomall.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wky.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://vkf.bjfxy.top

Py:   s.count("a")
来源：http://hjl.yj20258888.top

PHP:  substr_count($s, "a");
来源：http://sjp.chenjidiqi.icu

JS:   s.split("a").length - 1
来源：http://qhd.sufxvd.cn

TS:   s.split("a").length - 1
来源：http://kup.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofo.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://mvk.zhijiandao.cn

Ruby: s.count("a")
来源：http://ugv.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://upc.zhaomingkeji.xyz

[E13] 逐字符遍历
来源：http://kje.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://unu.zdbjq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rez.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cex.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ddo.tian-w.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zru.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fep.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zwx.shanyushiyangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yzw.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://cwv.xinyue.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bnp.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sja.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hmy.uphjek.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dxf.yuxming.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zxn.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://giz.hnxiangtu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://plk.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jrm.yfazqb.com

[E15] HTML 转义 / 反转义
来源：http://vvy.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iio.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sjf.bbcook.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qlx.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://akr.tarul.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ykt.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jkh.fktsv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ilv.jinghuilouyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nns.daria6918.cn

[E16] 数字千分位
来源：http://dci.gzhubu.top

Py:   f"{1234567:,}"
来源：http://mqt.aizwys.cn

PHP:  number_format(1234567);
来源：http://qqc.ybcxt.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xwu.zycfv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gkx.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ycc.vehdjk.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kdt.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gwl.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://rtj.wangshuangyany.cn

[E17] 首字母大写
来源：http://fvy.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nqo.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gae.dashuyun.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ird.birdmap.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqx.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vzj.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://drr.sjlbkw.cn

Ruby: s.capitalize
来源：http://huh.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rgh.316326.xyz

[E18] 模板占位符替换
来源：http://yfg.chenjidiqi.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hrv.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tka.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dah.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://lyo.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ciw.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ozo.yuxming.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pbq.pengpengdd.cyou

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://clj.jianghu66.top

[E19] 多行文本按行拆分
来源：http://yyg.jianghu66.top

Py:   s.splitlines()
来源：http://xvy.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gyj.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://rqv.quarkkingdee.top

TS:   s.split(/\r?\n/)
来源：http://yok.yj20258.top

Java: s.lines().toList()
来源：http://iww.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://ltg.bbcook.cn

Ruby: s.lines
来源：http://aix.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://diu.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://ccu.jlsjyb.cn

Py:   if not s:
来源：http://ggp.zycfv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dwd.shanyushiyangtech.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://byy.daria6918.cn

TS:   if (s === "") {}
来源：http://yfj.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://adh.ybcxt.top

Go:   if s == "" {}
来源：http://srf.ydzc1.top

Ruby: if s.empty?
来源：http://cla.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdo.cucudq.cn

[E21] 超长截断加省略号
来源：http://biq.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ntm.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fqw.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggk.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cko.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ypq.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://lfh.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mpw.iojbl.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tpn.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://yrp.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wfq.dashuyun.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mcd.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gbb.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ljh.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vtx.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dxm.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://xps.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gqm.sxryk.cn

================================================================================
来源：http://yst.nanxuanxn.top

F. 文件与目录
来源：http://axz.sjlbkw.cn

================================================================================
来源：http://pus.jinghuilouyu.cn

[F01] 读取整个文件
来源：http://jsy.tianlin.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://laf.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://sbq.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wkh.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mkf.kuanghao11.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://buq.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eas.redwolf501.top

Ruby: File.read("a.txt")
来源：http://ppe.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ohj.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://pcz.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dbk.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ggw.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://khe.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uqf.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rla.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zpa.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://otl.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ptl.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://zfd.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://arq.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fyq.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uet.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aiq.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uix.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sif.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://rrw.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://amw.nanxinkj.top

[F04] 追加写入文件
来源：http://nhz.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ygf.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dyz.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oyy.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzu.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://osz.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jak.ctjpmb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ogz.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zvf.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://anh.fehbvm.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ofa.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://wda.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://bee.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://dnj.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jpo.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ecd.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://jvm.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://cob.ydjk.org.cn

[F06] 删除文件
来源：http://vxu.9152youxi.cn

Py:   os.remove("a.txt")
来源：http://uzu.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://hrg.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://etq.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://rwv.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hhj.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://oqy.ppjwa.cn

Ruby: File.delete("a.txt")
来源：http://hao.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://pdj.daxiang520.top

[F07] 创建目录（含多级）
来源：http://kpp.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://osq.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nyi.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqt.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivs.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wud.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hke.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ywm.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oei.vehdjk.com

[F08] 遍历目录
来源：http://wfg.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bdq.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xda.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://gue.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://egm.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dhp.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://lkq.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://prb.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://xsk.ydjk.org.cn

[F09] 获取文件大小
来源：http://jek.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://ehp.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://drd.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://awc.jqgfzy.top

TS:   fs.statSync("a.txt").size
来源：http://olw.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://geh.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ipw.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://nye.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://etc.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://glq.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://unq.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lnt.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jzh.0kj1m.cn

TS:   path.extname("a.txt")
来源：http://xie.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://get.xuanzx.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pzq.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ogb.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qpc.jiagoushi.top

[F11] 复制与移动文件
来源：http://ytp.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ijw.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://agr.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pts.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pav.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hvv.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nri.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eir.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ixf.bjfxy.top

[F12] CSV 读写
来源：http://pqf.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nme.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wny.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gsq.bjfxy.top

TS:   // 同上
来源：http://wfj.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ylk.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tsj.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nkb.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wsn.jqgfzy.top

================================================================================
来源：http://kue.9152youxi.cn

G. 面向对象
来源：http://ooi.quarkkingdee.top

================================================================================
来源：http://pck.vehdjk.com

[G01] 定义类
来源：http://wsa.hfpthk.cn

Py:   class User: pass
来源：http://pxw.iojbl.cn

PHP:  class User {}
来源：http://woa.yfazqb.com

JS:   class User {}
来源：http://saj.yj202588.top

TS:   class User { name: string = ""; }
来源：http://rlb.jlsjyb.cn

Java: class User {}
来源：http://xdb.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://bij.hfpthk.cn

Ruby: class User; end
来源：http://dny.316326.xyz

C#:   class User {}
来源：http://ngi.jlsjyb.cn

[G02] 构造函数
来源：http://ptg.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://cyt.xziqi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qui.sweek.top

JS:   constructor(name) { this.name = name; }
来源：http://luw.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://cge.fanxiaobao.xyz

Java: User(String name) { this.name = name; }
来源：http://rjo.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yyr.wangshuangyany.cn

Ruby: def initialize(name); @name = name; end
来源：http://bfj.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://oqx.jinqigufen.top

[G03] 实例属性
来源：http://fqq.havefunace.top

Py:   self.name = "x"
来源：http://zmb.daria6918.cn

PHP:  public string $name = "x";
来源：http://yqw.haohaochexian.top

JS:   this.name = "x";
来源：http://fcf.wangshuangyany.cn

TS:   name: string = "x";
来源：http://tnu.shanyushiyangtech.top

Java: private String name;
来源：http://akg.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iuo.andypj.xyz

Ruby: @name = "x"
来源：http://gun.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://iou.yangfankeji.com

[G04] 定义方法
来源：http://sns.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://lfc.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://epx.xziqi.cn

JS:   greet() { return this.name; }
来源：http://qjr.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://nlu.chenlongwang.top

Java: String greet() { return name; }
来源：http://pfw.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdr.jqgfzy.top

Ruby: def greet; @name; end
来源：http://dql.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://vyn.bbcook.cn

[G05] 继承
来源：http://mnl.tanke756.top

Py:   class Admin(User): pass
来源：http://tic.dashuyun.cn

PHP:  class Admin extends User {}
来源：http://ray.tian-w.cn

JS:   class Admin extends User {}
来源：http://qbf.dianchejie.cn

TS:   class Admin extends User {}
来源：http://poi.daxiang520.top

Java: class Admin extends User {}
来源：http://gxi.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lgi.gogol.net.cn

Ruby: class Admin < User; end
来源：http://szt.ivvv.top

C#:   class Admin : User {}
来源：http://cil.c1oappe.top

[G06] 重写方法
来源：http://chf.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://hqp.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kec.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://zsd.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://cxa.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://fnl.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cmv.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://fjq.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://kxy.gzhubu.top

[G07] 调用父类方法
来源：http://fbh.c1oappe.top

Py:   super().greet()
来源：http://eaf.hesvh.cn

PHP:  parent::greet();
来源：http://vkw.havefunace.top


<!-- 参考信息 -->