代发 wailian999

[E14] URL 编码与 Base64
来源：http://fhm.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://etg.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://mui.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://euz.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pzn.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://coj.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cla.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ccf.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ohz.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://aeu.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mta.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bzq.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://frx.jinghuilouyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vyu.yueranfly.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://unj.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ppf.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://txu.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fvt.yfazqb.com

[E16] 数字千分位
来源：http://iby.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://qcy.ivvv.top

PHP:  number_format(1234567);
来源：http://ebt.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nkq.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dpf.sweek.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jvo.9152youxi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vwe.yongpay.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wub.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://fip.cdnleiting.top

[E17] 首字母大写
来源：http://hkt.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vwt.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oxt.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tkc.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xfi.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oue.shanyushiyangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wna.hongshengwenyu.top

Ruby: s.capitalize
来源：http://gzj.sysykeji.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nra.andypj.xyz

[E18] 模板占位符替换
来源：http://ggu.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fjq.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cno.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ngz.xylfe.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jze.zycfv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hrj.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qde.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://olr.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hbh.xinyue.icu

[E19] 多行文本按行拆分
来源：http://omy.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://jnj.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cnk.tian-w.cn

JS:   s.split(/\r?\n/)
来源：http://heu.nanxuanxn.top

TS:   s.split(/\r?\n/)
来源：http://dgj.fktsv.cn

Java: s.lines().toList()
来源：http://mst.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://uwq.haohaochexian.top

Ruby: s.lines
来源：http://jcj.fehbvm.com

C#:   s.Split('\n')
来源：http://yff.yj20258.top

[E20] 判断字符串是否为空
来源：http://zxu.tarul.cn

Py:   if not s:
来源：http://eaa.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pnx.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://abn.epnwcf.com

TS:   if (s === "") {}
来源：http://yjp.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://ivf.hywenlv.cn

Go:   if s == "" {}
来源：http://wsv.wangshuangyany.cn

Ruby: if s.empty?
来源：http://nuk.hongshengwenyu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ucp.fehbvm.com

[E21] 超长截断加省略号
来源：http://spo.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://apy.shangyingyoupin.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nao.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jua.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ckm.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bxx.hysaishi.cn

Go:   // 按 rune 判断长度后截断
来源：http://luh.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://obq.haohaochexian.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://syn.yongpay.top

[E22] 字节长度与字符长度
来源：http://szq.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lez.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://snc.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aaq.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://leo.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nlv.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhb.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://aar.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mkj.dashuyun.cn

================================================================================
来源：http://ieo.yvedp.cn

F. 文件与目录
来源：http://hhs.shanyushiyangtech.top

================================================================================
来源：http://msc.hfpthk.cn

[F01] 读取整个文件
来源：http://omy.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hgg.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://rjs.fzhhl.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aed.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pai.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vqq.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pjc.havefunace.top

Ruby: File.read("a.txt")
来源：http://bzl.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://aqo.fktsv.cn

[F02] 逐行读取文件
来源：http://guv.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zxt.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fmf.uphjek.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avh.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gjo.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ral.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fsi.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wvx.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vsb.xziqi.cn

[F03] 写入文件（覆盖）
来源：http://nue.hongshengwenyu.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pxd.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://grm.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ofo.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjt.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://djk.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hbf.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://utj.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://prv.zhiwuduotai.top

[F04] 追加写入文件
来源：http://mvb.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eng.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dsk.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dcp.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dqc.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iys.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fvo.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xco.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pye.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://itj.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://okx.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://wij.iojbl.cn

JS:   fs.existsSync("a.txt")
来源：http://hku.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://fej.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tsh.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://evn.ybcxt.top

Ruby: File.exist?("a.txt")
来源：http://xxf.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://cmm.jlsjyb.cn

[F06] 删除文件
来源：http://snw.jiagoushi.top

Py:   os.remove("a.txt")
来源：http://ghj.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://cqz.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wad.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://kar.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jdl.yonumen.top

Go:   os.Remove("a.txt")
来源：http://vqp.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://xmk.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://rgp.52xcode.cn

[F07] 创建目录（含多级）
来源：http://abb.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qms.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pyw.pycfn.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lcm.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jug.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vxr.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oge.xuetiantiany.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lum.xuetiantiany.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://shk.aizwys.cn

[F08] 遍历目录
来源：http://umj.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hja.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sdo.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://fbz.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://efs.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qyf.zdqjudy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bgc.wangdashe.top

Ruby: Dir.children("dir")
来源：http://jdt.zhongyouzk.top

C#:   Directory.GetFiles("dir")
来源：http://mjw.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://vsq.jqgfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ihi.havefunace.top

PHP:  filesize("a.txt");
来源：http://qbn.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://doi.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://sxk.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://fmx.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qlc.fktsv.cn

Ruby: File.size("a.txt")
来源：http://zrh.fzhhl.top

C#:   new FileInfo("a.txt").Length
来源：http://rlq.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://tpm.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://orz.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hah.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rgs.fehbvm.com

TS:   path.extname("a.txt")
来源：http://nyo.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ssy.yangfankeji.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://toj.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dnf.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zmc.bjfxy.top

[F11] 复制与移动文件
来源：http://xjj.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aod.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vep.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilo.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eax.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mhg.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ugr.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yht.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ezn.c1oappe.top

[F12] CSV 读写
来源：http://cxh.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bhr.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ujn.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://duy.yuxming.cn

TS:   // 同上
来源：http://zws.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tcw.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qlg.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://noj.yonumen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ydv.daxiang520.top

================================================================================
来源：http://stw.c1oappe.top

G. 面向对象
来源：http://zzk.shanyushiyangkeji.top

================================================================================
来源：http://wcw.svipenyu.cn

[G01] 定义类
来源：http://nqa.chenzaomai.com

Py:   class User: pass
来源：http://ght.daxiang520.top

PHP:  class User {}
来源：http://mym.jinghuilouyu.cn

JS:   class User {}
来源：http://yox.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://ecc.mhx1999.top

Java: class User {}
来源：http://qrc.ctjpmb.com

Go:   type User struct { Name string }
来源：http://hxn.daria6918.cn

Ruby: class User; end
来源：http://uso.zhoulong.xyz

C#:   class User {}
来源：http://pyw.c1oappe.top

[G02] 构造函数
来源：http://hje.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://bwf.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://zit.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://and.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://fus.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://hml.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nzp.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://pkf.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://kvg.redwolf501.top

[G03] 实例属性
来源：http://eyd.hammf.cn

Py:   self.name = "x"
来源：http://vqn.fehbvm.com

PHP:  public string $name = "x";
来源：http://uex.fehbvm.com

JS:   this.name = "x";
来源：http://dir.yonumen.top

TS:   name: string = "x";
来源：http://ido.xuetiantiany.cn

Java: private String name;
来源：http://dsm.shuidangran.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hmz.aizwys.cn

Ruby: @name = "x"
来源：http://fmb.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://qxo.xuanzx.com

[G04] 定义方法
来源：http://qyk.fktsv.cn

Py:   def greet(self): return self.name
来源：http://eva.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://icc.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://ktt.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://nfc.jqgufenzy.top

Java: String greet() { return name; }
来源：http://uqi.fanxiaobao.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://erq.cheryme.top

Ruby: def greet; @name; end
来源：http://aam.tanke756.top

C#:   public string Greet() => Name;
来源：http://ahg.hysaishi.cn

[G05] 继承
来源：http://cgg.zdbjq.cn

Py:   class Admin(User): pass
来源：http://guf.tanke756.top

PHP:  class Admin extends User {}
来源：http://mpz.jiagoushi.top

JS:   class Admin extends User {}
来源：http://sld.uphjek.com

TS:   class Admin extends User {}
来源：http://hyi.fzhhl.top

Java: class Admin extends User {}
来源：http://xwf.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mmt.smart0.xyz

Ruby: class Admin < User; end
来源：http://llx.xylfe.cn

C#:   class Admin : User {}
来源：http://fsp.52xcode.cn

[G06] 重写方法
来源：http://fox.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://zgr.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oja.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://byx.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://lgk.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://ltt.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ekc.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://tno.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://gjs.andypj.xyz

[G07] 调用父类方法
来源：http://yag.52xcode.cn

Py:   super().greet()
来源：http://for.zhiwuduotai.top

PHP:  parent::greet();
来源：http://fdr.chenlongwang.top

JS:   super.greet();
来源：http://ivu.zhiwuduotai.top

TS:   super.greet();
来源：http://ols.zhixingplan.top

Java: super.greet();
来源：http://ffx.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://npq.ydjk.org.cn

Ruby: super
来源：http://put.bbcook.cn

C#:   base.Greet();
来源：http://fzh.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://tcs.hcnkem.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sxa.vqdsnc.cn

PHP:  public static function f() {}
来源：http://oem.dashuyun.cn

JS:   static f() {}
来源：http://nmt.hongshengwenyu.top

TS:   static f(): void {}
来源：http://cgg.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://xxq.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jyv.tian-w.cn

Ruby: def self.f; end
来源：http://pzu.yueranfly.top

C#:   public static void F() {}
来源：http://tsr.yonumen.top

[G09] 接口 / 抽象类
来源：http://uqd.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://faa.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://qoh.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jxl.xuetiantiany.cn

TS:   interface Shape { area(): number; }
来源：http://ctm.xuanzx.com

Java: interface Shape { double area(); }
来源：http://ieh.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://klj.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ggp.gaohongyu789.top

C#:   interface IShape { double Area(); }
来源：http://uqy.ppjwa.cn

[G10] 访问控制
来源：http://dsf.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://irf.xuetiantiany.cn

PHP:  public / protected / private
来源：http://xjn.fzhhl.top

JS:   #private 字段；其余公开
来源：http://ypb.iojbl.cn

TS:   public / protected / private
来源：http://iec.zhijiandao.cn

Java: public / protected / private / 默认包级
来源：http://mbz.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lsd.gogol.net.cn

Ruby: public / protected / private
来源：http://hzg.cucudq.cn

C#:   public / protected / private / internal
来源：http://xww.zycfv.cn

[G11] getter / setter
来源：http://vxm.smart0.xyz

Py:   @property 与 @x.setter
来源：http://erl.9152youxi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rmu.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://hfg.wangshuangyany.cn

TS:   get name(): string { return this._name; }
来源：http://isr.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://eya.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://esc.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://xtb.xuanzx.com

C#:   public string Name { get; set; }
来源：http://ylw.9152youxi.cn

[G12] 对象转字符串
来源：http://oyo.sysykeji.top

Py:   def __str__(self): return self.name
来源：http://yxt.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://qcd.uphjek.com

JS:   toString() { return this.name; }
来源：http://bfy.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://sqz.fehbvm.com

Java: @Override public String toString() { return name; }
来源：http://hzu.fehbvm.com


<!-- 参考信息 -->