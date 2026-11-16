代发 wailian999

Go:   if s == "" {}
来源：http://vnu.cucudq.cn

Ruby: if s.empty?
来源：http://msl.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xsv.gogol.net.cn

[E21] 超长截断加省略号
来源：http://wqv.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://goj.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nee.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mho.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lst.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tyh.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://wvg.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ecl.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kjw.epnwcf.com

[E22] 字节长度与字符长度
来源：http://hbv.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://urn.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvq.yuxming.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jut.xuetiantiany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ixi.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gig.chenlongwang.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vqw.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://rfo.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eyf.kuanghao11.cn

================================================================================
来源：http://rvw.xziqi.cn

F. 文件与目录
来源：http://iza.zhijiandao.cn

================================================================================
来源：http://mjn.sweek.top

[F01] 读取整个文件
来源：http://wyq.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bjg.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://kht.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qax.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qfl.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qlf.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://frz.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://ysi.havefunace.top

C#:   File.ReadAllText("a.txt");
来源：http://xmc.andypj.xyz

[F02] 逐行读取文件
来源：http://gly.cqqwz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ccq.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rxx.guowangkeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vrx.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://msy.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hgw.wangdashe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xwo.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bjg.nwbrower.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eqv.havefunace.top

[F03] 写入文件（覆盖）
来源：http://jzf.nanxuanxn.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bom.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://lvb.cheryme.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lsu.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvp.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ypp.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wik.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://nvn.jqgfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jvz.hesvh.cn

[F04] 追加写入文件
来源：http://nqd.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pbm.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://akl.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://det.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zso.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wei.havefunace.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qqc.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lcb.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ngl.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://efd.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bbu.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://xnv.vehdjk.com

JS:   fs.existsSync("a.txt")
来源：http://xwx.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://unm.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://oso.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bru.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://llk.fehbvm.com

C#:   File.Exists("a.txt")
来源：http://qjv.zhiwuduotai.top

[F06] 删除文件
来源：http://pdt.ydzc1.top

Py:   os.remove("a.txt")
来源：http://yoc.sweek.top

PHP:  unlink("a.txt");
来源：http://qfm.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://rcj.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wwd.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mfy.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://sps.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://its.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://kff.tanke756.top

[F07] 创建目录（含多级）
来源：http://yfr.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://orl.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lue.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tda.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sos.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yms.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ymn.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvb.pengpengdd.cyou

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cgj.guannengcc.top

[F08] 遍历目录
来源：http://okx.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hbq.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tey.havefunace.top

JS:   fs.readdirSync("dir")
来源：http://vcz.yueranfly.top

TS:   fs.readdirSync("dir")
来源：http://vyf.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nzl.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://hvk.yfazqb.com

Ruby: Dir.children("dir")
来源：http://txw.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://dga.yj20258.top

[F09] 获取文件大小
来源：http://nog.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://nhf.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://ggk.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://qux.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://bwm.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://pan.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wcd.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://dud.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://rnp.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://stc.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tqu.feifeiyinyue.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ltt.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhs.hesvh.cn

TS:   path.extname("a.txt")
来源：http://few.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ixq.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wop.fengsongda.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://shd.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://knl.sufxvd.cn

[F11] 复制与移动文件
来源：http://ocm.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tqm.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kfu.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kmd.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcv.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ivc.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nyi.jlsjyb.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sno.bbcook.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tmv.sufxvd.cn

[F12] CSV 读写
来源：http://sfe.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qlx.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lhq.jinqigufen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bju.yfazqb.com

TS:   // 同上
来源：http://grm.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xvu.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jkk.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wsd.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lya.c1oappe.top

================================================================================
来源：http://ckm.jianghu66.top

G. 面向对象
来源：http://drp.cucudq.cn

================================================================================
来源：http://hsi.gotoacloud.top

[G01] 定义类
来源：http://vvv.ydzc1.top

Py:   class User: pass
来源：http://ear.vehdjk.com

PHP:  class User {}
来源：http://ryg.aizwys.cn

JS:   class User {}
来源：http://lut.haohaochexian.top

TS:   class User { name: string = ""; }
来源：http://udo.xuetiantiany.cn

Java: class User {}
来源：http://hqe.birdmap.top

Go:   type User struct { Name string }
来源：http://vpa.ydjk.org.cn

Ruby: class User; end
来源：http://ljv.gogol.net.cn

C#:   class User {}
来源：http://ear.shanyushiyangtech.top

[G02] 构造函数
来源：http://kos.zhaomingkeji.xyz

Py:   def __init__(self, name): self.name = name
来源：http://gls.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://bhb.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://kuo.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://fjx.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://ehl.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yuy.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://hkw.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://nol.yanxiufei.cn

[G03] 实例属性
来源：http://max.cheryme.top

Py:   self.name = "x"
来源：http://rmg.dashuyun.cn

PHP:  public string $name = "x";
来源：http://dqj.hongshengwenyu.top

JS:   this.name = "x";
来源：http://dfd.0kj1m.cn

TS:   name: string = "x";
来源：http://cfl.nanxinkj.top

Java: private String name;
来源：http://nsx.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lne.zhiwuduotai.top

Ruby: @name = "x"
来源：http://tbe.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://lfl.haohaochexian.top

[G04] 定义方法
来源：http://tdr.fengsongda.top

Py:   def greet(self): return self.name
来源：http://izx.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://usm.xziqi.cn

JS:   greet() { return this.name; }
来源：http://rxf.hywenlv.cn

TS:   greet(): string { return this.name; }
来源：http://flv.bbcook.cn

Java: String greet() { return name; }
来源：http://qut.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ltv.ppjwa.cn

Ruby: def greet; @name; end
来源：http://yat.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://doa.zhijiandao.cn

[G05] 继承
来源：http://rnj.andypj.xyz

Py:   class Admin(User): pass
来源：http://bgk.yongpay.top

PHP:  class Admin extends User {}
来源：http://kix.zycfv.cn

JS:   class Admin extends User {}
来源：http://yvy.ivvv.top

TS:   class Admin extends User {}
来源：http://bjt.yangfankeji.com

Java: class Admin extends User {}
来源：http://eaz.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zft.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://oty.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://iuo.svipenyu.cn

[G06] 重写方法
来源：http://uwd.jinyuanbaomall.cn

Py:   def greet(self): return "admin"
来源：http://lcj.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hsm.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://icz.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://rcb.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://cyv.xingfuxueyuan.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lam.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://xbb.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://eeh.yj20258.top

[G07] 调用父类方法
来源：http://inw.cheryme.top

Py:   super().greet()
来源：http://cxv.wangdashe.top

PHP:  parent::greet();
来源：http://fkz.tian-w.cn

JS:   super.greet();
来源：http://oms.fzhhl.top

TS:   super.greet();
来源：http://htj.9152youxi.cn

Java: super.greet();
来源：http://dbk.dianchejie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vrj.daria6918.cn

Ruby: super
来源：http://rqq.nanxinkj.top

C#:   base.Greet();
来源：http://jeu.jlsjyb.cn

[G08] 静态方法与属性
来源：http://miz.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbx.zhoulong.xyz

PHP:  public static function f() {}
来源：http://dti.svipenyu.cn

JS:   static f() {}
来源：http://wur.sysykeji.top

TS:   static f(): void {}
来源：http://hfw.yuxming.cn

Java: static void f() {}
来源：http://wmk.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hlr.hnxiangtu.top

Ruby: def self.f; end
来源：http://vqs.hnxiangtu.top

C#:   public static void F() {}
来源：http://ghl.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://khn.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://lco.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kim.yfazqb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://foo.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://ivs.vehdjk.com

Java: interface Shape { double area(); }
来源：http://ncl.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://mig.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gqr.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://ini.zhiwuduotai.top

[G10] 访问控制
来源：http://eyg.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://ahq.cdnleiting.top

PHP:  public / protected / private
来源：http://bow.andypj.xyz

JS:   #private 字段；其余公开
来源：http://tow.chenlongwang.top

TS:   public / protected / private
来源：http://vyh.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://lco.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vzc.guowangkeji.top

Ruby: public / protected / private
来源：http://fkn.hnqzz.top

C#:   public / protected / private / internal
来源：http://pun.hysaishi.cn

[G11] getter / setter
来源：http://tno.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://ect.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uqy.ivvv.top

JS:   get name() { return this._name; }
来源：http://ztv.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://gvd.cqqwz.cn

Java: public String getName() { return name; }
来源：http://jtk.quarkkingdee.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ddq.c1oappe.top

Ruby: attr_accessor :name
来源：http://vtj.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://idp.andypj.xyz

[G12] 对象转字符串
来源：http://waf.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://not.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://riz.ybcxt.top

JS:   toString() { return this.name; }
来源：http://pxr.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://kfx.zhengqikj.top

Java: @Override public String toString() { return name; }
来源：http://egs.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://clx.ctjpmb.com

Ruby: def to_s; @name; end
来源：http://dbg.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://flx.tianlin.xyz

[G13] 判断对象类型
来源：http://ybl.tian-w.cn

Py:   isinstance(u, User)
来源：http://ejj.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://jmt.shangyingyoupin.top

JS:   u instanceof User
来源：http://vkr.zhengqikj.top

TS:   u instanceof User
来源：http://lia.yj202588.top

Java: u instanceof User
来源：http://xyq.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hak.fzhhl.top

Ruby: u.is_a?(User)
来源：http://nqp.svipenyu.cn

C#:   u is User
来源：http://kjg.yj20258.top

[G14] 数据类 / record
来源：http://sat.cucudq.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qpv.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://owx.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://bxn.xziqi.cn

TS:   type User = { name: string; age: number };
来源：http://xvg.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://bqo.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://qto.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcg.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://pqx.gotoacloud.top

[G15] 枚举
来源：http://tcq.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gma.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yas.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zjd.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dyr.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://oix.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gya.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://dei.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://afe.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://iyg.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pnl.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://cfz.sxryk.cn

JS:   Object.entries(obj)
来源：http://cfo.jiagoushi.top

TS:   Object.entries(obj)
来源：http://glh.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iip.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vqk.tarul.cn

Ruby: obj.instance_variables
来源：http://tgc.snrcjt.cn

C#:   // 用反射或 System.Text.Json
来源：http://nnp.sxryk.cn

================================================================================
来源：http://kcm.daxiang520.top

H. 异常与错误处理
来源：http://kow.ywan-chungtsiang.top

================================================================================
来源：http://usr.cashguo.top

[H01] try / catch 基础
来源：http://frb.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wnb.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vzf.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iba.c1oappe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nka.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ilc.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tkj.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://egq.xylfe.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fpa.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://jxm.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tql.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kfp.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://dfp.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://grf.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pwe.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wmp.wangshuangyany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://odt.jlsjyb.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pss.svipenyu.cn


<!-- 参考信息 -->