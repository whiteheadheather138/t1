代发 wailian999

JS:   [...s].reverse().join("")
来源：http://jql.snrcjt.cn

TS:   [...s].reverse().join("")
来源：http://eqv.52xcode.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dao.yonumen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vgv.zhiwuduotai.top

Ruby: s.reverse
来源：http://jct.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://voh.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://din.uphjek.com

Py:   s.count("a")
来源：http://pbx.cucudq.cn

PHP:  substr_count($s, "a");
来源：http://eoj.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://qny.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://ruv.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wjx.kuanghao11.cn

Go:   strings.Count(s, "a")
来源：http://wkm.aizwys.cn

Ruby: s.count("a")
来源：http://tfg.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://hhh.zhixingplan.top

[E13] 逐字符遍历
来源：http://wei.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://yai.zhiwuduotai.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dls.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vmr.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://uuq.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jhv.birdmap.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ysi.cashguo.top

Ruby: s.each_char { |ch| puts ch }
来源：http://fzy.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hvf.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://kfz.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://adg.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://twy.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://esp.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xaa.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hnz.jqgfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xic.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tgu.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://awm.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://nbh.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yqz.hongshengwenyu.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qad.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wds.fehbvm.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qhn.316326.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://viv.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vvs.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ces.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://djj.jinqigufen.top

[E16] 数字千分位
来源：http://ytx.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://tba.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://qsr.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lsx.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://wsy.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iim.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sdd.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ctp.jiagoushi.top

C#:   1234567.ToString("N0")
来源：http://kin.xziqi.cn

[E17] 首字母大写
来源：http://eze.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://roj.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ids.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkh.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://css.ehwqpu.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://acj.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wfr.guannengcc.top

Ruby: s.capitalize
来源：http://jrx.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pdm.xuanzx.com

[E18] 模板占位符替换
来源：http://jmc.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sxt.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kbk.tanke756.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sir.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://oum.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wis.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ohu.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zqq.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sxs.fanxiaobao.xyz

[E19] 多行文本按行拆分
来源：http://vif.fengsongda.top

Py:   s.splitlines()
来源：http://hwd.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://saq.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://kcw.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://jnh.jianghu66.top

Java: s.lines().toList()
来源：http://zxs.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://iys.zhoulong.xyz

Ruby: s.lines
来源：http://wwg.yj20258888.top

C#:   s.Split('\n')
来源：http://fpz.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://fbu.tian-w.cn

Py:   if not s:
来源：http://tuq.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://odq.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bmw.pycfn.com

TS:   if (s === "") {}
来源：http://ckj.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://knn.svipenyu.cn

Go:   if s == "" {}
来源：http://unw.hysaishi.cn

Ruby: if s.empty?
来源：http://tcz.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wii.iojbl.cn

[E21] 超长截断加省略号
来源：http://fte.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jhe.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kbn.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qzn.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qfl.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jlz.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://vzy.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://udk.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ldh.316326.xyz

[E22] 字节长度与字符长度
来源：http://zos.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hce.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opq.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhv.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywo.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ehf.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ace.yfazqb.com

Ruby: s.bytesize;  s.length
来源：http://bcj.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://css.jinghuilouyu.cn

================================================================================
来源：http://zjs.xinyue.icu

F. 文件与目录
来源：http://knk.vqdsnc.cn

================================================================================
来源：http://ulu.havefunace.top

[F01] 读取整个文件
来源：http://aow.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hkk.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://jip.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hxx.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ujf.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yww.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mbl.ybcxt.top

Ruby: File.read("a.txt")
来源：http://lcq.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://rte.ydzc1.top

[F02] 逐行读取文件
来源：http://khs.yj20258.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ibf.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rtn.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nik.52xcode.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cbf.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dna.aizwys.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knm.birdmap.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://prm.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jnv.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://xme.yonumen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lky.ydjk.org.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mgx.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lht.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vcy.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hfz.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pjm.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://enu.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awe.xuanzx.com

[F04] 追加写入文件
来源：http://zqt.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lhd.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lse.xylfe.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kep.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://plh.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://amp.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qdx.meibo888.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gta.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://quk.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://irc.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kea.hywenlv.cn

PHP:  file_exists("a.txt");
来源：http://qef.ctjpmb.com

JS:   fs.existsSync("a.txt")
来源：http://ban.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://orb.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ryh.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qbo.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://fky.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://tms.kuanghao11.cn

[F06] 删除文件
来源：http://uor.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://pgl.mhx1999.top

PHP:  unlink("a.txt");
来源：http://veh.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://qfi.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://hyk.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dva.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://sja.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://ecr.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://dvc.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://ubt.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://goe.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://flj.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tok.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nar.shangyingyoupin.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zkq.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eam.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hio.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vjm.yongpay.top

[F08] 遍历目录
来源：http://urx.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kvx.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nsw.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://kmj.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://zit.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpf.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vyj.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://tbz.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://jlc.dianchejie.cn

[F09] 获取文件大小
来源：http://fbu.hfpthk.cn

Py:   os.path.getsize("a.txt")
来源：http://mpr.smart0.xyz

PHP:  filesize("a.txt");
来源：http://omi.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://rqi.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://uje.zhijiandao.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mtw.zhiwuduotai.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://noi.ehwqpu.com

Ruby: File.size("a.txt")
来源：http://yqg.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://ezu.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://cjz.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kgs.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://znr.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ovx.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://fsi.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://euw.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://krh.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mlx.pengpengdd.cyou

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hem.daxiang520.top

[F11] 复制与移动文件
来源：http://xsx.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://myg.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nut.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvi.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xdh.sufxvd.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://thb.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://efo.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pkw.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://owz.gogol.net.cn

[F12] CSV 读写
来源：http://izg.shzxlz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://swq.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tnu.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mzo.cashguo.top

TS:   // 同上
来源：http://pvr.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kpe.fengsongda.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sal.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nsu.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://btd.hnxiangtu.top

================================================================================
来源：http://ocf.52xcode.cn

G. 面向对象
来源：http://bxf.uphjek.com

================================================================================
来源：http://kiw.tarul.cn

[G01] 定义类
来源：http://wlo.0kj1m.cn

Py:   class User: pass
来源：http://arx.xuetiantiany.cn

PHP:  class User {}
来源：http://mvc.ppjwa.cn

JS:   class User {}
来源：http://who.yj202588.top

TS:   class User { name: string = ""; }
来源：http://vtu.hcnkem.com

Java: class User {}
来源：http://mps.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://syv.vqdsnc.cn

Ruby: class User; end
来源：http://osq.9152youxi.cn

C#:   class User {}
来源：http://cvq.daxiang520.top

[G02] 构造函数
来源：http://fty.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://moy.aizwys.cn

PHP:  public function __construct(public string $name) {}
来源：http://hzt.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://uen.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://zhk.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://ner.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jvd.iojbl.cn

Ruby: def initialize(name); @name = name; end
来源：http://irk.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://nsm.yj20258.top

[G03] 实例属性
来源：http://jzr.xuanzx.com

Py:   self.name = "x"
来源：http://swm.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://qyz.jinqigfzy.top

JS:   this.name = "x";
来源：http://cka.hywenlv.cn

TS:   name: string = "x";
来源：http://krp.epnwcf.com

Java: private String name;
来源：http://mnu.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://feq.jlsjyb.cn

Ruby: @name = "x"
来源：http://iir.chenlongwang.top

C#:   public string Name { get; set; } = "x";
来源：http://yhs.yueranfly.top

[G04] 定义方法
来源：http://qxh.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://bko.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ptu.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://lme.feifeiyinyue.top

TS:   greet(): string { return this.name; }
来源：http://pib.zhoulong.xyz

Java: String greet() { return name; }
来源：http://sxj.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://avl.xuetiantiany.cn

Ruby: def greet; @name; end
来源：http://lcx.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://ciz.cdnleiting.top

[G05] 继承
来源：http://kkz.meibo888.top

Py:   class Admin(User): pass
来源：http://oqe.yuxming.cn

PHP:  class Admin extends User {}
来源：http://rzu.52xcode.cn

JS:   class Admin extends User {}
来源：http://pps.havefunace.top

TS:   class Admin extends User {}
来源：http://yvs.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://tfn.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://srs.fanxiaobao.xyz

Ruby: class Admin < User; end
来源：http://gdt.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://rik.zhixingplan.top

[G06] 重写方法
来源：http://uii.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://slq.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gdb.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://zqu.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://pbu.bjfxy.top

Java: @Override String greet() { return "admin"; }
来源：http://vph.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kgs.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://jyn.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://vus.quarkkingdee.top

[G07] 调用父类方法
来源：http://rhw.tanke756.top

Py:   super().greet()
来源：http://nji.jiagoushi.top

PHP:  parent::greet();
来源：http://ybz.yangfankeji.com

JS:   super.greet();
来源：http://qxk.snrcjt.cn

TS:   super.greet();
来源：http://ste.uphjek.com

Java: super.greet();
来源：http://ghd.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hja.shangyingyoupin.top

Ruby: super
来源：http://mns.yj202588.top

C#:   base.Greet();
来源：http://pkw.ivvv.top

[G08] 静态方法与属性
来源：http://znk.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kkt.jinghuilouyu.cn

PHP:  public static function f() {}
来源：http://ldo.yuanzhike.top

JS:   static f() {}
来源：http://guo.redwolf501.top

TS:   static f(): void {}
来源：http://xvb.hcnkem.com

Java: static void f() {}
来源：http://gfo.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dea.hysaishi.cn

Ruby: def self.f; end
来源：http://jbs.jiagoushi.top

C#:   public static void F() {}
来源：http://uqt.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://gyo.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://vky.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://npy.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://foh.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://zqx.iojbl.cn

Java: interface Shape { double area(); }
来源：http://fsm.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://vbh.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qzh.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://axf.gotoacloud.top


<!-- 参考信息 -->