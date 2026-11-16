代发 wailian999

JS:   [...s].reverse().join("")
来源：http://zvy.gotoacloud.top

TS:   [...s].reverse().join("")
来源：http://eal.cdnleiting.top

Java: new StringBuilder(s).reverse().toString()
来源：http://clv.meibo888.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://twr.guowangkeji.top

Ruby: s.reverse
来源：http://nab.svipenyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://toq.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://qpt.yvedp.cn

Py:   s.count("a")
来源：http://rfw.0kj1m.cn

PHP:  substr_count($s, "a");
来源：http://aqy.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://oex.yj202588.top

TS:   s.split("a").length - 1
来源：http://nfb.andypj.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kvq.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://bpu.guannengcc.top

Ruby: s.count("a")
来源：http://ymh.zhijiandao.cn

C#:   s.Count(c => c == 'a')
来源：http://kfj.zdbjq.cn

[E13] 逐字符遍历
来源：http://eqj.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://sdd.sufxvd.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rak.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://fre.hnxiangtu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://whd.pycfn.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wrd.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zcs.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dee.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aay.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://lxc.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://syq.gogol.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ang.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nji.shangyingyoupin.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tql.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://owm.nwbrower.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hth.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iwb.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yop.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://gkb.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tav.zhiwuduotai.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sab.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lwh.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lnp.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nth.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ewl.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lcx.bjfxy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xzm.smart0.xyz

[E16] 数字千分位
来源：http://pfn.vqdsnc.cn

Py:   f"{1234567:,}"
来源：http://xjd.gzhubu.top

PHP:  number_format(1234567);
来源：http://rdi.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://edl.sxryk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://crc.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pgw.daria6918.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://thv.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qez.iojbl.cn

C#:   1234567.ToString("N0")
来源：http://xah.vqdsnc.cn

[E17] 首字母大写
来源：http://amo.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nwk.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xek.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kuv.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ujl.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yig.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hfm.wangshuangyany.cn

Ruby: s.capitalize
来源：http://mrq.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://srn.ctjpmb.com

[E18] 模板占位符替换
来源：http://fbq.sxryk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://psy.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gxp.nanxuanxn.top

JS:   tpl.replaceAll("{name}", name)
来源：http://roo.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://jot.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://elw.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lvs.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://awj.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lme.cashguo.top

[E19] 多行文本按行拆分
来源：http://zuq.daxiang520.top

Py:   s.splitlines()
来源：http://bnn.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://box.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://nlv.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://gry.aizwys.cn

Java: s.lines().toList()
来源：http://htc.kuanghao11.cn

Go:   strings.Split(s, "\n")
来源：http://jpm.yanxiufei.cn

Ruby: s.lines
来源：http://iwz.ppjwa.cn

C#:   s.Split('\n')
来源：http://wsl.ybcxt.top

[E20] 判断字符串是否为空
来源：http://nth.vehdjk.com

Py:   if not s:
来源：http://yso.tarul.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cuz.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nbs.gotoacloud.top

TS:   if (s === "") {}
来源：http://pad.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://jyw.c1oappe.top

Go:   if s == "" {}
来源：http://cmh.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://yqr.sysykeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dmc.yj202588.top

[E21] 超长截断加省略号
来源：http://xng.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oqr.hnxiangtu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kvf.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xro.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rmq.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aiq.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://uvo.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ply.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://keb.zdqjudy.top

[E22] 字节长度与字符长度
来源：http://jun.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hxh.sweek.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qlx.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zfp.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vod.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dno.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dug.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://oyq.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xqh.vehdjk.com

================================================================================
来源：http://hku.gogol.net.cn

F. 文件与目录
来源：http://ggt.daria6918.cn

================================================================================
来源：http://xol.guowangkeji.top

[F01] 读取整个文件
来源：http://wmq.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xkj.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://lax.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pfc.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jfq.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://khm.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://khn.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://uob.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://oen.vehdjk.com

[F02] 逐行读取文件
来源：http://dny.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anv.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://upn.c1oappe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lfq.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wam.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sgr.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://neo.gzhubu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zym.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ivi.yj20258.top

[F03] 写入文件（覆盖）
来源：http://pfd.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ycq.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nnl.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://avb.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ltn.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eby.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kit.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://kov.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dpf.zdbjq.cn

[F04] 追加写入文件
来源：http://qnm.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jby.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://olc.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chi.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dke.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gqs.cashguo.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vyl.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://diw.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gjj.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://olh.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eew.guannengcc.top

PHP:  file_exists("a.txt");
来源：http://pdg.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://lzq.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://lid.chenjidiqi.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://keb.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://swl.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://kxs.iojbl.cn

C#:   File.Exists("a.txt")
来源：http://rnd.uphjek.com

[F06] 删除文件
来源：http://ehm.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://wbg.yvedp.cn

PHP:  unlink("a.txt");
来源：http://rzf.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://ucm.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://loz.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rvz.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://eru.sysykeji.top

Ruby: File.delete("a.txt")
来源：http://res.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://axh.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://fzb.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lvx.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hse.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sbd.yuanzhike.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tca.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sjt.9152youxi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gbi.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dav.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cit.iojbl.cn

[F08] 遍历目录
来源：http://zhz.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ihm.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://odh.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://mbb.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://jpv.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hwz.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rzu.fzhhl.top

Ruby: Dir.children("dir")
来源：http://xbp.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://dhk.pengpengdd.cyou

[F09] 获取文件大小
来源：http://jrn.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://uui.quarkkingdee.top

PHP:  filesize("a.txt");
来源：http://hhc.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://adb.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://gps.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://ewt.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://txr.c1oappe.top

Ruby: File.size("a.txt")
来源：http://zlr.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://hew.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://kqd.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rbq.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kfv.ppjwa.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://psw.hywenlv.cn

TS:   path.extname("a.txt")
来源：http://fgf.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ugc.bbcook.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uoi.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zye.jianghu66.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dgy.guannengcc.top

[F11] 复制与移动文件
来源：http://bzv.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fgx.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://omn.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbp.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvg.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rvj.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wfc.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bxm.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ndn.shangyingyoupin.top

[F12] CSV 读写
来源：http://xnz.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pve.tian-w.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gdw.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tow.ywan-chungtsiang.top

TS:   // 同上
来源：http://xsg.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sey.sjlbkw.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lri.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eae.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mre.tanke756.top

================================================================================
来源：http://odj.tanke756.top

G. 面向对象
来源：http://ill.jinghuilouyu.cn

================================================================================
来源：http://ldu.hcnkem.com

[G01] 定义类
来源：http://qrj.haohaochexian.top

Py:   class User: pass
来源：http://jen.yanxiufei.cn

PHP:  class User {}
来源：http://elu.hongshengwenyu.top

JS:   class User {}
来源：http://bqw.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://wdo.sjlbkw.cn

Java: class User {}
来源：http://ttn.wangdashe.top

Go:   type User struct { Name string }
来源：http://qyq.hongshengwenyu.top

Ruby: class User; end
来源：http://yuw.yj20258888.top

C#:   class User {}
来源：http://qxz.shanyushiyangtech.top

[G02] 构造函数
来源：http://pzb.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://ymr.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://ikp.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://fgv.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://oip.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://jbv.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tia.wangdashe.top

Ruby: def initialize(name); @name = name; end
来源：http://abg.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://noq.sufxvd.cn

[G03] 实例属性
来源：http://mpw.9152youxi.cn

Py:   self.name = "x"
来源：http://kxg.yueranfly.top

PHP:  public string $name = "x";
来源：http://ybp.cheryme.top

JS:   this.name = "x";
来源：http://nac.xylfe.cn

TS:   name: string = "x";
来源：http://utu.chenjidiqi.icu

Java: private String name;
来源：http://bnn.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jrn.pycfn.com

Ruby: @name = "x"
来源：http://yvp.ybcxt.top

C#:   public string Name { get; set; } = "x";
来源：http://wfb.yonumen.top

[G04] 定义方法
来源：http://kbq.yuxming.cn

Py:   def greet(self): return self.name
来源：http://mpu.vqdsnc.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wdu.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://hph.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://ivv.bbcook.cn

Java: String greet() { return name; }
来源：http://xka.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ilk.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://mqa.smart0.xyz

C#:   public string Greet() => Name;
来源：http://nly.0kj1m.cn

[G05] 继承
来源：http://dxc.quarkkingdee.top

Py:   class Admin(User): pass
来源：http://jed.sysykeji.top

PHP:  class Admin extends User {}
来源：http://bko.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://vsn.nanxinkj.top

TS:   class Admin extends User {}
来源：http://wet.cashguo.top

Java: class Admin extends User {}
来源：http://sjr.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aiz.316326.xyz

Ruby: class Admin < User; end
来源：http://rcx.wangdashe.top

C#:   class Admin : User {}
来源：http://gej.feifeiyinyue.top

[G06] 重写方法
来源：http://qbc.havefunace.top

Py:   def greet(self): return "admin"
来源：http://iin.ydjk.org.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wfp.gzhubu.top

JS:   greet() { return "admin"; }
来源：http://vqg.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://ggi.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://iyr.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bwm.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://wet.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://fbn.chenzaomai.com

[G07] 调用父类方法
来源：http://xqs.jinqigufen.top

Py:   super().greet()
来源：http://dwj.sufxvd.cn

PHP:  parent::greet();
来源：http://wyr.hesvh.cn

JS:   super.greet();
来源：http://sxd.meibo888.top

TS:   super.greet();
来源：http://fht.xylfe.cn

Java: super.greet();
来源：http://qdl.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vks.hammf.cn

Ruby: super
来源：http://qlk.52xcode.cn

C#:   base.Greet();
来源：http://iex.9152youxi.cn

[G08] 静态方法与属性
来源：http://yea.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://udz.yj20258888.top

PHP:  public static function f() {}
来源：http://ext.cqqwz.cn

JS:   static f() {}
来源：http://kdx.tanke756.top

TS:   static f(): void {}
来源：http://imo.epnwcf.com

Java: static void f() {}
来源：http://fxr.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://lbf.feifeiyinyue.top

Ruby: def self.f; end
来源：http://hqc.yfazqb.com

C#:   public static void F() {}
来源：http://kkp.meibo888.top

[G09] 接口 / 抽象类
来源：http://gce.chenlongwang.top

Py:   from abc import ABC, abstractmethod
来源：http://sih.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://qmd.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hzp.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://yre.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://noj.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://rij.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dhq.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://iaq.fehbvm.com


<!-- 参考信息 -->