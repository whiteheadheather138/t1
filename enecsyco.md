代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://fxm.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://efn.fanxiaobao.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qpf.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sux.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jin.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://vul.nwbrower.top

Py:   s.splitlines()
来源：http://sne.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jxy.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://lsg.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://ior.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://njh.hammf.cn

Go:   strings.Split(s, "\n")
来源：http://mze.feifeiyinyue.top

Ruby: s.lines
来源：http://ccj.yuxming.cn

C#:   s.Split('\n')
来源：http://aje.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://tfm.zhoulong.xyz

Py:   if not s:
来源：http://wmm.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sod.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://llx.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://bfl.jqgfzy.top

Java: if (s.isEmpty()) {}
来源：http://eoh.c1oappe.top

Go:   if s == "" {}
来源：http://sbh.xingfuxueyuan.xyz

Ruby: if s.empty?
来源：http://llb.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bkj.jinqigufen.top

[E21] 超长截断加省略号
来源：http://teq.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://abn.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://heu.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zwh.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gtb.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rzw.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://tzm.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xsd.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxr.fehbvm.com

[E22] 字节长度与字符长度
来源：http://ltp.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oey.ywan-chungtsiang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mnk.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rfp.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yeb.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ole.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://upq.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://zdv.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hkx.yuxming.cn

================================================================================
来源：http://fjt.zhijiandao.cn

F. 文件与目录
来源：http://mal.kuanghao11.cn

================================================================================
来源：http://otf.daxiang520.top

[F01] 读取整个文件
来源：http://vpb.yueranfly.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ron.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://qkc.jinqigfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wmz.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yvw.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kvp.ybcxt.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lor.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://qmj.yuxming.cn

C#:   File.ReadAllText("a.txt");
来源：http://reh.jinqigfzy.top

[F02] 逐行读取文件
来源：http://yln.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jkp.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vey.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zda.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uba.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sgu.vqdsnc.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hnn.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ojx.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kce.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://tep.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oau.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://rdf.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iet.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fac.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uva.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ooz.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://mqn.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xyf.ydjk.org.cn

[F04] 追加写入文件
来源：http://zvk.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ipu.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://deh.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ppt.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vhi.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ifo.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ujg.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tdx.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qeo.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://cuo.zhixingplan.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dfb.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://zhw.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://slx.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://zas.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yyb.sweek.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hjf.guowangkeji.top

Ruby: File.exist?("a.txt")
来源：http://ywq.meibo888.top

C#:   File.Exists("a.txt")
来源：http://wfk.meibo888.top

[F06] 删除文件
来源：http://elp.fehbvm.com

Py:   os.remove("a.txt")
来源：http://wwt.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://ugw.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://csy.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://upo.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fuv.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://kov.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://aqc.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://kgp.hcnkem.com

[F07] 创建目录（含多级）
来源：http://afn.yj20258.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qlz.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zos.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qoz.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tvm.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vsn.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fxy.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xgf.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ftk.iojbl.cn

[F08] 遍历目录
来源：http://cyl.feifeiyinyue.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sst.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ytm.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://jgp.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://pje.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xjv.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ytw.gzhubu.top

Ruby: Dir.children("dir")
来源：http://myk.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://xpl.9152youxi.cn

[F09] 获取文件大小
来源：http://ltm.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://fmi.yvedp.cn

PHP:  filesize("a.txt");
来源：http://yxt.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://gvw.hesvh.cn

TS:   fs.statSync("a.txt").size
来源：http://rtn.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bii.ivvv.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wwz.tian-w.cn

Ruby: File.size("a.txt")
来源：http://yse.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://vju.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://ajh.aibaodan.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ohf.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://usq.svipenyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ych.snrcjt.cn

TS:   path.extname("a.txt")
来源：http://mnf.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bqf.hcnkem.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ily.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wyu.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xhy.ctjpmb.com

[F11] 复制与移动文件
来源：http://qpo.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zau.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zcf.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://een.zhaomingkeji.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xip.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://del.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aag.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jur.zhiwuduotai.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jeh.zdqjudy.top

[F12] CSV 读写
来源：http://obv.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://shp.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pmi.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://goq.cucudq.cn

TS:   // 同上
来源：http://qxr.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lyu.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bgg.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fbn.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://msi.yonumen.top

================================================================================
来源：http://lhq.hnqzz.top

G. 面向对象
来源：http://dis.redwolf501.top

================================================================================
来源：http://vxw.wangshuangyany.cn

[G01] 定义类
来源：http://slk.jlsjyb.cn

Py:   class User: pass
来源：http://ixz.yonumen.top

PHP:  class User {}
来源：http://lnn.quarkkingdee.top

JS:   class User {}
来源：http://upq.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://zdp.yj20258888.top

Java: class User {}
来源：http://yxv.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://cqt.xinyue.icu

Ruby: class User; end
来源：http://hfo.jqgufenzy.top

C#:   class User {}
来源：http://yzh.52xcode.cn

[G02] 构造函数
来源：http://mej.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://qfe.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://irq.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://lyu.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://kqs.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://kro.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ihs.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://zqu.jianghu66.top

C#:   public User(string name) { Name = name; }
来源：http://nug.havefunace.top

[G03] 实例属性
来源：http://xbd.shanyushiyangtech.top

Py:   self.name = "x"
来源：http://duj.ydzc1.top

PHP:  public string $name = "x";
来源：http://xqm.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://qty.yuxming.cn

TS:   name: string = "x";
来源：http://hqv.dianchejie.cn

Java: private String name;
来源：http://vjj.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kib.yfazqb.com

Ruby: @name = "x"
来源：http://ddx.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://rib.sjlbkw.cn

[G04] 定义方法
来源：http://azx.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://wig.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dlh.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://quu.0kj1m.cn

TS:   greet(): string { return this.name; }
来源：http://fzu.yangfankeji.com

Java: String greet() { return name; }
来源：http://thl.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uxs.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://jwl.yj20258.top

C#:   public string Greet() => Name;
来源：http://biy.vqdsnc.cn

[G05] 继承
来源：http://acv.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://ypb.fengsongda.top

PHP:  class Admin extends User {}
来源：http://krg.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://zys.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://vub.yj202588.top

Java: class Admin extends User {}
来源：http://rxj.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iqj.wangshuangyany.cn

Ruby: class Admin < User; end
来源：http://tmx.svipenyu.cn

C#:   class Admin : User {}
来源：http://ntq.yangfankeji.com

[G06] 重写方法
来源：http://tfq.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://gpg.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ovg.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://zkf.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://byn.redwolf501.top

Java: @Override String greet() { return "admin"; }
来源：http://bra.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://icj.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://otr.zhoulong.xyz

C#:   public override string Greet() => "admin";
来源：http://xqv.hnqzz.top

[G07] 调用父类方法
来源：http://jtz.ppjwa.cn

Py:   super().greet()
来源：http://xcu.yanxiufei.cn

PHP:  parent::greet();
来源：http://qcw.fktsv.cn

JS:   super.greet();
来源：http://anb.jinqigfzy.top

TS:   super.greet();
来源：http://xzq.fengsongda.top

Java: super.greet();
来源：http://otf.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sau.ydjk.org.cn

Ruby: super
来源：http://ywp.jqgfzy.top

C#:   base.Greet();
来源：http://ksf.hammf.cn

[G08] 静态方法与属性
来源：http://bwi.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oke.zhijiandao.cn

PHP:  public static function f() {}
来源：http://doi.zdbjq.cn

JS:   static f() {}
来源：http://vzk.cashguo.top

TS:   static f(): void {}
来源：http://via.jianghu66.top

Java: static void f() {}
来源：http://cie.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rhv.xuanzx.com

Ruby: def self.f; end
来源：http://amc.ydjk.org.cn

C#:   public static void F() {}
来源：http://nic.yj20258888.top

[G09] 接口 / 抽象类
来源：http://nmp.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://fxy.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://pup.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fpz.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://wbu.fehbvm.com

Java: interface Shape { double area(); }
来源：http://tsa.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cey.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ypd.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://gap.fzhhl.top

[G10] 访问控制
来源：http://zwz.feifeiyinyue.top

Py:   约定 _protected / __private（不强制）
来源：http://oua.sysykeji.top

PHP:  public / protected / private
来源：http://prv.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://dlr.dianchejie.cn

TS:   public / protected / private
来源：http://pan.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://mnd.xingfuxueyuan.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://ouo.shzxlz.cn

Ruby: public / protected / private
来源：http://zhz.dianchejie.cn

C#:   public / protected / private / internal
来源：http://yai.chenjidiqi.icu

[G11] getter / setter
来源：http://gyh.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://xoi.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dtp.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://xsz.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://ear.xuanzx.com

Java: public String getName() { return name; }
来源：http://cuq.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lgo.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://cbh.yj20258888.top

C#:   public string Name { get; set; }
来源：http://qlg.yonumen.top

[G12] 对象转字符串
来源：http://hpo.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://mcs.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zct.yj20258.top

JS:   toString() { return this.name; }
来源：http://lbf.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://rqh.gaohongyu789.top

Java: @Override public String toString() { return name; }
来源：http://ekg.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://xix.zhijiandao.cn

Ruby: def to_s; @name; end
来源：http://kbk.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://amg.chenjidiqi.icu

[G13] 判断对象类型
来源：http://wte.smart0.xyz

Py:   isinstance(u, User)
来源：http://rnk.aizwys.cn

PHP:  $u instanceof User
来源：http://ihc.snrcjt.cn

JS:   u instanceof User
来源：http://xwz.ydjk.org.cn

TS:   u instanceof User
来源：http://mcc.feifeiyinyue.top

Java: u instanceof User
来源：http://sio.jiagoushi.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zkx.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://lve.xuetiantiany.cn

C#:   u is User
来源：http://vvm.aizwys.cn

[G14] 数据类 / record
来源：http://jke.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xfh.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://diy.zhiwuduotai.top

JS:   // 无内置：普通类或对象字面量
来源：http://xoq.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://vph.mhx1999.top

Java: record User(String name, int age) {}
来源：http://isc.pycfn.com

Go:   type User struct { Name string; Age int }
来源：http://wqf.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jny.vqdsnc.cn

C#:   record User(string Name, int Age);
来源：http://rav.ydjk.org.cn

[G15] 枚举
来源：http://pkw.cheryme.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://snp.hysaishi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fuu.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dch.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sna.shzxlz.cn

Java: enum Color { RED, GREEN }
来源：http://gta.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mbf.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://qme.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hjc.chenjidiqi.icu

[G16] 对象转数组 / 字典
来源：http://vyk.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vjd.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://fwj.dianchejie.cn

JS:   Object.entries(obj)
来源：http://yfe.zhixingplan.top

TS:   Object.entries(obj)
来源：http://ady.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bux.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gfb.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://anz.jlsjyb.cn

C#:   // 用反射或 System.Text.Json
来源：http://bic.ctjpmb.com

================================================================================
来源：http://xsh.sxryk.cn


<!-- 参考信息 -->