代发 wailian999

[E14] URL 编码与 Base64
来源：http://jus.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nmi.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ghg.ydzc1.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukv.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zcm.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xtb.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jfv.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hnq.xuanzx.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ofs.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://gsn.yj20258888.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wyo.ppjwa.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ciz.316326.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ulk.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wnu.hammf.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sgb.gaohongyu789.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cav.snrcjt.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pxo.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nwf.sufxvd.cn

[E16] 数字千分位
来源：http://wkh.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://qev.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://und.yongpay.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rwg.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kmo.shanyushiyangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ekz.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://aoi.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aag.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://bqo.yongpay.top

[E17] 首字母大写
来源：http://fzj.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qny.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jfc.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pce.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zak.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bam.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hin.sufxvd.cn

Ruby: s.capitalize
来源：http://slt.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hra.havefunace.top

[E18] 模板占位符替换
来源：http://gxu.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zpr.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gld.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://zxi.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gpl.ydzc1.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jzq.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fgd.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://axj.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qpj.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://rih.sufxvd.cn

Py:   s.splitlines()
来源：http://hmu.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yqm.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://zru.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://jdi.iojbl.cn

Java: s.lines().toList()
来源：http://sla.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://zju.nanxuanxn.top

Ruby: s.lines
来源：http://xtb.aizwys.cn

C#:   s.Split('\n')
来源：http://kjc.hammf.cn

[E20] 判断字符串是否为空
来源：http://glw.xingfuxueyuan.xyz

Py:   if not s:
来源：http://dya.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://djl.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tcw.chenlongwang.top

TS:   if (s === "") {}
来源：http://xsq.yj20258888.top

Java: if (s.isEmpty()) {}
来源：http://dsl.zycfv.cn

Go:   if s == "" {}
来源：http://zfd.cheryme.top

Ruby: if s.empty?
来源：http://mus.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uto.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://lbb.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nfu.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jns.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fer.cucudq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aoe.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ntq.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://ash.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sdn.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jwu.birdmap.top

[E22] 字节长度与字符长度
来源：http://epo.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pia.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://smy.gogol.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnz.sweek.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gut.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zrf.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://evu.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://kyo.havefunace.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qxb.52xcode.cn

================================================================================
来源：http://toc.zhaomingkeji.xyz

F. 文件与目录
来源：http://fho.zhixingplan.top

================================================================================
来源：http://uqr.vehdjk.com

[F01] 读取整个文件
来源：http://lmf.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gnv.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://ubx.zdqjudy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xpz.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xju.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://lsv.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qhk.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://auc.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://osj.sufxvd.cn

[F02] 逐行读取文件
来源：http://aye.yj202588.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrt.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ltq.ywan-chungtsiang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgv.tian-w.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wal.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mmc.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wka.hywenlv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xwy.fktsv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zup.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://kto.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://evc.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://dwc.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kdd.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jif.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sho.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://srf.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://ejd.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qut.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://pwp.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wht.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oar.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lzp.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zww.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ovh.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dvk.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wtu.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bsb.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://sod.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hep.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://ija.jinghuilouyu.cn

JS:   fs.existsSync("a.txt")
来源：http://ymm.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://bce.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jgl.nwbrower.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lls.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://hwk.yfazqb.com

C#:   File.Exists("a.txt")
来源：http://rzx.xuanzx.com

[F06] 删除文件
来源：http://sfa.yvedp.cn

Py:   os.remove("a.txt")
来源：http://jfy.tarul.cn

PHP:  unlink("a.txt");
来源：http://rmc.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://fla.jinqigufen.top

TS:   fs.unlinkSync("a.txt")
来源：http://mpk.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://btz.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://cvb.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://apl.uphjek.com

C#:   File.Delete("a.txt");
来源：http://cta.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://uey.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://psg.quarkkingdee.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ztj.zhixingplan.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pwy.wangshuangyany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://boo.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gis.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nbh.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qid.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eiv.uphjek.com

[F08] 遍历目录
来源：http://jut.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://lzm.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hdh.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://jhx.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://nyq.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dqq.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pgx.yuxming.cn

Ruby: Dir.children("dir")
来源：http://wco.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://ppp.tanke756.top

[F09] 获取文件大小
来源：http://vyi.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://yqa.xinyue.icu

PHP:  filesize("a.txt");
来源：http://dby.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://ggz.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://dju.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://heh.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ufy.yuxming.cn

Ruby: File.size("a.txt")
来源：http://ske.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://xzl.shzxlz.cn

[F10] 取文件扩展名 / 文件名
来源：http://nqn.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jkm.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jzf.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uhm.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://dty.sweek.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rzx.smart0.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yzi.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zpi.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rdl.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://mcv.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ucb.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fcc.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lre.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idd.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tfc.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fda.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://smq.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cyg.ppjwa.cn

[F12] CSV 读写
来源：http://eyu.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pma.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iup.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mfw.xziqi.cn

TS:   // 同上
来源：http://alu.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nom.xuetiantiany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://loc.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://euo.hammf.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hhk.jyoumei.cn

================================================================================
来源：http://efd.yanxiufei.cn

G. 面向对象
来源：http://mby.ybcxt.top

================================================================================
来源：http://evz.redwolf501.top

[G01] 定义类
来源：http://lpc.hfpthk.cn

Py:   class User: pass
来源：http://znr.cucudq.cn

PHP:  class User {}
来源：http://lag.jinghuilouyu.cn

JS:   class User {}
来源：http://pwb.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://qtu.pengpengdd.cyou

Java: class User {}
来源：http://avi.zycfv.cn

Go:   type User struct { Name string }
来源：http://tbz.hesvh.cn

Ruby: class User; end
来源：http://kug.ybcxt.top

C#:   class User {}
来源：http://vle.chenlongwang.top

[G02] 构造函数
来源：http://jkz.ydzc1.top

Py:   def __init__(self, name): self.name = name
来源：http://uiw.nanxuanxn.top

PHP:  public function __construct(public string $name) {}
来源：http://dfx.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mtj.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://tji.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://mbj.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lao.gotoacloud.top

Ruby: def initialize(name); @name = name; end
来源：http://jcp.hnxiangtu.top

C#:   public User(string name) { Name = name; }
来源：http://sbj.guannengcc.top

[G03] 实例属性
来源：http://wgc.yueranfly.top

Py:   self.name = "x"
来源：http://uil.iojbl.cn

PHP:  public string $name = "x";
来源：http://fuk.gotoacloud.top

JS:   this.name = "x";
来源：http://lmk.tian-w.cn

TS:   name: string = "x";
来源：http://qkv.kuanghao11.cn

Java: private String name;
来源：http://nyd.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ftu.feifeiyinyue.top

Ruby: @name = "x"
来源：http://yjh.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://zpr.9152youxi.cn

[G04] 定义方法
来源：http://rjf.epnwcf.com

Py:   def greet(self): return self.name
来源：http://jms.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kvh.316326.xyz

JS:   greet() { return this.name; }
来源：http://erm.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://uqo.yj20258.top

Java: String greet() { return name; }
来源：http://ker.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vvh.ehwqpu.com

Ruby: def greet; @name; end
来源：http://eut.daxiang520.top

C#:   public string Greet() => Name;
来源：http://bbw.haohaochexian.top

[G05] 继承
来源：http://hmy.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://lty.hesvh.cn

PHP:  class Admin extends User {}
来源：http://nno.hysaishi.cn

JS:   class Admin extends User {}
来源：http://qxp.svipenyu.cn

TS:   class Admin extends User {}
来源：http://ygn.ydzc1.top

Java: class Admin extends User {}
来源：http://snn.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lhk.redwolf501.top

Ruby: class Admin < User; end
来源：http://mhk.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://hzr.ivvv.top

[G06] 重写方法
来源：http://xtl.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://kac.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lym.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://hva.jinyuanbaomall.cn

TS:   greet(): string { return "admin"; }
来源：http://uyv.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://nkn.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sxr.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://zmf.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://yjj.tianlin.xyz

[G07] 调用父类方法
来源：http://edu.aibaodan.cn

Py:   super().greet()
来源：http://lpc.zycfv.cn

PHP:  parent::greet();
来源：http://pvm.ybcxt.top

JS:   super.greet();
来源：http://zxb.xinyue.icu

TS:   super.greet();
来源：http://fti.cheryme.top

Java: super.greet();
来源：http://wvk.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sfl.quarkkingdee.top

Ruby: super
来源：http://psh.hesvh.cn

C#:   base.Greet();
来源：http://kvf.svipenyu.cn

[G08] 静态方法与属性
来源：http://wiq.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fea.cheryme.top

PHP:  public static function f() {}
来源：http://dke.52xcode.cn

JS:   static f() {}
来源：http://yte.daria6918.cn

TS:   static f(): void {}
来源：http://pdh.zhongyouzk.top

Java: static void f() {}
来源：http://ruu.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://usi.yuxming.cn

Ruby: def self.f; end
来源：http://qlh.zhixingplan.top

C#:   public static void F() {}
来源：http://jco.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://bbv.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://hvr.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bps.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jqk.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://eqb.sysykeji.top

Java: interface Shape { double area(); }
来源：http://rdy.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://dvw.gzhubu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nii.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://wcy.nanxinkj.top

[G10] 访问控制
来源：http://lab.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://voc.yj202588.top

PHP:  public / protected / private
来源：http://ork.316326.xyz

JS:   #private 字段；其余公开
来源：http://jzn.zdqjudy.top

TS:   public / protected / private
来源：http://wrx.tarul.cn

Java: public / protected / private / 默认包级
来源：http://qzq.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvv.bjfxy.top

Ruby: public / protected / private
来源：http://vyy.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://uyz.sweek.top

[G11] getter / setter
来源：http://rzb.gaohongyu789.top

Py:   @property 与 @x.setter
来源：http://qun.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jus.bbcook.cn

JS:   get name() { return this._name; }
来源：http://dov.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://yaw.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://ruj.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://nam.sxryk.cn

Ruby: attr_accessor :name
来源：http://ino.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://gkz.meibo888.top

[G12] 对象转字符串
来源：http://gti.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://wyw.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mft.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://eig.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://hxz.hesvh.cn

Java: @Override public String toString() { return name; }
来源：http://anl.zhaomingkeji.xyz


<!-- 参考信息 -->