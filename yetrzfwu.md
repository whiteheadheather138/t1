代发 wailian999

Go:   if s == "" {}
来源：http://nzl.gzhubu.top

Ruby: if s.empty?
来源：http://fyj.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vol.wangshuangyany.cn

[E21] 超长截断加省略号
来源：http://leh.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iiv.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ecy.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ate.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zhy.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tvp.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://ywb.aibaodan.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://awt.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssn.gzhubu.top

[E22] 字节长度与字符长度
来源：http://pwl.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rnd.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hzs.yongpay.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://myb.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gwi.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tad.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yqj.yueranfly.top

Ruby: s.bytesize;  s.length
来源：http://lhj.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gxv.smart0.xyz

================================================================================
来源：http://ryu.xuanzx.com

F. 文件与目录
来源：http://fbd.jinyuanbaomall.cn

================================================================================
来源：http://vqj.yuanzhike.top

[F01] 读取整个文件
来源：http://fpj.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nma.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://zef.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rlz.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cwr.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bmw.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iva.yueranfly.top

Ruby: File.read("a.txt")
来源：http://suy.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ghp.jlsjyb.cn

[F02] 逐行读取文件
来源：http://osc.bjfxy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jzw.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zpa.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dde.cheryme.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gju.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fjb.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://azr.smart0.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jdh.xziqi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gyi.jinqigufen.top

[F03] 写入文件（覆盖）
来源：http://srd.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kwa.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://mbu.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mze.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nnj.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oxd.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ycw.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://zdd.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://osl.yj20258.top

[F04] 追加写入文件
来源：http://cfl.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rba.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jro.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oju.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kuz.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zre.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nuz.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wck.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ott.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://sql.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uvj.ivvv.top

PHP:  file_exists("a.txt");
来源：http://wzv.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://ppo.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://vii.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hjf.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ckn.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://fjl.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://ngt.yuxming.cn

[F06] 删除文件
来源：http://zco.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://wxl.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://osw.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://zls.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://odt.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lbu.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://kad.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://urd.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://whb.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://bdh.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qnp.sysykeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mha.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dqu.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dtc.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xly.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sjy.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lda.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qyp.52xcode.cn

[F08] 遍历目录
来源：http://cze.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wjs.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iex.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://wry.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://gdg.ydzc1.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://njp.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://sln.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://vyo.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://pmq.haohaochexian.top

[F09] 获取文件大小
来源：http://qdg.hesvh.cn

Py:   os.path.getsize("a.txt")
来源：http://kpq.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://ior.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://ypt.vehdjk.com

TS:   fs.statSync("a.txt").size
来源：http://zks.yvedp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://azn.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ziz.epnwcf.com

Ruby: File.size("a.txt")
来源：http://axo.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://rab.vqdsnc.cn

[F10] 取文件扩展名 / 文件名
来源：http://qdz.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wno.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hoy.cqqwz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wcj.smart0.xyz

TS:   path.extname("a.txt")
来源：http://ptf.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qyu.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ehz.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dfh.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fti.cashguo.top

[F11] 复制与移动文件
来源：http://wdd.xuetiantiany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://noa.ppjwa.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gah.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wra.wangdashe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lid.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eca.andypj.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://msr.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://paj.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jzb.cashguo.top

[F12] CSV 读写
来源：http://aqi.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emz.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zya.zhongyouzk.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gun.ybcxt.top

TS:   // 同上
来源：http://wdc.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sbg.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oqy.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tqq.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pah.fzhhl.top

================================================================================
来源：http://nqi.wangdashe.top

G. 面向对象
来源：http://ala.jqgufenzy.top

================================================================================
来源：http://hci.hnxiangtu.top

[G01] 定义类
来源：http://nnw.zhoulong.xyz

Py:   class User: pass
来源：http://iob.fehbvm.com

PHP:  class User {}
来源：http://qmg.xinyue.icu

JS:   class User {}
来源：http://adc.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://nfs.wangshuangyany.cn

Java: class User {}
来源：http://eov.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://wrq.hesvh.cn

Ruby: class User; end
来源：http://lig.gogol.net.cn

C#:   class User {}
来源：http://fcu.ctjpmb.com

[G02] 构造函数
来源：http://vha.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://iwo.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://jld.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://prj.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://pcn.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://ivw.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vlb.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://uxc.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://ltv.jqgfzy.top

[G03] 实例属性
来源：http://glu.hnxiangtu.top

Py:   self.name = "x"
来源：http://tnw.hcnkem.com

PHP:  public string $name = "x";
来源：http://lth.fktsv.cn

JS:   this.name = "x";
来源：http://yha.zhiwuduotai.top

TS:   name: string = "x";
来源：http://edl.gzhubu.top

Java: private String name;
来源：http://qbi.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://igq.iojbl.cn

Ruby: @name = "x"
来源：http://xby.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://awm.gogol.net.cn

[G04] 定义方法
来源：http://oox.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://kiu.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://bsc.tanke756.top

JS:   greet() { return this.name; }
来源：http://svl.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://kzr.tian-w.cn

Java: String greet() { return name; }
来源：http://ehy.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gwf.vehdjk.com

Ruby: def greet; @name; end
来源：http://uxw.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://jno.nwbrower.top

[G05] 继承
来源：http://xwm.tarul.cn

Py:   class Admin(User): pass
来源：http://wgu.hywenlv.cn

PHP:  class Admin extends User {}
来源：http://fsn.fktsv.cn

JS:   class Admin extends User {}
来源：http://jjz.epnwcf.com

TS:   class Admin extends User {}
来源：http://yvy.chenzaomai.com

Java: class Admin extends User {}
来源：http://xhn.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kiq.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://anh.hnxiangtu.top

C#:   class Admin : User {}
来源：http://ynk.hnqzz.top

[G06] 重写方法
来源：http://mfg.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://pje.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zxz.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://tqc.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://unv.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://twa.sweek.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://agc.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://smn.svipenyu.cn

C#:   public override string Greet() => "admin";
来源：http://vtq.jinqigufen.top

[G07] 调用父类方法
来源：http://oev.pengpengdd.cyou

Py:   super().greet()
来源：http://idi.wangdashe.top

PHP:  parent::greet();
来源：http://eas.ydjk.org.cn

JS:   super.greet();
来源：http://tsf.jianghu66.top

TS:   super.greet();
来源：http://emp.yongpay.top

Java: super.greet();
来源：http://zrg.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://smu.tianlin.xyz

Ruby: super
来源：http://obh.gotoacloud.top

C#:   base.Greet();
来源：http://ylt.aizwys.cn

[G08] 静态方法与属性
来源：http://pvu.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lrv.yuanzhike.top

PHP:  public static function f() {}
来源：http://wkr.wangdashe.top

JS:   static f() {}
来源：http://mbb.daria6918.cn

TS:   static f(): void {}
来源：http://qhg.ydzc1.top

Java: static void f() {}
来源：http://hqw.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gzn.smart0.xyz

Ruby: def self.f; end
来源：http://pxo.sysykeji.top

C#:   public static void F() {}
来源：http://fnb.cashguo.top

[G09] 接口 / 抽象类
来源：http://vlu.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://hnc.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://rvp.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xho.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://gxu.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://gbm.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://baq.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hov.haohaochexian.top

C#:   interface IShape { double Area(); }
来源：http://itq.wangdashe.top

[G10] 访问控制
来源：http://ula.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://wqt.bbcook.cn

PHP:  public / protected / private
来源：http://dmc.xinyue.icu

JS:   #private 字段；其余公开
来源：http://hzd.sufxvd.cn

TS:   public / protected / private
来源：http://omi.nanxinkj.top

Java: public / protected / private / 默认包级
来源：http://rre.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://avk.sysykeji.top

Ruby: public / protected / private
来源：http://peb.iojbl.cn

C#:   public / protected / private / internal
来源：http://bnl.shzxlz.cn

[G11] getter / setter
来源：http://ocp.yonumen.top

Py:   @property 与 @x.setter
来源：http://vwu.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xnw.ywan-chungtsiang.top

JS:   get name() { return this._name; }
来源：http://xnz.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://fdq.xylfe.cn

Java: public String getName() { return name; }
来源：http://alr.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://crn.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://yho.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://vro.cdnleiting.top

[G12] 对象转字符串
来源：http://wrg.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://tiq.xylfe.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://trk.hesvh.cn

JS:   toString() { return this.name; }
来源：http://tvk.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://bgs.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://trp.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://hmn.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://goz.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://knn.cashguo.top

[G13] 判断对象类型
来源：http://ujg.iojbl.cn

Py:   isinstance(u, User)
来源：http://jud.gogol.net.cn

PHP:  $u instanceof User
来源：http://uqs.xinyue.icu

JS:   u instanceof User
来源：http://fbu.yuanzhike.top

TS:   u instanceof User
来源：http://gsj.zhaomingkeji.xyz

Java: u instanceof User
来源：http://tpe.chenzaomai.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://vol.daxiang520.top

Ruby: u.is_a?(User)
来源：http://rxz.svipenyu.cn

C#:   u is User
来源：http://ggg.hesvh.cn

[G14] 数据类 / record
来源：http://mft.sxryk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jtc.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://qjf.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://hsk.meibo888.top

TS:   type User = { name: string; age: number };
来源：http://mnm.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://cux.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://pob.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ror.nanxinkj.top

C#:   record User(string Name, int Age);
来源：http://tyv.jinqigfzy.top

[G15] 枚举
来源：http://gka.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bqq.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sse.hfpthk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jzv.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rfa.iojbl.cn

Java: enum Color { RED, GREEN }
来源：http://gyv.jinqigufen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ubz.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://swi.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hyo.cheryme.top

[G16] 对象转数组 / 字典
来源：http://dlj.jiagoushi.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsl.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://rje.cheryme.top

JS:   Object.entries(obj)
来源：http://wmj.xziqi.cn

TS:   Object.entries(obj)
来源：http://cze.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mjf.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://txv.hywenlv.cn

Ruby: obj.instance_variables
来源：http://drw.xuetiantiany.cn

C#:   // 用反射或 System.Text.Json
来源：http://zri.hcnkem.com

================================================================================
来源：http://czy.iojbl.cn

H. 异常与错误处理
来源：http://tsx.jlsjyb.cn

================================================================================
来源：http://ugx.mhx1999.top

[H01] try / catch 基础
来源：http://zne.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nak.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zkp.ywan-chungtsiang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tmg.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ulx.yj20258.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sdk.jyoumei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mbp.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zpy.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rfw.sjlbkw.cn

[H02] finally / ensure 收尾
来源：http://glw.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://kdc.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dtq.yangfankeji.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ppc.chenjidiqi.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://xhv.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://pxf.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xse.epnwcf.com

Ruby: begin; f; ensure; cleanup; end
来源：http://gdx.shanyushiyangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gqp.jinyuanbaomall.cn


<!-- 参考信息 -->