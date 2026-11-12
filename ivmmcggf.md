代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://reo.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ydw.jyoumei.cn

[E16] 数字千分位
来源：http://fyx.wangdashe.top

Py:   f"{1234567:,}"
来源：http://prw.fzhhl.top

PHP:  number_format(1234567);
来源：http://zkm.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xwd.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fmg.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lju.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lbk.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://flz.fengsongda.top

C#:   1234567.ToString("N0")
来源：http://ims.hywenlv.cn

[E17] 首字母大写
来源：http://nhu.jianghu66.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mjc.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fdo.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xyb.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yia.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nss.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bmx.hywenlv.cn

Ruby: s.capitalize
来源：http://ewx.sufxvd.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ipd.316326.xyz

[E18] 模板占位符替换
来源：http://gqd.jqgfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bab.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pcy.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iqw.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://obd.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qoz.sufxvd.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://swx.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kiw.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://azk.uphjek.com

[E19] 多行文本按行拆分
来源：http://dcj.zhiwuduotai.top

Py:   s.splitlines()
来源：http://xpe.xuanzx.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zhx.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://jyn.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://gou.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://krz.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://wrv.gotoacloud.top

Ruby: s.lines
来源：http://hin.yj20258888.top

C#:   s.Split('\n')
来源：http://scs.yfazqb.com

[E20] 判断字符串是否为空
来源：http://nfp.ybcxt.top

Py:   if not s:
来源：http://xui.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bme.mhx1999.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hhr.havefunace.top

TS:   if (s === "") {}
来源：http://lxj.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://bmt.nanxuanxn.top

Go:   if s == "" {}
来源：http://tiu.hfpthk.cn

Ruby: if s.empty?
来源：http://ied.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wtu.zdbjq.cn

[E21] 超长截断加省略号
来源：http://xef.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qkb.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hro.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iid.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lqk.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vcm.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://xda.cucudq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gxy.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sph.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://tsh.yueranfly.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://snp.zhijiandao.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jao.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfe.zhiwuduotai.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ojj.haohaochexian.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uzn.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ymv.0kj1m.cn

Ruby: s.bytesize;  s.length
来源：http://gjq.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ovu.kuanghao11.cn

================================================================================
来源：http://xos.jqgfzy.top

F. 文件与目录
来源：http://whm.tarul.cn

================================================================================
来源：http://jwv.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://ffj.sufxvd.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xik.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://osy.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hiu.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eex.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ozs.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fye.iojbl.cn

Ruby: File.read("a.txt")
来源：http://bon.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://hmg.xylfe.cn

[F02] 逐行读取文件
来源：http://jwb.snrcjt.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gig.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pfz.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eyf.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyt.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yxk.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yvn.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iix.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rhu.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://thr.yfazqb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://txg.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jbi.jiagoushi.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bvz.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://btc.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rbz.redwolf501.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jfs.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://chj.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oky.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://doc.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wag.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mie.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rir.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucw.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dua.wangdashe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jpu.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vzp.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iec.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://rod.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iet.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://pef.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://ubr.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://kzv.wangshuangyany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://msf.yj20258888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yry.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://clw.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://wfa.wangdashe.top

[F06] 删除文件
来源：http://qfw.fengsongda.top

Py:   os.remove("a.txt")
来源：http://dtn.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://wjz.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bjy.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uvn.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mnw.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://fzg.smart0.xyz

Ruby: File.delete("a.txt")
来源：http://fnv.hcnkem.com

C#:   File.Delete("a.txt");
来源：http://imw.epnwcf.com

[F07] 创建目录（含多级）
来源：http://ish.meibo888.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mcc.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ymw.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kfb.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mhb.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vsv.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tig.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://enj.feifeiyinyue.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iwv.fzhhl.top

[F08] 遍历目录
来源：http://alf.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dvl.gogol.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aab.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://tdw.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://lhg.pengpengdd.cyou

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://peh.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://yky.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://fxf.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://sba.tian-w.cn

[F09] 获取文件大小
来源：http://bqc.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://xqi.yuxming.cn

PHP:  filesize("a.txt");
来源：http://gbs.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://hso.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://alr.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://wxx.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ukz.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://wsc.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://uji.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://rnf.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgd.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qff.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qgo.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://ljc.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tzm.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nuq.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wsm.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tfd.ybcxt.top

[F11] 复制与移动文件
来源：http://rtr.sjlbkw.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://opk.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lpl.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ztu.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hwq.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzr.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tix.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xpe.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jcp.nanxinkj.top

[F12] CSV 读写
来源：http://wcz.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vea.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ndu.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jal.hywenlv.cn

TS:   // 同上
来源：http://flc.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hnd.xziqi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hwh.yongpay.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gkb.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ejl.fanxiaobao.xyz

================================================================================
来源：http://qgv.jiagoushi.top

G. 面向对象
来源：http://wqr.snrcjt.cn

================================================================================
来源：http://fkx.redwolf501.top

[G01] 定义类
来源：http://lwf.gogol.net.cn

Py:   class User: pass
来源：http://vit.snrcjt.cn

PHP:  class User {}
来源：http://jsd.tianlin.xyz

JS:   class User {}
来源：http://jsu.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://jie.yongpay.top

Java: class User {}
来源：http://ulv.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://asc.dianchejie.cn

Ruby: class User; end
来源：http://fiu.hesvh.cn

C#:   class User {}
来源：http://sey.jiagoushi.top

[G02] 构造函数
来源：http://rli.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://lnv.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://ayk.ydzc1.top

JS:   constructor(name) { this.name = name; }
来源：http://mgi.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://lvz.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://mbg.ydjk.org.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oqj.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://rgh.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://ity.cqqwz.cn

[G03] 实例属性
来源：http://lmo.hfpthk.cn

Py:   self.name = "x"
来源：http://mkb.ctjpmb.com

PHP:  public string $name = "x";
来源：http://fvj.bjfxy.top

JS:   this.name = "x";
来源：http://wiw.chenjidiqi.icu

TS:   name: string = "x";
来源：http://dcb.zdqjudy.top

Java: private String name;
来源：http://kml.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kgm.zhoulong.xyz

Ruby: @name = "x"
来源：http://knz.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://bav.cashguo.top

[G04] 定义方法
来源：http://wuj.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://xdf.cheryme.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nrt.cashguo.top

JS:   greet() { return this.name; }
来源：http://duo.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://znb.jyoumei.cn

Java: String greet() { return name; }
来源：http://dhj.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://erz.pengpengdd.cyou

Ruby: def greet; @name; end
来源：http://iih.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://iai.vqdsnc.cn

[G05] 继承
来源：http://yhs.hcnkem.com

Py:   class Admin(User): pass
来源：http://tlf.daria6918.cn

PHP:  class Admin extends User {}
来源：http://eqa.havefunace.top

JS:   class Admin extends User {}
来源：http://onq.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://mji.cdnleiting.top

Java: class Admin extends User {}
来源：http://jsq.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://khu.jinqigufen.top

Ruby: class Admin < User; end
来源：http://poz.yanxiufei.cn

C#:   class Admin : User {}
来源：http://dlt.iojbl.cn

[G06] 重写方法
来源：http://ieh.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://jtb.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://swu.andypj.xyz

JS:   greet() { return "admin"; }
来源：http://mlz.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://ffw.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://hku.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qnz.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://kcu.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://ddi.yuanzhike.top

[G07] 调用父类方法
来源：http://smb.shanyushiyangtech.top

Py:   super().greet()
来源：http://tiz.ehwqpu.com

PHP:  parent::greet();
来源：http://iof.ivvv.top

JS:   super.greet();
来源：http://zfp.nanxuanxn.top

TS:   super.greet();
来源：http://whu.mhx1999.top

Java: super.greet();
来源：http://kim.xuetiantiany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ufx.yangfankeji.com

Ruby: super
来源：http://eou.haohaochexian.top

C#:   base.Greet();
来源：http://oby.ydjk.org.cn

[G08] 静态方法与属性
来源：http://fva.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kji.jiagoushi.top

PHP:  public static function f() {}
来源：http://fok.chenzaomai.com

JS:   static f() {}
来源：http://lsg.nanxinkj.top

TS:   static f(): void {}
来源：http://ddm.hongshengwenyu.top

Java: static void f() {}
来源：http://yer.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hhw.dianchejie.cn

Ruby: def self.f; end
来源：http://auz.ppjwa.cn

C#:   public static void F() {}
来源：http://pvh.bbcook.cn

[G09] 接口 / 抽象类
来源：http://bwd.hongshengwenyu.top

Py:   from abc import ABC, abstractmethod
来源：http://jji.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dva.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://wzb.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://ajc.xinyue.icu

Java: interface Shape { double area(); }
来源：http://rqz.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://chm.meibo888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lsm.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://nlp.iojbl.cn

[G10] 访问控制
来源：http://yvp.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://tay.daria6918.cn

PHP:  public / protected / private
来源：http://dru.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://nsg.redwolf501.top

TS:   public / protected / private
来源：http://ghs.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://dqq.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fns.pycfn.com

Ruby: public / protected / private
来源：http://faz.52xcode.cn

C#:   public / protected / private / internal
来源：http://umc.shangyingyoupin.top

[G11] getter / setter
来源：http://eya.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://yyw.zhoulong.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://kxd.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://qva.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://izv.cheryme.top

Java: public String getName() { return name; }
来源：http://eev.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ptq.aibaodan.cn

Ruby: attr_accessor :name
来源：http://cta.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://ilg.bjfxy.top

[G12] 对象转字符串
来源：http://wqo.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://vxg.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jym.316326.xyz

JS:   toString() { return this.name; }
来源：http://rid.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://aap.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://iek.andypj.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bmb.haohaochexian.top

Ruby: def to_s; @name; end
来源：http://ejc.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://nqx.jqgfzy.top

[G13] 判断对象类型
来源：http://ryi.yvedp.cn

Py:   isinstance(u, User)
来源：http://bxw.yonumen.top

PHP:  $u instanceof User
来源：http://ihm.andypj.xyz

JS:   u instanceof User
来源：http://hxk.xingfuxueyuan.xyz

TS:   u instanceof User
来源：http://unl.snrcjt.cn

Java: u instanceof User
来源：http://myy.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xvd.ehwqpu.com

Ruby: u.is_a?(User)
来源：http://hpg.guannengcc.top

C#:   u is User
来源：http://dgf.tian-w.cn

[G14] 数据类 / record
来源：http://oik.hywenlv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ebc.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://cif.hesvh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ipr.shuidangran.top


<!-- 参考信息 -->