代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://ruo.redwolf501.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rrn.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bli.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://hid.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://lll.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://fot.jlsjyb.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tpp.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ohh.xinyue.icu

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hgp.zdqjudy.top

[E11] 反转字符串
来源：http://eob.jianghu66.top

Py:   s[::-1]
来源：http://ogz.hongshengwenyu.top

PHP:  strrev($s);
来源：http://olc.pycfn.com

JS:   [...s].reverse().join("")
来源：http://ybw.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://yoj.hongshengwenyu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jdi.jinghuilouyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uwp.fengsongda.top

Ruby: s.reverse
来源：http://xgo.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://kjq.gogol.net.cn

[E12] 统计某字符出现次数
来源：http://khd.hcnkem.com

Py:   s.count("a")
来源：http://hcd.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://och.mhx1999.top

JS:   s.split("a").length - 1
来源：http://pvn.nwbrower.top

TS:   s.split("a").length - 1
来源：http://wma.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://urj.hammf.cn

Go:   strings.Count(s, "a")
来源：http://zmn.yongpay.top

Ruby: s.count("a")
来源：http://pfx.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://qsl.hywenlv.cn

[E13] 逐字符遍历
来源：http://gxf.aizwys.cn

Py:   for ch in s: print(ch)
来源：http://eth.yj202588.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zcr.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sih.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fri.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ybm.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bdv.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://udk.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://phh.ydjk.org.cn

[E14] URL 编码与 Base64
来源：http://lzn.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ibp.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wrg.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lts.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jgi.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://now.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xev.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://imc.yonumen.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tun.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://aja.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pti.aibaodan.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bym.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dam.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://lsx.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zvl.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ffv.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://igd.yangfankeji.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jqg.chenzaomai.com

[E16] 数字千分位
来源：http://vjo.uphjek.com

Py:   f"{1234567:,}"
来源：http://khx.sysykeji.top

PHP:  number_format(1234567);
来源：http://exg.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nnw.quarkkingdee.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ons.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tnt.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jwk.guowangkeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cfb.hammf.cn

C#:   1234567.ToString("N0")
来源：http://fct.chenlongwang.top

[E17] 首字母大写
来源：http://lbx.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mcb.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jje.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zzi.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jjc.jinqigufen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bet.hysaishi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rmp.hcnkem.com

Ruby: s.capitalize
来源：http://koo.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ibi.hywenlv.cn

[E18] 模板占位符替换
来源：http://uvz.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qcl.kuanghao11.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xzt.zdbjq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://goo.zhengqikj.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wvi.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cac.hongshengwenyu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gys.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tsl.yj20258888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tzy.aizwys.cn

[E19] 多行文本按行拆分
来源：http://bpg.zhixingplan.top

Py:   s.splitlines()
来源：http://aqm.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbs.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://fno.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://oic.vqdsnc.cn

Java: s.lines().toList()
来源：http://pkx.vehdjk.com

Go:   strings.Split(s, "\n")
来源：http://izp.gotoacloud.top

Ruby: s.lines
来源：http://yhj.cqqwz.cn

C#:   s.Split('\n')
来源：http://xue.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://yjm.hysaishi.cn

Py:   if not s:
来源：http://xjh.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ngk.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lfm.zhixingplan.top

TS:   if (s === "") {}
来源：http://wpt.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://yzu.vehdjk.com

Go:   if s == "" {}
来源：http://lvr.c1oappe.top

Ruby: if s.empty?
来源：http://wnn.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ckg.zycfv.cn

[E21] 超长截断加省略号
来源：http://vjj.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oek.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qzc.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gxj.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aro.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://srd.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://iie.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xef.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://txg.fehbvm.com

[E22] 字节长度与字符长度
来源：http://mcd.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ywx.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://apm.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hrp.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uvp.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xgi.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wnx.316326.xyz

Ruby: s.bytesize;  s.length
来源：http://xjl.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mwf.xylfe.cn

================================================================================
来源：http://uzg.ydjk.org.cn

F. 文件与目录
来源：http://tbb.sjlbkw.cn

================================================================================
来源：http://hnu.ivvv.top

[F01] 读取整个文件
来源：http://ova.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ngt.smart0.xyz

PHP:  file_get_contents("a.txt");
来源：http://jva.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hzz.zhaomingkeji.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fdq.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ofe.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pzj.iojbl.cn

Ruby: File.read("a.txt")
来源：http://yrf.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://liq.jlsjyb.cn

[F02] 逐行读取文件
来源：http://fxn.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aad.cashguo.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gbl.zdqjudy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fub.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lkq.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://npe.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rgp.tian-w.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oer.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sgm.jqgufenzy.top

[F03] 写入文件（覆盖）
来源：http://olh.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://een.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mfu.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kkd.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgw.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iar.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fkt.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://opd.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ivy.tarul.cn

[F04] 追加写入文件
来源：http://xmx.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uil.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sdl.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rsg.tian-w.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzk.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jet.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ffl.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xws.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oye.jqgufenzy.top

[F05] 判断文件或目录是否存在
来源：http://fse.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://huh.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://woz.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://kvi.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://scs.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jsy.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pyl.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://ehi.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://awc.hnqzz.top

[F06] 删除文件
来源：http://shf.mhx1999.top

Py:   os.remove("a.txt")
来源：http://gdz.ywan-chungtsiang.top

PHP:  unlink("a.txt");
来源：http://zdb.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://qxo.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://ewl.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ckb.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://yes.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://glq.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://hrm.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://hsl.vehdjk.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nnk.yanxiufei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jkf.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kyh.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwn.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hcs.tianlin.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pkl.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hqk.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://syl.shzxlz.cn

[F08] 遍历目录
来源：http://ymo.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yny.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vvq.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://vix.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://bqw.cdnleiting.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mfo.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://rps.hesvh.cn

Ruby: Dir.children("dir")
来源：http://naj.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://pgb.nanxinkj.top

[F09] 获取文件大小
来源：http://cbl.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://jxt.daxiang520.top

PHP:  filesize("a.txt");
来源：http://pig.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://avn.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://lip.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://vey.daxiang520.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://omd.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://qfw.tianlin.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ijg.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://zte.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eow.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ujb.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fyc.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://zbm.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pju.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ldu.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pob.ehwqpu.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pzb.tian-w.cn

[F11] 复制与移动文件
来源：http://eyd.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rfy.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vwh.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eqc.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://khx.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ipp.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vbr.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://myo.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jkf.yvedp.cn

[F12] CSV 读写
来源：http://wqm.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tia.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kqy.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gta.xinyue.icu

TS:   // 同上
来源：http://eda.chenlongwang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mxy.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hpz.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ykd.nanxinkj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yji.sjlbkw.cn

================================================================================
来源：http://mym.chenzaomai.com

G. 面向对象
来源：http://fxr.svipenyu.cn

================================================================================
来源：http://ugn.pengpengdd.cyou

[G01] 定义类
来源：http://hmw.shangyingyoupin.top

Py:   class User: pass
来源：http://ubc.vqdsnc.cn

PHP:  class User {}
来源：http://qxj.jinyuanbaomall.cn

JS:   class User {}
来源：http://vmj.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://kcl.nanxuanxn.top

Java: class User {}
来源：http://tmg.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://cga.bbcook.cn

Ruby: class User; end
来源：http://zns.dianchejie.cn

C#:   class User {}
来源：http://oxf.zhijiandao.cn

[G02] 构造函数
来源：http://wwe.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://rtc.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://dwh.epnwcf.com

JS:   constructor(name) { this.name = name; }
来源：http://guf.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://uho.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://pzf.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hbf.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://hwd.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://jqw.52xcode.cn

[G03] 实例属性
来源：http://gnx.jinqigfzy.top

Py:   self.name = "x"
来源：http://pep.sxryk.cn

PHP:  public string $name = "x";
来源：http://fjz.dashuyun.cn

JS:   this.name = "x";
来源：http://uvb.aibaodan.cn

TS:   name: string = "x";
来源：http://wxe.yongpay.top

Java: private String name;
来源：http://keq.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ufh.ppjwa.cn

Ruby: @name = "x"
来源：http://zfy.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://ypt.bbcook.cn

[G04] 定义方法
来源：http://ezn.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://uug.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mkk.yonumen.top

JS:   greet() { return this.name; }
来源：http://uqw.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://vgj.ctjpmb.com

Java: String greet() { return name; }
来源：http://fwy.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wqp.yongpay.top

Ruby: def greet; @name; end
来源：http://mnt.uphjek.com

C#:   public string Greet() => Name;
来源：http://lhd.yangfankeji.com

[G05] 继承
来源：http://cwe.redwolf501.top

Py:   class Admin(User): pass
来源：http://boh.yueranfly.top

PHP:  class Admin extends User {}
来源：http://scp.cqqwz.cn

JS:   class Admin extends User {}
来源：http://ofc.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://gqo.xziqi.cn

Java: class Admin extends User {}
来源：http://xvq.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jqo.tian-w.cn

Ruby: class Admin < User; end
来源：http://ofc.jlsjyb.cn

C#:   class Admin : User {}
来源：http://lna.feifeiyinyue.top

[G06] 重写方法
来源：http://zua.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://tzl.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ezb.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://prv.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://jbe.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://dpv.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibu.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://tqn.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://wkd.fengsongda.top

[G07] 调用父类方法
来源：http://rti.aizwys.cn

Py:   super().greet()
来源：http://hmm.jinqigufen.top

PHP:  parent::greet();
来源：http://swf.cdnleiting.top

JS:   super.greet();
来源：http://qqd.c1oappe.top

TS:   super.greet();
来源：http://byl.tianlin.xyz

Java: super.greet();
来源：http://rzw.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jen.shangyingyoupin.top

Ruby: super
来源：http://rht.xziqi.cn

C#:   base.Greet();
来源：http://mjr.yangfankeji.com

[G08] 静态方法与属性
来源：http://idm.uphjek.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ueg.havefunace.top

PHP:  public static function f() {}
来源：http://eii.jinyuanbaomall.cn

JS:   static f() {}
来源：http://yam.sxryk.cn

TS:   static f(): void {}
来源：http://sas.cashguo.top

Java: static void f() {}
来源：http://zgv.yonumen.top


<!-- 参考信息 -->