代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zng.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://ifq.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jxu.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nay.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://osl.andypj.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://zwn.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dza.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cyj.shangyingyoupin.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dll.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yxm.yangfankeji.com

[E16] 数字千分位
来源：http://dxk.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://sdl.gogol.net.cn

PHP:  number_format(1234567);
来源：http://xis.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://smr.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bwx.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vsh.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ssd.hcnkem.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tsp.cashguo.top

C#:   1234567.ToString("N0")
来源：http://rvp.hongshengwenyu.top

[E17] 首字母大写
来源：http://suf.birdmap.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zxi.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tsw.guowangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yjz.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://acf.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pcf.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cfn.fktsv.cn

Ruby: s.capitalize
来源：http://qdm.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ipy.fanxiaobao.xyz

[E18] 模板占位符替换
来源：http://kqz.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://usn.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lmm.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dsn.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://afx.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dzf.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://whu.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gjz.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oyn.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://myl.iojbl.cn

Py:   s.splitlines()
来源：http://bks.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zax.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://emf.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://zhr.cdnleiting.top

Java: s.lines().toList()
来源：http://vzr.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://oew.hysaishi.cn

Ruby: s.lines
来源：http://qzo.dianchejie.cn

C#:   s.Split('\n')
来源：http://irb.cashguo.top

[E20] 判断字符串是否为空
来源：http://dma.havefunace.top

Py:   if not s:
来源：http://ssl.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cdz.ctjpmb.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uzf.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://lqu.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://pxw.xingfuxueyuan.xyz

Go:   if s == "" {}
来源：http://uzr.316326.xyz

Ruby: if s.empty?
来源：http://rra.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tbu.sysykeji.top

[E21] 超长截断加省略号
来源：http://ysp.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iti.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pkw.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vom.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vzu.jqgfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://weo.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://mwv.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ddf.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kgn.yongpay.top

[E22] 字节长度与字符长度
来源：http://sem.dianchejie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gmg.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vdx.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gre.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://txk.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wjk.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qlo.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://nbi.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqv.guowangkeji.top

================================================================================
来源：http://vxq.fzhhl.top

F. 文件与目录
来源：http://qnq.sysykeji.top

================================================================================
来源：http://hvj.jqgufenzy.top

[F01] 读取整个文件
来源：http://jwm.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://htc.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://idl.zhengqikj.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rng.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://urk.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://pox.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://shu.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://byu.tarul.cn

C#:   File.ReadAllText("a.txt");
来源：http://can.zhongyouzk.top

[F02] 逐行读取文件
来源：http://keu.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bhj.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cfv.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nwe.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffa.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hfz.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ext.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ygu.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pok.xuanzx.com

[F03] 写入文件（覆盖）
来源：http://qyi.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ojs.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://exf.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sny.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yol.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbz.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://czu.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://gjx.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uzb.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://gyy.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xri.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://evt.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cfa.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://msb.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hsb.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kdf.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://opn.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uyy.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://pyg.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nep.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://ler.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://duo.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://bfo.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://odk.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dzz.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://raz.cashguo.top

C#:   File.Exists("a.txt")
来源：http://qel.ctjpmb.com

[F06] 删除文件
来源：http://jwr.zhiwuduotai.top

Py:   os.remove("a.txt")
来源：http://zja.yongpay.top

PHP:  unlink("a.txt");
来源：http://jkj.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://hzy.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ydl.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tbh.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://erj.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://njc.hammf.cn

C#:   File.Delete("a.txt");
来源：http://sph.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://hfp.nwbrower.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ujj.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://npc.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cgb.guannengcc.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mnv.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://now.guowangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mui.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tcw.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tcv.jianghu66.top

[F08] 遍历目录
来源：http://qkz.guannengcc.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iho.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://elq.hfpthk.cn

JS:   fs.readdirSync("dir")
来源：http://svi.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://dmb.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://txq.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wex.hfpthk.cn

Ruby: Dir.children("dir")
来源：http://moz.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://ytd.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://jkj.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://gel.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://wvo.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://iwx.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://gck.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://rkw.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fiw.yfazqb.com

Ruby: File.size("a.txt")
来源：http://zcu.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://jvi.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://eit.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rig.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gzu.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nfz.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://yyd.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://riv.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pyd.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bqz.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zpd.ctjpmb.com

[F11] 复制与移动文件
来源：http://rcq.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lwm.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hsn.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pal.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohi.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tdx.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vto.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pme.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yrs.tianlin.xyz

[F12] CSV 读写
来源：http://vtp.tarul.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emf.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yph.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uuz.gotoacloud.top

TS:   // 同上
来源：http://ljh.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yge.snrcjt.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qwq.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kho.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qaf.dashuyun.cn

================================================================================
来源：http://zqn.snrcjt.cn

G. 面向对象
来源：http://tnz.zdqjudy.top

================================================================================
来源：http://lby.hysaishi.cn

[G01] 定义类
来源：http://bxa.ydzc1.top

Py:   class User: pass
来源：http://zqi.haohaochexian.top

PHP:  class User {}
来源：http://dph.andypj.xyz

JS:   class User {}
来源：http://zgv.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://aav.zhaomingkeji.xyz

Java: class User {}
来源：http://spd.jianghu66.top

Go:   type User struct { Name string }
来源：http://fhe.jyoumei.cn

Ruby: class User; end
来源：http://yzs.smart0.xyz

C#:   class User {}
来源：http://gzl.ybcxt.top

[G02] 构造函数
来源：http://tsd.hammf.cn

Py:   def __init__(self, name): self.name = name
来源：http://hrz.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://wib.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://nhe.ivvv.top

TS:   constructor(public name: string) {}
来源：http://gip.jlsjyb.cn

Java: User(String name) { this.name = name; }
来源：http://iig.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cah.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://met.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://yfo.yueranfly.top

[G03] 实例属性
来源：http://upc.daxiang520.top

Py:   self.name = "x"
来源：http://ngr.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://bmm.ydjk.org.cn

JS:   this.name = "x";
来源：http://uvc.daxiang520.top

TS:   name: string = "x";
来源：http://uqr.xuanzx.com

Java: private String name;
来源：http://ltp.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wsi.jiagoushi.top

Ruby: @name = "x"
来源：http://rwk.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://xuj.zycfv.cn

[G04] 定义方法
来源：http://tdg.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://xwy.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aop.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://mbq.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://gnm.gaohongyu789.top

Java: String greet() { return name; }
来源：http://okk.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mqg.wangdashe.top

Ruby: def greet; @name; end
来源：http://vvw.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://gjx.yuanzhike.top

[G05] 继承
来源：http://bod.yonumen.top

Py:   class Admin(User): pass
来源：http://wqz.cashguo.top

PHP:  class Admin extends User {}
来源：http://yll.uphjek.com

JS:   class Admin extends User {}
来源：http://cml.aibaodan.cn

TS:   class Admin extends User {}
来源：http://dpe.aibaodan.cn

Java: class Admin extends User {}
来源：http://wne.shangyingyoupin.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cqr.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://yvg.xinyue.icu

C#:   class Admin : User {}
来源：http://xgj.cheryme.top

[G06] 重写方法
来源：http://atv.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://ycq.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tuo.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://rbm.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://tae.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://wbp.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mwq.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://mfw.xuetiantiany.cn

C#:   public override string Greet() => "admin";
来源：http://kqh.andypj.xyz

[G07] 调用父类方法
来源：http://kou.wangdashe.top

Py:   super().greet()
来源：http://eoh.sysykeji.top

PHP:  parent::greet();
来源：http://mdx.fanxiaobao.xyz

JS:   super.greet();
来源：http://yto.bbcook.cn

TS:   super.greet();
来源：http://lxi.xziqi.cn

Java: super.greet();
来源：http://tuf.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://whq.fanxiaobao.xyz

Ruby: super
来源：http://eox.yuanzhike.top

C#:   base.Greet();
来源：http://olj.yuanzhike.top

[G08] 静态方法与属性
来源：http://lzg.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ete.fengsongda.top

PHP:  public static function f() {}
来源：http://ltq.dashuyun.cn

JS:   static f() {}
来源：http://thf.gotoacloud.top

TS:   static f(): void {}
来源：http://dfk.wangdashe.top

Java: static void f() {}
来源：http://dwr.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qwu.shzxlz.cn

Ruby: def self.f; end
来源：http://yok.gogol.net.cn

C#:   public static void F() {}
来源：http://dyk.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://ylw.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://aov.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://jau.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wqw.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://bpk.aizwys.cn

Java: interface Shape { double area(); }
来源：http://kok.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://arf.jinqigfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ijl.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://xkb.tian-w.cn

[G10] 访问控制
来源：http://glg.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://nqp.andypj.xyz

PHP:  public / protected / private
来源：http://hyt.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://dat.sxryk.cn

TS:   public / protected / private
来源：http://qkx.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://cpv.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://edr.svipenyu.cn

Ruby: public / protected / private
来源：http://edb.xuanzx.com

C#:   public / protected / private / internal
来源：http://udy.yonumen.top

[G11] getter / setter
来源：http://hzt.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://lys.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://bpz.daxiang520.top

JS:   get name() { return this._name; }
来源：http://vpt.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://otz.yonumen.top

Java: public String getName() { return name; }
来源：http://cnn.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hcn.sufxvd.cn

Ruby: attr_accessor :name
来源：http://ety.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://vgr.mhx1999.top

[G12] 对象转字符串
来源：http://xyn.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://eiq.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ypm.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://xey.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://uzy.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://dts.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://guc.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://fgy.snrcjt.cn

C#:   public override string ToString() => Name;
来源：http://aoy.sjlbkw.cn

[G13] 判断对象类型
来源：http://wsl.bbcook.cn

Py:   isinstance(u, User)
来源：http://irv.smart0.xyz

PHP:  $u instanceof User
来源：http://zpk.pycfn.com

JS:   u instanceof User
来源：http://jro.xylfe.cn

TS:   u instanceof User
来源：http://whd.zhiwuduotai.top


<!-- 参考信息 -->