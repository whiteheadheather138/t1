代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pls.dashuyun.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ofr.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://vpn.yj20258.top

[E17] 首字母大写
来源：http://zsj.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://isw.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cuh.zdbjq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bju.zhiwuduotai.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://frb.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vht.nanxinkj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://slq.ivvv.top

Ruby: s.capitalize
来源：http://lkl.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://iyt.quarkkingdee.top

[E18] 模板占位符替换
来源：http://bzf.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ztq.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wso.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oqg.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nxj.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hpf.zdbjq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gix.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hpk.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wgh.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://dbw.jqgfzy.top

Py:   s.splitlines()
来源：http://afd.epnwcf.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xet.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://zlq.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://rlh.kuanghao11.cn

Java: s.lines().toList()
来源：http://pth.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://hdn.yuanzhike.top

Ruby: s.lines
来源：http://bol.xinyue.icu

C#:   s.Split('\n')
来源：http://dnz.hammf.cn

[E20] 判断字符串是否为空
来源：http://gcz.jinqigufen.top

Py:   if not s:
来源：http://oaf.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lit.kuanghao11.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fhu.cucudq.cn

TS:   if (s === "") {}
来源：http://vjc.ybcxt.top

Java: if (s.isEmpty()) {}
来源：http://snp.bjfxy.top

Go:   if s == "" {}
来源：http://ski.0kj1m.cn

Ruby: if s.empty?
来源：http://ufu.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tnk.aizwys.cn

[E21] 超长截断加省略号
来源：http://ffn.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jge.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xkd.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hov.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jsi.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gxi.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://gjh.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tet.xingfuxueyuan.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sws.chenzaomai.com

[E22] 字节长度与字符长度
来源：http://zfi.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vxk.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hkb.zdqjudy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ven.0kj1m.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nwq.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rtl.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uqc.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://vnp.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gli.chenzaomai.com

================================================================================
来源：http://oha.shangyingyoupin.top

F. 文件与目录
来源：http://scb.meibo888.top

================================================================================
来源：http://pmn.nanxinkj.top

[F01] 读取整个文件
来源：http://yrj.hywenlv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mee.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://ygb.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eau.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zye.zhengqikj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ftf.hfpthk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://acu.fzhhl.top

Ruby: File.read("a.txt")
来源：http://tqg.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://qaa.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://zls.jinyuanbaomall.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yrw.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zff.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cdg.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://for.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zpe.havefunace.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gna.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lxl.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mbf.chenlongwang.top

[F03] 写入文件（覆盖）
来源：http://dyh.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ren.smart0.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://lio.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzq.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lux.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cpr.c1oappe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cxm.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://rau.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ghk.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://phk.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://unm.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://grv.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xzt.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rnq.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfq.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://viq.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dnc.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkb.epnwcf.com

[F05] 判断文件或目录是否存在
来源：http://tdt.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://enb.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://slg.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://yle.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://utp.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://aaa.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://foz.0kj1m.cn

Ruby: File.exist?("a.txt")
来源：http://wqo.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://nho.yvedp.cn

[F06] 删除文件
来源：http://izt.fktsv.cn

Py:   os.remove("a.txt")
来源：http://kon.sweek.top

PHP:  unlink("a.txt");
来源：http://ran.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hrj.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://rbs.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sua.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://sbh.sjlbkw.cn

Ruby: File.delete("a.txt")
来源：http://jug.hnqzz.top

C#:   File.Delete("a.txt");
来源：http://fnq.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://fqm.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://odq.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nlh.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vey.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvr.bjfxy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mup.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rpq.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ohw.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bzo.yuanzhike.top

[F08] 遍历目录
来源：http://bcb.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fbk.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yaw.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://znj.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://som.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yht.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://jwb.sweek.top

Ruby: Dir.children("dir")
来源：http://cfy.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://opk.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://lsd.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://zlk.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://vix.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://csf.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://kxo.dashuyun.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lag.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eib.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://gdx.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://alc.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://lgc.vqdsnc.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://djp.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xza.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yvi.gotoacloud.top

TS:   path.extname("a.txt")
来源：http://ztb.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jak.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://abb.yj20258.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ttl.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hjg.hcnkem.com

[F11] 复制与移动文件
来源：http://gvj.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vgx.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vvj.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nyi.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oxv.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wmh.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ipe.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wfb.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dcg.yanxiufei.cn

[F12] CSV 读写
来源：http://ulx.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xdz.wangdashe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxj.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yjv.jlsjyb.cn

TS:   // 同上
来源：http://jye.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://itr.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xnb.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://aqk.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://tkg.52xcode.cn

================================================================================
来源：http://pac.tanke756.top

G. 面向对象
来源：http://rhq.yonumen.top

================================================================================
来源：http://jwq.guannengcc.top

[G01] 定义类
来源：http://hfr.shanyushiyangtech.top

Py:   class User: pass
来源：http://tzu.fzhhl.top

PHP:  class User {}
来源：http://rtm.guannengcc.top

JS:   class User {}
来源：http://xih.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://shh.jinyuanbaomall.cn

Java: class User {}
来源：http://aej.tianlin.xyz

Go:   type User struct { Name string }
来源：http://eun.vqdsnc.cn

Ruby: class User; end
来源：http://rah.hcnkem.com

C#:   class User {}
来源：http://rov.xuanzx.com

[G02] 构造函数
来源：http://vnt.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://zty.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://ppe.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://gqt.haohaochexian.top

TS:   constructor(public name: string) {}
来源：http://jmv.sweek.top

Java: User(String name) { this.name = name; }
来源：http://xyw.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bjd.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://eme.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://aei.cashguo.top

[G03] 实例属性
来源：http://beo.gogol.net.cn

Py:   self.name = "x"
来源：http://hat.yvedp.cn

PHP:  public string $name = "x";
来源：http://vtr.yj202588.top

JS:   this.name = "x";
来源：http://wfz.jqgfzy.top

TS:   name: string = "x";
来源：http://uad.jinghuilouyu.cn

Java: private String name;
来源：http://hit.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tvm.yuxming.cn

Ruby: @name = "x"
来源：http://qdj.jinyuanbaomall.cn

C#:   public string Name { get; set; } = "x";
来源：http://atz.ctjpmb.com

[G04] 定义方法
来源：http://dor.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://tul.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jlc.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://cls.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://zuz.xuanzx.com

Java: String greet() { return name; }
来源：http://fex.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://abj.yueranfly.top

Ruby: def greet; @name; end
来源：http://zmi.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://qff.jinqigfzy.top

[G05] 继承
来源：http://kgm.bbcook.cn

Py:   class Admin(User): pass
来源：http://aiv.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://dic.daria6918.cn

JS:   class Admin extends User {}
来源：http://xkr.jianghu66.top

TS:   class Admin extends User {}
来源：http://vwc.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://nyj.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rdb.jinqigfzy.top

Ruby: class Admin < User; end
来源：http://wxp.aibaodan.cn

C#:   class Admin : User {}
来源：http://jhg.quarkkingdee.top

[G06] 重写方法
来源：http://zbk.cashguo.top

Py:   def greet(self): return "admin"
来源：http://fob.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qcv.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://hkd.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://aed.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://vyv.yuanzhike.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uji.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://wjr.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://lwf.uphjek.com

[G07] 调用父类方法
来源：http://tdp.yangfankeji.com

Py:   super().greet()
来源：http://yxn.yfazqb.com

PHP:  parent::greet();
来源：http://ewh.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://oim.yonumen.top

TS:   super.greet();
来源：http://dkd.tian-w.cn

Java: super.greet();
来源：http://val.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fru.hesvh.cn

Ruby: super
来源：http://uvp.tianlin.xyz

C#:   base.Greet();
来源：http://jzv.dashuyun.cn

[G08] 静态方法与属性
来源：http://hal.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://avf.jianghu66.top

PHP:  public static function f() {}
来源：http://gmm.xylfe.cn

JS:   static f() {}
来源：http://hzd.snrcjt.cn

TS:   static f(): void {}
来源：http://tnw.hnxiangtu.top

Java: static void f() {}
来源：http://qsd.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pnf.xinyue.icu

Ruby: def self.f; end
来源：http://psa.cqqwz.cn

C#:   public static void F() {}
来源：http://jla.hysaishi.cn

[G09] 接口 / 抽象类
来源：http://vcf.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://syu.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nup.daria6918.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://goi.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://fhk.yj20258888.top

Java: interface Shape { double area(); }
来源：http://dyt.zdbjq.cn

Go:   type Shape interface { Area() float64 }
来源：http://vay.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sqh.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://nls.hywenlv.cn

[G10] 访问控制
来源：http://hpa.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://ndo.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://vne.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://gka.xinyue.icu

TS:   public / protected / private
来源：http://ufu.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://vwk.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jcm.52xcode.cn

Ruby: public / protected / private
来源：http://gji.cheryme.top

C#:   public / protected / private / internal
来源：http://jwl.zhixingplan.top

[G11] getter / setter
来源：http://dgb.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://spu.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://dup.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://noo.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://joc.iojbl.cn

Java: public String getName() { return name; }
来源：http://jwk.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qud.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://ucq.uphjek.com

C#:   public string Name { get; set; }
来源：http://qle.guannengcc.top

[G12] 对象转字符串
来源：http://myr.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://yga.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ydv.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://iqr.xinyue.icu

TS:   toString(): string { return this.name; }
来源：http://ept.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://rfx.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qcr.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://nqf.meibo888.top

C#:   public override string ToString() => Name;
来源：http://vzm.haohaochexian.top

[G13] 判断对象类型
来源：http://uzx.tianlin.xyz

Py:   isinstance(u, User)
来源：http://yrz.52xcode.cn

PHP:  $u instanceof User
来源：http://slt.52xcode.cn

JS:   u instanceof User
来源：http://hgl.aizwys.cn

TS:   u instanceof User
来源：http://bpf.zhaomingkeji.xyz

Java: u instanceof User
来源：http://epo.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://hui.cashguo.top

Ruby: u.is_a?(User)
来源：http://iqg.jinghuilouyu.cn

C#:   u is User
来源：http://euv.pycfn.com

[G14] 数据类 / record
来源：http://teg.316326.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ioy.cucudq.cn

PHP:  // 用 readonly 属性模拟
来源：http://jlc.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ubs.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://swr.tanke756.top

Java: record User(String name, int age) {}
来源：http://wlj.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://gte.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cdb.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://mvb.cheryme.top

[G15] 枚举
来源：http://pes.uphjek.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sky.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://szr.pengpengdd.cyou


<!-- 参考信息 -->