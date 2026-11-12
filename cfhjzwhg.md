代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://slt.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uud.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jlv.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xan.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzu.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://abf.cashguo.top

Py:   s.splitlines()
来源：http://wdd.jianghu66.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mtk.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://kxr.fktsv.cn

TS:   s.split(/\r?\n/)
来源：http://ffs.ydzc1.top

Java: s.lines().toList()
来源：http://crw.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://gmz.316326.xyz

Ruby: s.lines
来源：http://sct.jyoumei.cn

C#:   s.Split('\n')
来源：http://tdy.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://yxy.jinqigufen.top

Py:   if not s:
来源：http://htu.hnxiangtu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jlu.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sld.yfazqb.com

TS:   if (s === "") {}
来源：http://ymk.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://npr.fengsongda.top

Go:   if s == "" {}
来源：http://wfq.gogol.net.cn

Ruby: if s.empty?
来源：http://igi.havefunace.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nbg.xylfe.cn

[E21] 超长截断加省略号
来源：http://mof.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ojx.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vqd.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rlv.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mkk.jqgufenzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gnv.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://lzw.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bpg.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://btm.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://pbb.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cul.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dty.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lri.aibaodan.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://njf.tianlin.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://thk.jqgufenzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ohh.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://tfv.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://htz.hesvh.cn

================================================================================
来源：http://qxm.tarul.cn

F. 文件与目录
来源：http://iml.tarul.cn

================================================================================
来源：http://lvn.xuanzx.com

[F01] 读取整个文件
来源：http://opr.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qjw.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://jdz.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ngg.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yck.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fvl.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fkk.ivvv.top

Ruby: File.read("a.txt")
来源：http://pes.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://nmz.fanxiaobao.xyz

[F02] 逐行读取文件
来源：http://ixy.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zdt.yuxming.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bdn.sweek.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ppa.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://loy.andypj.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vhs.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uzd.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uro.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://myn.haohaochexian.top

[F03] 写入文件（覆盖）
来源：http://nlp.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ynt.yuanzhike.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rpp.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gdv.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ohi.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mec.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tpv.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://kyc.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wed.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://nob.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fpf.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lhx.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sua.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kay.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vtv.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tnn.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ghi.hywenlv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ucm.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://jtm.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ora.zycfv.cn

PHP:  file_exists("a.txt");
来源：http://smp.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://gyv.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://kwk.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xky.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vtk.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://wcf.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://jjt.svipenyu.cn

[F06] 删除文件
来源：http://slz.yuxming.cn

Py:   os.remove("a.txt")
来源：http://bel.yj20258888.top

PHP:  unlink("a.txt");
来源：http://vpj.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vft.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://vkh.smart0.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vuh.guannengcc.top

Go:   os.Remove("a.txt")
来源：http://rqd.ivvv.top

Ruby: File.delete("a.txt")
来源：http://oph.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://sxh.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://hal.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fgq.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kuv.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axt.quarkkingdee.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uie.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sap.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dah.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mbe.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fut.aibaodan.cn

[F08] 遍历目录
来源：http://zno.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ckv.gotoacloud.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vho.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://psf.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://gts.c1oappe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zmc.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ehk.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://swu.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://ypp.tian-w.cn

[F09] 获取文件大小
来源：http://rfe.zhiwuduotai.top

Py:   os.path.getsize("a.txt")
来源：http://jyl.redwolf501.top

PHP:  filesize("a.txt");
来源：http://buo.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://tkq.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://zxl.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hfz.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://trn.hammf.cn

Ruby: File.size("a.txt")
来源：http://crm.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://epb.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ric.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sxo.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://drf.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xrq.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://yju.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eol.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hnm.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hjg.zhengqikj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://roj.vehdjk.com

[F11] 复制与移动文件
来源：http://bbq.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hbx.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kda.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ubl.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sdn.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gfi.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jix.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wig.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qcs.hnqzz.top

[F12] CSV 读写
来源：http://cfn.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dho.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://woc.fktsv.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mlx.gotoacloud.top

TS:   // 同上
来源：http://jew.xuanzx.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zca.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ztf.ywan-chungtsiang.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gdw.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://coe.gogol.net.cn

================================================================================
来源：http://xdj.xuetiantiany.cn

G. 面向对象
来源：http://zwv.jqgfzy.top

================================================================================
来源：http://apy.ivvv.top

[G01] 定义类
来源：http://sdx.pengpengdd.cyou

Py:   class User: pass
来源：http://ahc.jqgufenzy.top

PHP:  class User {}
来源：http://sfl.jqgufenzy.top

JS:   class User {}
来源：http://zgw.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://wah.xinyue.icu

Java: class User {}
来源：http://xah.zhaomingkeji.xyz

Go:   type User struct { Name string }
来源：http://ojf.ivvv.top

Ruby: class User; end
来源：http://mkz.yvedp.cn

C#:   class User {}
来源：http://xcx.yvedp.cn

[G02] 构造函数
来源：http://yem.gotoacloud.top

Py:   def __init__(self, name): self.name = name
来源：http://mcm.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://git.tanke756.top

JS:   constructor(name) { this.name = name; }
来源：http://bhf.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://rqw.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://xnw.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uox.hammf.cn

Ruby: def initialize(name); @name = name; end
来源：http://gma.meibo888.top

C#:   public User(string name) { Name = name; }
来源：http://xik.gotoacloud.top

[G03] 实例属性
来源：http://cse.bbcook.cn

Py:   self.name = "x"
来源：http://wsq.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://kzv.haohaochexian.top

JS:   this.name = "x";
来源：http://jes.hnxiangtu.top

TS:   name: string = "x";
来源：http://xcc.fanxiaobao.xyz

Java: private String name;
来源：http://cdv.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ypl.cucudq.cn

Ruby: @name = "x"
来源：http://cac.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://kge.cheryme.top

[G04] 定义方法
来源：http://kgd.fengsongda.top

Py:   def greet(self): return self.name
来源：http://xip.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://isp.guannengcc.top

JS:   greet() { return this.name; }
来源：http://noy.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://jgp.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://ptq.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ypp.cheryme.top

Ruby: def greet; @name; end
来源：http://ppi.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://ufb.guannengcc.top

[G05] 继承
来源：http://awz.gaohongyu789.top

Py:   class Admin(User): pass
来源：http://uti.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://gmr.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://jhj.yuanzhike.top

TS:   class Admin extends User {}
来源：http://rff.gotoacloud.top

Java: class Admin extends User {}
来源：http://esh.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uxh.sxryk.cn

Ruby: class Admin < User; end
来源：http://ypm.ctjpmb.com

C#:   class Admin : User {}
来源：http://wiz.yj202588.top

[G06] 重写方法
来源：http://ywl.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://eht.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tlc.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://fyp.shanyushiyangtech.top

TS:   greet(): string { return "admin"; }
来源：http://sna.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://ebn.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dpx.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://lbk.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://cbc.shangyingyoupin.top

[G07] 调用父类方法
来源：http://wct.ehwqpu.com

Py:   super().greet()
来源：http://dro.sjlbkw.cn

PHP:  parent::greet();
来源：http://yne.shangyingyoupin.top

JS:   super.greet();
来源：http://twx.dashuyun.cn

TS:   super.greet();
来源：http://phg.hongshengwenyu.top

Java: super.greet();
来源：http://imc.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fvn.gzhubu.top

Ruby: super
来源：http://frx.dianchejie.cn

C#:   base.Greet();
来源：http://ibu.gaohongyu789.top

[G08] 静态方法与属性
来源：http://hmr.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://btk.tarul.cn

PHP:  public static function f() {}
来源：http://dup.gzhubu.top

JS:   static f() {}
来源：http://tev.jinqigfzy.top

TS:   static f(): void {}
来源：http://jil.jinghuilouyu.cn

Java: static void f() {}
来源：http://uvc.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xvz.ivvv.top

Ruby: def self.f; end
来源：http://pbj.xziqi.cn

C#:   public static void F() {}
来源：http://hfl.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://dvu.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://kem.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://dsz.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cio.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://rhg.meibo888.top

Java: interface Shape { double area(); }
来源：http://xrg.cdnleiting.top

Go:   type Shape interface { Area() float64 }
来源：http://bid.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cjs.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://esi.cdnleiting.top

[G10] 访问控制
来源：http://gjr.bbcook.cn

Py:   约定 _protected / __private（不强制）
来源：http://lcv.yuxming.cn

PHP:  public / protected / private
来源：http://arj.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://smf.daria6918.cn

TS:   public / protected / private
来源：http://hbi.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://oac.hysaishi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ypn.hesvh.cn

Ruby: public / protected / private
来源：http://cyz.hcnkem.com

C#:   public / protected / private / internal
来源：http://dqa.zdbjq.cn

[G11] getter / setter
来源：http://sty.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://afd.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://adp.fengsongda.top

JS:   get name() { return this._name; }
来源：http://kzp.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://imy.ywan-chungtsiang.top

Java: public String getName() { return name; }
来源：http://czv.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jcv.tanke756.top

Ruby: attr_accessor :name
来源：http://awq.sweek.top

C#:   public string Name { get; set; }
来源：http://oyn.c1oappe.top

[G12] 对象转字符串
来源：http://mqb.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://tyc.yanxiufei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbx.cucudq.cn

JS:   toString() { return this.name; }
来源：http://pro.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://nqj.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://wzl.sxryk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cgt.redwolf501.top

Ruby: def to_s; @name; end
来源：http://tue.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://cpw.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://fzk.yj202588.top

Py:   isinstance(u, User)
来源：http://rig.ppjwa.cn

PHP:  $u instanceof User
来源：http://jyd.daxiang520.top

JS:   u instanceof User
来源：http://mhp.yj20258888.top

TS:   u instanceof User
来源：http://whj.aibaodan.cn

Java: u instanceof User
来源：http://jsz.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://esi.hesvh.cn

Ruby: u.is_a?(User)
来源：http://ppv.quarkkingdee.top

C#:   u is User
来源：http://hta.0kj1m.cn

[G14] 数据类 / record
来源：http://dpp.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zvl.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://hps.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://gaz.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://xua.hongshengwenyu.top

Java: record User(String name, int age) {}
来源：http://ucc.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://enh.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dps.yongpay.top

C#:   record User(string Name, int Age);
来源：http://vfr.hcnkem.com

[G15] 枚举
来源：http://ztv.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://alm.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jpi.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yej.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://deu.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://ivj.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fmx.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://cqf.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nsr.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://vuu.zhixingplan.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kdw.chenzaomai.com

PHP:  get_object_vars($obj);
来源：http://sif.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://pni.0kj1m.cn

TS:   Object.entries(obj)
来源：http://meo.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qiu.tanke756.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ynk.sufxvd.cn

Ruby: obj.instance_variables
来源：http://hrk.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://lbw.yj20258.top

================================================================================
来源：http://txz.vehdjk.com


<!-- 参考信息 -->