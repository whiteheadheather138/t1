代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://bjm.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://twc.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ktx.hnxiangtu.top

JS:   "7".padStart(3, "0")
来源：http://bwx.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://obg.hammf.cn

Java: String.format("%03d", 7)
来源：http://ylc.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://gmf.fktsv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oes.tianlin.xyz

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gnd.sjlbkw.cn

[E11] 反转字符串
来源：http://txo.yuanzhike.top

Py:   s[::-1]
来源：http://xaw.uphjek.com

PHP:  strrev($s);
来源：http://lzh.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://fnl.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://vik.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://frp.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://usi.shanyushiyangkeji.top

Ruby: s.reverse
来源：http://clr.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://amu.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://zxo.fehbvm.com

Py:   s.count("a")
来源：http://ofu.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://btn.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://gvn.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://mzu.yj20258.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uip.havefunace.top

Go:   strings.Count(s, "a")
来源：http://xwf.feifeiyinyue.top

Ruby: s.count("a")
来源：http://dyg.gaohongyu789.top

C#:   s.Count(c => c == 'a')
来源：http://zvb.wangdashe.top

[E13] 逐字符遍历
来源：http://nno.tarul.cn

Py:   for ch in s: print(ch)
来源：http://vga.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yur.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://rwr.aizwys.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qjx.hcnkem.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oup.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pta.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uou.316326.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wzd.hcnkem.com

[E14] URL 编码与 Base64
来源：http://ufw.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jvi.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://hag.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kvs.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vyw.snrcjt.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ygc.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qrt.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dtr.jqgfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sfb.316326.xyz

[E15] HTML 转义 / 反转义
来源：http://cpi.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zfr.andypj.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://chx.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mqy.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kiv.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dtu.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qfq.shanyushiyangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tlb.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ljo.aizwys.cn

[E16] 数字千分位
来源：http://rfi.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://wna.sufxvd.cn

PHP:  number_format(1234567);
来源：http://skm.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vjk.fehbvm.com

TS:   (1234567).toLocaleString("en-US")
来源：http://zvz.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jbt.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hnr.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sjn.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://ura.jqgfzy.top

[E17] 首字母大写
来源：http://zda.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lln.chenzaomai.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://utp.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nxi.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ffg.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uoa.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xyp.birdmap.top

Ruby: s.capitalize
来源：http://myq.snrcjt.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ghf.svipenyu.cn

[E18] 模板占位符替换
来源：http://xym.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uqu.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://whc.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ixh.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ogk.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mhi.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ota.svipenyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://soz.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dbg.bjfxy.top

[E19] 多行文本按行拆分
来源：http://sfh.yj20258.top

Py:   s.splitlines()
来源：http://tqs.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zqi.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://qpc.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://fgc.cdnleiting.top

Java: s.lines().toList()
来源：http://exh.sweek.top

Go:   strings.Split(s, "\n")
来源：http://orp.redwolf501.top

Ruby: s.lines
来源：http://aqj.sjlbkw.cn

C#:   s.Split('\n')
来源：http://oig.iojbl.cn

[E20] 判断字符串是否为空
来源：http://prs.chenzaomai.com

Py:   if not s:
来源：http://ngh.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://umh.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hks.52xcode.cn

TS:   if (s === "") {}
来源：http://epm.sysykeji.top

Java: if (s.isEmpty()) {}
来源：http://kwj.kuanghao11.cn

Go:   if s == "" {}
来源：http://jdv.dashuyun.cn

Ruby: if s.empty?
来源：http://ulz.jianghu66.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vqb.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://nkh.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://syv.shuidangran.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cyl.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gis.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fss.chenlongwang.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iag.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://hyc.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hsh.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xng.aibaodan.cn

[E22] 字节长度与字符长度
来源：http://ogq.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qha.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://maz.havefunace.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vty.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://klg.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tqt.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fnt.xinyue.icu

Ruby: s.bytesize;  s.length
来源：http://qyf.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dsm.wangdashe.top

================================================================================
来源：http://nap.yueranfly.top

F. 文件与目录
来源：http://dii.yueranfly.top

================================================================================
来源：http://avo.yfazqb.com

[F01] 读取整个文件
来源：http://foc.havefunace.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jcu.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://srq.chenzaomai.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ttt.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sfe.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lvq.zhaomingkeji.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uut.andypj.xyz

Ruby: File.read("a.txt")
来源：http://lgu.zhengqikj.top

C#:   File.ReadAllText("a.txt");
来源：http://gcn.0kj1m.cn

[F02] 逐行读取文件
来源：http://zce.shuidangran.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nsw.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omd.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jmt.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://smf.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://brp.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://epj.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gug.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vxa.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://kpe.0kj1m.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://quo.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cyz.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ien.meibo888.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnj.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sog.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qta.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://sgn.yfazqb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kli.hongshengwenyu.top

[F04] 追加写入文件
来源：http://yxt.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ftf.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cdc.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kic.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmc.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mdl.nanxinkj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rmm.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zyx.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://udg.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://tbw.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dpb.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://gjn.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://biy.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://ibn.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rby.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xsq.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://skm.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://zix.jinyuanbaomall.cn

[F06] 删除文件
来源：http://bhc.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://cfm.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://ryb.iojbl.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ikn.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://jht.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rlk.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://bsx.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://buz.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://swv.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://scj.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vje.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dlj.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hww.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dek.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yqe.haohaochexian.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://goo.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ltm.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ktl.shzxlz.cn

[F08] 遍历目录
来源：http://iqf.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zkm.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jkz.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://fpf.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://acu.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bpe.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xms.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://pvn.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://yuv.zhoulong.xyz

[F09] 获取文件大小
来源：http://zwa.pycfn.com

Py:   os.path.getsize("a.txt")
来源：http://nbg.daxiang520.top

PHP:  filesize("a.txt");
来源：http://ujs.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://eje.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://xvb.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ucm.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cnf.ydzc1.top

Ruby: File.size("a.txt")
来源：http://too.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://xte.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://kko.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yel.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ics.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sim.xinyue.icu

TS:   path.extname("a.txt")
来源：http://uzq.zhoulong.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ccy.jianghu66.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xan.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qwh.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kvu.zdbjq.cn

[F11] 复制与移动文件
来源：http://psu.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://odw.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uwm.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onn.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpn.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxz.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kcn.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nzn.yanxiufei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://npv.jinqigfzy.top

[F12] CSV 读写
来源：http://oot.9152youxi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ffl.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxs.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kdk.hysaishi.cn

TS:   // 同上
来源：http://dbb.yonumen.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://glg.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gmm.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pey.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://urr.birdmap.top

================================================================================
来源：http://gax.fanxiaobao.xyz

G. 面向对象
来源：http://oeh.xingfuxueyuan.xyz

================================================================================
来源：http://hgc.hfpthk.cn

[G01] 定义类
来源：http://qwj.chenlongwang.top

Py:   class User: pass
来源：http://fmq.fzhhl.top

PHP:  class User {}
来源：http://vnz.birdmap.top

JS:   class User {}
来源：http://rgs.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://xhy.316326.xyz

Java: class User {}
来源：http://ufh.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://rqa.meibo888.top

Ruby: class User; end
来源：http://pwc.jinqigfzy.top

C#:   class User {}
来源：http://kdy.sjlbkw.cn

[G02] 构造函数
来源：http://grn.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://xgc.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://onf.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://ael.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://yhv.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://zok.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yaq.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://lgc.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://fbd.zhengqikj.top

[G03] 实例属性
来源：http://xxc.jinqigfzy.top

Py:   self.name = "x"
来源：http://dyn.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://pmm.yj20258.top

JS:   this.name = "x";
来源：http://gai.hfpthk.cn

TS:   name: string = "x";
来源：http://vca.yfazqb.com

Java: private String name;
来源：http://hay.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bwf.jqgufenzy.top

Ruby: @name = "x"
来源：http://mix.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://ezh.gzhubu.top

[G04] 定义方法
来源：http://kcs.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://wfe.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fbl.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://fqe.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://xfn.hcnkem.com

Java: String greet() { return name; }
来源：http://zcu.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://esw.316326.xyz

Ruby: def greet; @name; end
来源：http://vjm.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://jnz.ivvv.top

[G05] 继承
来源：http://mwn.sweek.top

Py:   class Admin(User): pass
来源：http://yzi.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://ena.ydzc1.top

JS:   class Admin extends User {}
来源：http://bns.c1oappe.top

TS:   class Admin extends User {}
来源：http://kry.nwbrower.top

Java: class Admin extends User {}
来源：http://fsa.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://noj.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://ikh.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://pjf.zhiwuduotai.top

[G06] 重写方法
来源：http://kgt.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://ide.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kyc.316326.xyz

JS:   greet() { return "admin"; }
来源：http://hai.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://jpv.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://jmx.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jng.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://yqs.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://zlr.zdbjq.cn

[G07] 调用父类方法
来源：http://tte.yj20258888.top

Py:   super().greet()
来源：http://zis.hesvh.cn

PHP:  parent::greet();
来源：http://spi.cqqwz.cn

JS:   super.greet();
来源：http://vgw.shanyushiyangkeji.top

TS:   super.greet();
来源：http://drb.fzhhl.top

Java: super.greet();
来源：http://llp.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://doq.nwbrower.top

Ruby: super
来源：http://fqt.pycfn.com

C#:   base.Greet();
来源：http://nht.svipenyu.cn

[G08] 静态方法与属性
来源：http://ojj.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wdz.yuanzhike.top

PHP:  public static function f() {}
来源：http://knl.hywenlv.cn

JS:   static f() {}
来源：http://ajj.hnxiangtu.top

TS:   static f(): void {}
来源：http://rjq.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://ojp.xuetiantiany.cn


<!-- 参考信息 -->