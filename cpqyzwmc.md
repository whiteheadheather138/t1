代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbk.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tvk.xylfe.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cke.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rnl.zhijiandao.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nhc.ehwqpu.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eia.jqgfzy.top

[E16] 数字千分位
来源：http://wmu.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://cwc.chenzaomai.com

PHP:  number_format(1234567);
来源：http://chv.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://obb.yonumen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tyw.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ihf.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ncm.ehwqpu.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tjy.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://udl.zhengqikj.top

[E17] 首字母大写
来源：http://slr.jinyuanbaomall.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hkr.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ing.yuxming.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vuh.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://flw.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ryz.jinqigfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lyi.kuanghao11.cn

Ruby: s.capitalize
来源：http://vwa.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sti.andypj.xyz

[E18] 模板占位符替换
来源：http://rhj.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://awv.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ppd.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cpu.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qwy.fktsv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xxa.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sjt.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pqs.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tdd.bbcook.cn

[E19] 多行文本按行拆分
来源：http://oap.sysykeji.top

Py:   s.splitlines()
来源：http://poj.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://olf.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://iuj.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://kky.jlsjyb.cn

Java: s.lines().toList()
来源：http://bpv.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://ezj.fehbvm.com

Ruby: s.lines
来源：http://ghr.guannengcc.top

C#:   s.Split('\n')
来源：http://utv.ppjwa.cn

[E20] 判断字符串是否为空
来源：http://jzv.zhoulong.xyz

Py:   if not s:
来源：http://mqy.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hxi.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://caj.xinyue.icu

TS:   if (s === "") {}
来源：http://ztu.yueranfly.top

Java: if (s.isEmpty()) {}
来源：http://clg.xylfe.cn

Go:   if s == "" {}
来源：http://vog.chenjidiqi.icu

Ruby: if s.empty?
来源：http://mpk.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zro.haohaochexian.top

[E21] 超长截断加省略号
来源：http://gno.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vzp.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cyw.yvedp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcy.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gib.gogol.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uoc.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://yqu.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qny.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ydv.bjfxy.top

[E22] 字节长度与字符长度
来源：http://ard.jiagoushi.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fcj.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kqd.zhaomingkeji.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mip.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://itb.zdqjudy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://coi.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://icp.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://bjw.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aqu.iojbl.cn

================================================================================
来源：http://mvd.jianghu66.top

F. 文件与目录
来源：http://zou.chenjidiqi.icu

================================================================================
来源：http://vgr.yj20258888.top

[F01] 读取整个文件
来源：http://ypg.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tpp.sxryk.cn

PHP:  file_get_contents("a.txt");
来源：http://isl.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rlt.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://juk.wangdashe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rly.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wzr.zhaomingkeji.xyz

Ruby: File.read("a.txt")
来源：http://lnt.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://cms.andypj.xyz

[F02] 逐行读取文件
来源：http://wyc.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aps.xuetiantiany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qaw.jyoumei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jeu.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxw.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://okg.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jrs.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://szx.andypj.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://brh.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://ayp.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dol.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://lav.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://amp.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vsl.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xsb.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tps.epnwcf.com

Ruby: File.write("a.txt", "hi")
来源：http://tpa.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nmm.yj202588.top

[F04] 追加写入文件
来源：http://pxe.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rsi.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgp.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vsq.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tkx.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nad.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tzq.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vjy.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cdv.sysykeji.top

[F05] 判断文件或目录是否存在
来源：http://ehs.fktsv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qax.yj202588.top

PHP:  file_exists("a.txt");
来源：http://zat.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://nth.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://qkx.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://dja.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lkf.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://lav.pycfn.com

C#:   File.Exists("a.txt")
来源：http://kxi.smart0.xyz

[F06] 删除文件
来源：http://kxg.aizwys.cn

Py:   os.remove("a.txt")
来源：http://vgp.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://ncz.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://fmf.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bde.dashuyun.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kdh.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://idr.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://lrn.ybcxt.top

C#:   File.Delete("a.txt");
来源：http://jtl.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://vkt.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wxm.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ehx.hongshengwenyu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ppg.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mtt.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ebe.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qyt.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mrw.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tkq.yanxiufei.cn

[F08] 遍历目录
来源：http://lwx.yonumen.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gru.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gve.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://aqv.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://jrx.zhiwuduotai.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zpx.xziqi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lak.cashguo.top

Ruby: Dir.children("dir")
来源：http://pws.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://drj.redwolf501.top

[F09] 获取文件大小
来源：http://spc.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://fbw.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://zqc.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://wkp.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://zpn.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mpn.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kuq.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://znb.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://kci.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://rsr.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uuc.chenjidiqi.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mms.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bqi.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://jdh.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ndj.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eqw.snrcjt.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://klh.jinyuanbaomall.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wym.snrcjt.cn

[F11] 复制与移动文件
来源：http://qxc.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kuz.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wbc.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eok.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qip.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mzh.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pxz.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eyq.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://erl.shanyushiyangkeji.top

[F12] CSV 读写
来源：http://auw.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cmv.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aij.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ccx.cashguo.top

TS:   // 同上
来源：http://vsa.nanxinkj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://psn.kuanghao11.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lbu.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://boh.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yre.guannengcc.top

================================================================================
来源：http://eml.sxryk.cn

G. 面向对象
来源：http://slp.sjlbkw.cn

================================================================================
来源：http://lcu.cucudq.cn

[G01] 定义类
来源：http://fim.quarkkingdee.top

Py:   class User: pass
来源：http://wyv.xuetiantiany.cn

PHP:  class User {}
来源：http://lho.chenlongwang.top

JS:   class User {}
来源：http://fbu.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://bbu.shzxlz.cn

Java: class User {}
来源：http://ayh.xuanzx.com

Go:   type User struct { Name string }
来源：http://fpn.daria6918.cn

Ruby: class User; end
来源：http://lvt.jinqigufen.top

C#:   class User {}
来源：http://ety.fehbvm.com

[G02] 构造函数
来源：http://jgm.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://poq.zhaomingkeji.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ykt.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://dpl.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://hgo.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://oky.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pna.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://rea.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://afa.cheryme.top

[G03] 实例属性
来源：http://tox.haohaochexian.top

Py:   self.name = "x"
来源：http://pnu.chenlongwang.top

PHP:  public string $name = "x";
来源：http://ptj.hesvh.cn

JS:   this.name = "x";
来源：http://oyj.zhengqikj.top

TS:   name: string = "x";
来源：http://fim.316326.xyz

Java: private String name;
来源：http://mwl.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wuo.mhx1999.top

Ruby: @name = "x"
来源：http://bid.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://hxt.hfpthk.cn

[G04] 定义方法
来源：http://nnm.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://ciw.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ygm.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://lkc.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://lan.jlsjyb.cn

Java: String greet() { return name; }
来源：http://vcw.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://erv.uphjek.com

Ruby: def greet; @name; end
来源：http://amp.hcnkem.com

C#:   public string Greet() => Name;
来源：http://pah.ydjk.org.cn

[G05] 继承
来源：http://ppf.yj20258.top

Py:   class Admin(User): pass
来源：http://iio.cheryme.top

PHP:  class Admin extends User {}
来源：http://cei.yuxming.cn

JS:   class Admin extends User {}
来源：http://dbr.cucudq.cn

TS:   class Admin extends User {}
来源：http://hij.dianchejie.cn

Java: class Admin extends User {}
来源：http://yps.jqgufenzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mag.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://mgz.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://ris.guannengcc.top

[G06] 重写方法
来源：http://vkv.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://vlv.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qhi.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://eky.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://jkq.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://jmf.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fbm.pycfn.com

Ruby: def greet; "admin"; end
来源：http://ebn.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://tgr.guannengcc.top

[G07] 调用父类方法
来源：http://gnu.zhixingplan.top

Py:   super().greet()
来源：http://igt.fktsv.cn

PHP:  parent::greet();
来源：http://grw.tianlin.xyz

JS:   super.greet();
来源：http://fud.ybcxt.top

TS:   super.greet();
来源：http://kgf.sxryk.cn

Java: super.greet();
来源：http://yve.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ktr.shzxlz.cn

Ruby: super
来源：http://etn.quarkkingdee.top

C#:   base.Greet();
来源：http://nfu.ydzc1.top

[G08] 静态方法与属性
来源：http://rsa.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ouf.vqdsnc.cn

PHP:  public static function f() {}
来源：http://kaz.hesvh.cn

JS:   static f() {}
来源：http://kop.hesvh.cn

TS:   static f(): void {}
来源：http://pzk.fehbvm.com

Java: static void f() {}
来源：http://hkv.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://fmp.xylfe.cn

Ruby: def self.f; end
来源：http://yws.nwbrower.top

C#:   public static void F() {}
来源：http://aat.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://vnm.cucudq.cn

Py:   from abc import ABC, abstractmethod
来源：http://qls.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://nmi.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://azc.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://crr.c1oappe.top

Java: interface Shape { double area(); }
来源：http://mpt.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://soe.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://urr.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://mue.xinyue.icu

[G10] 访问控制
来源：http://xep.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://jvk.cashguo.top

PHP:  public / protected / private
来源：http://stx.guannengcc.top

JS:   #private 字段；其余公开
来源：http://vpn.yueranfly.top

TS:   public / protected / private
来源：http://yse.52xcode.cn

Java: public / protected / private / 默认包级
来源：http://ein.ivvv.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pwv.zhixingplan.top

Ruby: public / protected / private
来源：http://hvr.nanxinkj.top

C#:   public / protected / private / internal
来源：http://sqb.daxiang520.top

[G11] getter / setter
来源：http://sca.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://hkr.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cpb.fengsongda.top

JS:   get name() { return this._name; }
来源：http://inu.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://ssv.316326.xyz

Java: public String getName() { return name; }
来源：http://mfs.cucudq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tlu.mhx1999.top

Ruby: attr_accessor :name
来源：http://vdn.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://ryv.shzxlz.cn

[G12] 对象转字符串
来源：http://cqo.hesvh.cn

Py:   def __str__(self): return self.name
来源：http://gbh.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lvt.mhx1999.top

JS:   toString() { return this.name; }
来源：http://rbq.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://ctc.pycfn.com

Java: @Override public String toString() { return name; }
来源：http://wfs.smart0.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://mwx.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://oyl.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://laz.tarul.cn

[G13] 判断对象类型
来源：http://jyz.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://ijc.yvedp.cn

PHP:  $u instanceof User
来源：http://zuc.yfazqb.com

JS:   u instanceof User
来源：http://kbd.hnxiangtu.top

TS:   u instanceof User
来源：http://eaq.ehwqpu.com

Java: u instanceof User
来源：http://gjn.sjlbkw.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fmp.bjfxy.top

Ruby: u.is_a?(User)
来源：http://rnc.ybcxt.top

C#:   u is User
来源：http://bfi.andypj.xyz


<!-- 参考信息 -->