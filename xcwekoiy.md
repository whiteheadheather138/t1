代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zkc.zhiwuduotai.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bzq.tianlin.xyz

JS:   s.replace(/\s+/g, "")
来源：http://zdw.316326.xyz

TS:   s.replace(/\s+/g, "")
来源：http://lic.sysykeji.top

Java: s.replaceAll("\\s+", "")
来源：http://ywu.tanke756.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://iqe.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://jkt.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://src.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://owh.jianghu66.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ppt.jqgufenzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ktb.yanxiufei.cn

JS:   "7".padStart(3, "0")
来源：http://kob.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://ekt.cashguo.top

Java: String.format("%03d", 7)
来源：http://qgk.yueranfly.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://vtr.vehdjk.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ifd.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kbv.hnxiangtu.top

[E11] 反转字符串
来源：http://yzy.sysykeji.top

Py:   s[::-1]
来源：http://ryt.andypj.xyz

PHP:  strrev($s);
来源：http://tay.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://has.bbcook.cn

TS:   [...s].reverse().join("")
来源：http://yvf.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ldi.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ace.fzhhl.top

Ruby: s.reverse
来源：http://mfq.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://hme.jinqigfzy.top

[E12] 统计某字符出现次数
来源：http://nko.yueranfly.top

Py:   s.count("a")
来源：http://onu.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://dzx.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://pvs.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://rzh.yj202588.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sjx.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://pdj.fehbvm.com

Ruby: s.count("a")
来源：http://sqf.fehbvm.com

C#:   s.Count(c => c == 'a')
来源：http://arh.tanke756.top

[E13] 逐字符遍历
来源：http://buf.fengsongda.top

Py:   for ch in s: print(ch)
来源：http://nbc.yueranfly.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eyk.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yuz.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fnq.daria6918.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ily.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qmt.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eyg.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rwq.nwbrower.top

[E14] URL 编码与 Base64
来源：http://zhc.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yvp.52xcode.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://awn.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://srs.redwolf501.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bio.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kow.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tac.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lqm.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://shr.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://zfk.gzhubu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tfk.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pml.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://heh.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jxi.jianghu66.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qyu.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ccn.tanke756.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qin.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eap.ppjwa.cn

[E16] 数字千分位
来源：http://qzj.hesvh.cn

Py:   f"{1234567:,}"
来源：http://dkp.sjlbkw.cn

PHP:  number_format(1234567);
来源：http://ope.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pdt.hesvh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dre.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qcs.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vex.xingfuxueyuan.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lbm.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://tsf.snrcjt.cn

[E17] 首字母大写
来源：http://zig.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yec.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qgh.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhp.gogol.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wej.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lcp.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ilu.shangyingyoupin.top

Ruby: s.capitalize
来源：http://est.jinyuanbaomall.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xpz.hnqzz.top

[E18] 模板占位符替换
来源：http://weu.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tjq.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vuu.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mso.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wes.hammf.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ewg.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://aza.nwbrower.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xlk.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yjn.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://kpa.bbcook.cn

Py:   s.splitlines()
来源：http://uic.9152youxi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mni.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://cmj.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://vyi.yangfankeji.com

Java: s.lines().toList()
来源：http://gxj.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://qar.shuidangran.top

Ruby: s.lines
来源：http://yaw.svipenyu.cn

C#:   s.Split('\n')
来源：http://uel.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://tyq.316326.xyz

Py:   if not s:
来源：http://ksk.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zlj.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://veo.yvedp.cn

TS:   if (s === "") {}
来源：http://tsu.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://wyj.cheryme.top

Go:   if s == "" {}
来源：http://gqb.dianchejie.cn

Ruby: if s.empty?
来源：http://icl.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jin.gotoacloud.top

[E21] 超长截断加省略号
来源：http://cxn.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://obq.smart0.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypd.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ngx.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jrc.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gyp.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://rbo.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uxj.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uqj.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://vqd.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nes.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwt.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gov.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwm.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cwu.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lkh.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://cfy.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ltw.vehdjk.com

================================================================================
来源：http://sgx.tianlin.xyz

F. 文件与目录
来源：http://ocn.fanxiaobao.xyz

================================================================================
来源：http://gxx.quarkkingdee.top

[F01] 读取整个文件
来源：http://igf.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mll.hongshengwenyu.top

PHP:  file_get_contents("a.txt");
来源：http://ayj.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ksh.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cla.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gow.gotoacloud.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cdl.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://ixv.jinyuanbaomall.cn

C#:   File.ReadAllText("a.txt");
来源：http://gir.316326.xyz

[F02] 逐行读取文件
来源：http://pfx.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rxh.svipenyu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vrs.fktsv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibl.tanke756.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gkm.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://syb.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ghn.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hfd.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oyp.vqdsnc.cn

[F03] 写入文件（覆盖）
来源：http://xiv.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jdq.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dsi.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dex.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ywq.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imu.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lkq.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://nze.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ooq.cqqwz.cn

[F04] 追加写入文件
来源：http://fvx.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://quo.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nny.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bir.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpp.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ydi.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jcx.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qhj.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://shl.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://eph.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://udw.hcnkem.com

PHP:  file_exists("a.txt");
来源：http://ugw.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://ezt.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://ecn.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hrz.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qvv.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://opo.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://dyf.shangyingyoupin.top

[F06] 删除文件
来源：http://fen.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://ean.daria6918.cn

PHP:  unlink("a.txt");
来源：http://iki.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://buf.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://sla.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rli.hongshengwenyu.top

Go:   os.Remove("a.txt")
来源：http://wyg.uphjek.com

Ruby: File.delete("a.txt")
来源：http://ydk.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://pza.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://kvy.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ayo.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qfn.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tdx.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psr.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uod.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rut.wangshuangyany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xxx.jinqigufen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yaq.shanyushiyangkeji.top

[F08] 遍历目录
来源：http://qrf.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aac.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://box.ctjpmb.com

JS:   fs.readdirSync("dir")
来源：http://htt.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://noy.chenlongwang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vbk.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mxv.yueranfly.top

Ruby: Dir.children("dir")
来源：http://xvq.xylfe.cn

C#:   Directory.GetFiles("dir")
来源：http://zvv.vehdjk.com

[F09] 获取文件大小
来源：http://sva.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://gps.tanke756.top

PHP:  filesize("a.txt");
来源：http://msx.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://oud.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://asl.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://vxh.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jla.shuidangran.top

Ruby: File.size("a.txt")
来源：http://bqr.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://elu.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://kff.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wnb.yueranfly.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hus.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://clp.cheryme.top

TS:   path.extname("a.txt")
来源：http://xsn.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mta.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qcn.xylfe.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyo.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kad.zdqjudy.top

[F11] 复制与移动文件
来源：http://llx.ehwqpu.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wwt.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tvs.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kjn.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wdb.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ima.daria6918.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rlx.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cvm.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uvg.tian-w.cn

[F12] CSV 读写
来源：http://fel.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ojb.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mfq.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jby.yuxming.cn

TS:   // 同上
来源：http://wif.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://auk.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ebf.ctjpmb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ksl.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://njv.yuanzhike.top

================================================================================
来源：http://lhb.gotoacloud.top

G. 面向对象
来源：http://gmh.hongshengwenyu.top

================================================================================
来源：http://fed.feifeiyinyue.top

[G01] 定义类
来源：http://ptz.shanyushiyangtech.top

Py:   class User: pass
来源：http://xub.cucudq.cn

PHP:  class User {}
来源：http://rxx.tanke756.top

JS:   class User {}
来源：http://pbu.bbcook.cn

TS:   class User { name: string = ""; }
来源：http://rpv.tarul.cn

Java: class User {}
来源：http://vrm.hammf.cn

Go:   type User struct { Name string }
来源：http://sva.birdmap.top

Ruby: class User; end
来源：http://gob.sweek.top

C#:   class User {}
来源：http://wnf.zycfv.cn

[G02] 构造函数
来源：http://qvl.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://jjs.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://ifm.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://yyc.xylfe.cn

TS:   constructor(public name: string) {}
来源：http://xli.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://otm.hnxiangtu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gcs.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://kyt.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://sdf.zycfv.cn

[G03] 实例属性
来源：http://tqi.cucudq.cn

Py:   self.name = "x"
来源：http://wfw.havefunace.top

PHP:  public string $name = "x";
来源：http://dtr.sufxvd.cn

JS:   this.name = "x";
来源：http://dce.aibaodan.cn

TS:   name: string = "x";
来源：http://ghd.xziqi.cn

Java: private String name;
来源：http://vro.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zqt.hfpthk.cn

Ruby: @name = "x"
来源：http://grn.yanxiufei.cn

C#:   public string Name { get; set; } = "x";
来源：http://wyk.ctjpmb.com

[G04] 定义方法
来源：http://dze.sweek.top

Py:   def greet(self): return self.name
来源：http://ief.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vzc.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://iqb.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://psh.zhoulong.xyz

Java: String greet() { return name; }
来源：http://tin.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nsi.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://xyb.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://dky.zhaomingkeji.xyz

[G05] 继承
来源：http://xte.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://iwt.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://tqo.epnwcf.com

JS:   class Admin extends User {}
来源：http://xot.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://hlm.ybcxt.top

Java: class Admin extends User {}
来源：http://qmt.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dzj.nwbrower.top

Ruby: class Admin < User; end
来源：http://cin.jqgufenzy.top

C#:   class Admin : User {}
来源：http://szv.ivvv.top

[G06] 重写方法
来源：http://nfj.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://bvu.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://xuz.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://jbv.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://psq.iojbl.cn

Java: @Override String greet() { return "admin"; }
来源：http://tnl.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://crq.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://zjj.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://xpo.chenzaomai.com

[G07] 调用父类方法
来源：http://euy.jiagoushi.top

Py:   super().greet()
来源：http://ata.zhiwuduotai.top

PHP:  parent::greet();
来源：http://fnj.zdqjudy.top

JS:   super.greet();
来源：http://wlq.hcnkem.com

TS:   super.greet();
来源：http://byj.ybcxt.top

Java: super.greet();
来源：http://pzp.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rfq.0kj1m.cn


<!-- 参考信息 -->