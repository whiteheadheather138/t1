代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://cvc.hammf.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lil.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lku.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://cua.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://pjr.gaohongyu789.top

Java: String.format("%03d", 7)
来源：http://eos.quarkkingdee.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://axd.ppjwa.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://igf.iojbl.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qxn.hcnkem.com

[E11] 反转字符串
来源：http://qyu.aizwys.cn

Py:   s[::-1]
来源：http://koe.havefunace.top

PHP:  strrev($s);
来源：http://qep.316326.xyz

JS:   [...s].reverse().join("")
来源：http://qnw.havefunace.top

TS:   [...s].reverse().join("")
来源：http://aip.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://izd.yanxiufei.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mvk.smart0.xyz

Ruby: s.reverse
来源：http://nas.andypj.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qbj.tanke756.top

[E12] 统计某字符出现次数
来源：http://tpw.sweek.top

Py:   s.count("a")
来源：http://cya.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://nbe.hcnkem.com

JS:   s.split("a").length - 1
来源：http://jbq.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://mfs.iojbl.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ivl.vehdjk.com

Go:   strings.Count(s, "a")
来源：http://xuo.zhengqikj.top

Ruby: s.count("a")
来源：http://uex.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://ige.xziqi.cn

[E13] 逐字符遍历
来源：http://irr.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://nrw.hesvh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gpi.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cbe.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://uxn.52xcode.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://huo.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://slf.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bkl.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hjv.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://kio.bbcook.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynn.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://vgv.9152youxi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zmi.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gff.epnwcf.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ysf.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ieq.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cpk.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ymp.hammf.cn

[E15] HTML 转义 / 反转义
来源：http://hpw.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://psq.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ivh.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tun.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dvn.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kms.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rdr.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dhk.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cht.hcnkem.com

[E16] 数字千分位
来源：http://myd.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://upw.vqdsnc.cn

PHP:  number_format(1234567);
来源：http://vhz.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://qxx.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yro.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nhp.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgr.wangdashe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dfk.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://bzr.cdnleiting.top

[E17] 首字母大写
来源：http://rbn.shzxlz.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gig.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nlt.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umi.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ehd.ivvv.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ega.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pxk.tianlin.xyz

Ruby: s.capitalize
来源：http://iey.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vkm.hesvh.cn

[E18] 模板占位符替换
来源：http://fgn.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://trz.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://obw.daxiang520.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ucp.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bdi.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jqw.zhixingplan.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nmn.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ubo.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://stt.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://jth.yuxming.cn

Py:   s.splitlines()
来源：http://crw.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uht.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://xmc.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://con.andypj.xyz

Java: s.lines().toList()
来源：http://hzh.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://htc.ehwqpu.com

Ruby: s.lines
来源：http://hda.kuanghao11.cn

C#:   s.Split('\n')
来源：http://kyy.bbcook.cn

[E20] 判断字符串是否为空
来源：http://zsv.nwbrower.top

Py:   if not s:
来源：http://jlp.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wfc.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jwn.chenzaomai.com

TS:   if (s === "") {}
来源：http://ekg.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://ngs.zhiwuduotai.top

Go:   if s == "" {}
来源：http://pvk.xuetiantiany.cn

Ruby: if s.empty?
来源：http://iez.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nrn.yj202588.top

[E21] 超长截断加省略号
来源：http://czu.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cgw.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mhu.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wxu.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kkb.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yqp.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://arg.chenjidiqi.icu

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vbt.yuxming.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ixh.yongpay.top

[E22] 字节长度与字符长度
来源：http://fqb.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vbc.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fux.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rgi.sxryk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oxx.epnwcf.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sja.wangshuangyany.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nuo.jinghuilouyu.cn

Ruby: s.bytesize;  s.length
来源：http://fjd.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pao.yuanzhike.top

================================================================================
来源：http://guo.jqgfzy.top

F. 文件与目录
来源：http://fpl.zhixingplan.top

================================================================================
来源：http://vto.yueranfly.top

[F01] 读取整个文件
来源：http://iyb.daria6918.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pai.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://zqe.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ilq.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tdh.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tbp.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ohj.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://ukm.yonumen.top

C#:   File.ReadAllText("a.txt");
来源：http://dib.daxiang520.top

[F02] 逐行读取文件
来源：http://atd.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hxi.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sjj.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mew.ehwqpu.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dhb.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wmg.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://poc.haohaochexian.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qxb.xinyue.icu

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dia.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://ipv.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dtm.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oxw.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubc.mhx1999.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vmd.hammf.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hmc.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hvy.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://ype.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lzr.c1oappe.top

[F04] 追加写入文件
来源：http://gya.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://udo.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sgj.jianghu66.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ocf.fehbvm.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zgt.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dyq.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dfz.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rkk.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://doj.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://vei.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ycs.meibo888.top

PHP:  file_exists("a.txt");
来源：http://plf.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://ton.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://kfe.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pxx.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://saf.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://huz.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://ndd.xuetiantiany.cn

[F06] 删除文件
来源：http://hul.chenjidiqi.icu

Py:   os.remove("a.txt")
来源：http://xui.aizwys.cn

PHP:  unlink("a.txt");
来源：http://vcc.dianchejie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vln.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://tny.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mog.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://dbz.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://swh.yj202588.top

C#:   File.Delete("a.txt");
来源：http://btn.jyoumei.cn

[F07] 创建目录（含多级）
来源：http://nhx.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yvc.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kfs.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ehn.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cea.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jfi.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://faz.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oru.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uzr.nwbrower.top

[F08] 遍历目录
来源：http://txk.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gwy.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ody.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://skr.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://iym.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rft.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nro.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://zcd.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://emd.hysaishi.cn

[F09] 获取文件大小
来源：http://fet.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://kup.uphjek.com

PHP:  filesize("a.txt");
来源：http://xqq.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://qmx.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://iek.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yos.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ohz.fktsv.cn

Ruby: File.size("a.txt")
来源：http://rmm.tarul.cn

C#:   new FileInfo("a.txt").Length
来源：http://gvd.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://qlc.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fzu.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://elh.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kdn.hcnkem.com

TS:   path.extname("a.txt")
来源：http://iff.quarkkingdee.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xfs.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvc.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://odj.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nfu.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://cra.aibaodan.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bse.ydjk.org.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://irg.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eop.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynq.tanke756.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iox.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ssz.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://djz.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yla.sxryk.cn

[F12] CSV 读写
来源：http://eyo.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jel.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gac.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jfx.uphjek.com

TS:   // 同上
来源：http://wza.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mkt.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jjb.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xxq.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ayk.shangyingyoupin.top

================================================================================
来源：http://cgh.snrcjt.cn

G. 面向对象
来源：http://zwm.yongpay.top

================================================================================
来源：http://zgp.jlsjyb.cn

[G01] 定义类
来源：http://sue.zhijiandao.cn

Py:   class User: pass
来源：http://tbc.yonumen.top

PHP:  class User {}
来源：http://ktm.dashuyun.cn

JS:   class User {}
来源：http://hqn.cashguo.top

TS:   class User { name: string = ""; }
来源：http://nmp.birdmap.top

Java: class User {}
来源：http://kes.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://kex.sxryk.cn

Ruby: class User; end
来源：http://mgc.havefunace.top

C#:   class User {}
来源：http://fzu.zhengqikj.top

[G02] 构造函数
来源：http://sgu.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://wtg.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://kmq.guannengcc.top

JS:   constructor(name) { this.name = name; }
来源：http://gdb.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://zvg.cashguo.top

Java: User(String name) { this.name = name; }
来源：http://xza.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gcy.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://fml.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://zzf.bjfxy.top

[G03] 实例属性
来源：http://bbv.snrcjt.cn

Py:   self.name = "x"
来源：http://ozb.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://sdg.yfazqb.com

JS:   this.name = "x";
来源：http://wfa.jlsjyb.cn

TS:   name: string = "x";
来源：http://lrz.ppjwa.cn

Java: private String name;
来源：http://yrf.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://isg.gzhubu.top

Ruby: @name = "x"
来源：http://ngp.gaohongyu789.top

C#:   public string Name { get; set; } = "x";
来源：http://nag.316326.xyz

[G04] 定义方法
来源：http://kyf.epnwcf.com

Py:   def greet(self): return self.name
来源：http://qlj.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lnr.nanxinkj.top

JS:   greet() { return this.name; }
来源：http://dth.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://vmd.fehbvm.com

Java: String greet() { return name; }
来源：http://gaj.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vcj.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://cxe.hcnkem.com

C#:   public string Greet() => Name;
来源：http://noa.redwolf501.top

[G05] 继承
来源：http://naj.dashuyun.cn

Py:   class Admin(User): pass
来源：http://fkw.yonumen.top

PHP:  class Admin extends User {}
来源：http://prz.shuidangran.top

JS:   class Admin extends User {}
来源：http://lej.yj202588.top

TS:   class Admin extends User {}
来源：http://ble.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://dyh.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kcu.tarul.cn

Ruby: class Admin < User; end
来源：http://txu.tanke756.top

C#:   class Admin : User {}
来源：http://yjr.cucudq.cn

[G06] 重写方法
来源：http://kxd.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://dto.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gcw.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://pxn.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://kro.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://nxa.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwh.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://uzh.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://wuh.jqgfzy.top

[G07] 调用父类方法
来源：http://gbq.pengpengdd.cyou

Py:   super().greet()
来源：http://ysr.mhx1999.top

PHP:  parent::greet();
来源：http://pvd.mhx1999.top

JS:   super.greet();
来源：http://mkv.daria6918.cn

TS:   super.greet();
来源：http://rsq.xingfuxueyuan.xyz

Java: super.greet();
来源：http://dib.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vpd.gaohongyu789.top

Ruby: super
来源：http://yfr.guowangkeji.top

C#:   base.Greet();
来源：http://iid.yuxming.cn

[G08] 静态方法与属性
来源：http://wya.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dps.andypj.xyz

PHP:  public static function f() {}
来源：http://ews.52xcode.cn

JS:   static f() {}
来源：http://eix.shanyushiyangtech.top

TS:   static f(): void {}
来源：http://ymu.yfazqb.com

Java: static void f() {}
来源：http://vof.zhiwuduotai.top


<!-- 参考信息 -->