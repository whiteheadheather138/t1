代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dst.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sfr.nwbrower.top

[F03] 写入文件（覆盖）
来源：http://xga.sxryk.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lns.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://eup.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ite.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yed.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rif.aizwys.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oyb.yueranfly.top

Ruby: File.write("a.txt", "hi")
来源：http://hec.hywenlv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qrr.jqgfzy.top

[F04] 追加写入文件
来源：http://ejm.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://umb.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dve.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kfj.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cvy.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tjf.smart0.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fss.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qgc.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://khc.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://hmp.cucudq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ixy.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://xfo.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://pdm.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://yok.uphjek.com

Java: Files.exists(Path.of("a.txt"))
来源：http://njr.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dqi.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://ywy.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://rzw.chenjidiqi.icu

[F06] 删除文件
来源：http://upn.sweek.top

Py:   os.remove("a.txt")
来源：http://fse.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://zrc.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://jmz.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://ubs.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://anj.dashuyun.cn

Go:   os.Remove("a.txt")
来源：http://dyk.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://bpf.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://mco.smart0.xyz

[F07] 创建目录（含多级）
来源：http://qcv.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fwa.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gjb.9152youxi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awy.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://csq.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cqd.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sph.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xhh.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://noy.shzxlz.cn

[F08] 遍历目录
来源：http://zru.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yan.smart0.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://plm.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://apq.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://nvi.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fpi.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tbz.tarul.cn

Ruby: Dir.children("dir")
来源：http://niv.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://bgb.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://kbn.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://qdk.xylfe.cn

PHP:  filesize("a.txt");
来源：http://bkg.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://aml.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://dyt.iojbl.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jzo.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjk.yangfankeji.com

Ruby: File.size("a.txt")
来源：http://bbo.chenlongwang.top

C#:   new FileInfo("a.txt").Length
来源：http://akx.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://erv.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ave.jqgfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zpk.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wta.sxryk.cn

TS:   path.extname("a.txt")
来源：http://wgz.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zxz.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tvz.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ppb.guowangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aia.cqqwz.cn

[F11] 复制与移动文件
来源：http://dsq.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gai.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uih.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://onm.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zll.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ava.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://foy.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mgx.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fub.birdmap.top

[F12] CSV 读写
来源：http://cym.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xfv.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rls.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kdn.zdbjq.cn

TS:   // 同上
来源：http://okv.52xcode.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mly.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qir.hcnkem.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yww.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dgw.jinqigfzy.top

================================================================================
来源：http://leb.316326.xyz

G. 面向对象
来源：http://uxg.zhengqikj.top

================================================================================
来源：http://hdo.shanyushiyangtech.top

[G01] 定义类
来源：http://vbi.jianghu66.top

Py:   class User: pass
来源：http://ylk.jyoumei.cn

PHP:  class User {}
来源：http://krb.mhx1999.top

JS:   class User {}
来源：http://axd.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://jmp.shangyingyoupin.top

Java: class User {}
来源：http://hvw.hesvh.cn

Go:   type User struct { Name string }
来源：http://bdr.yuanzhike.top

Ruby: class User; end
来源：http://yyj.zhoulong.xyz

C#:   class User {}
来源：http://tdz.ydjk.org.cn

[G02] 构造函数
来源：http://suq.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://itc.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://baf.zhaomingkeji.xyz

JS:   constructor(name) { this.name = name; }
来源：http://lur.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://qbs.shzxlz.cn

Java: User(String name) { this.name = name; }
来源：http://ulc.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ddo.vehdjk.com

Ruby: def initialize(name); @name = name; end
来源：http://tdc.pengpengdd.cyou

C#:   public User(string name) { Name = name; }
来源：http://rin.yonumen.top

[G03] 实例属性
来源：http://mnh.wangshuangyany.cn

Py:   self.name = "x"
来源：http://kcv.cheryme.top

PHP:  public string $name = "x";
来源：http://hmr.daria6918.cn

JS:   this.name = "x";
来源：http://puo.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://bxs.feifeiyinyue.top

Java: private String name;
来源：http://isa.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nfn.daxiang520.top

Ruby: @name = "x"
来源：http://ivn.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://zex.sxryk.cn

[G04] 定义方法
来源：http://peq.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://bin.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zce.yuanzhike.top

JS:   greet() { return this.name; }
来源：http://asc.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://dnn.fktsv.cn

Java: String greet() { return name; }
来源：http://kkg.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oem.havefunace.top

Ruby: def greet; @name; end
来源：http://zwb.xziqi.cn

C#:   public string Greet() => Name;
来源：http://jub.quarkkingdee.top

[G05] 继承
来源：http://jok.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://blg.vehdjk.com

PHP:  class Admin extends User {}
来源：http://jdh.tianlin.xyz

JS:   class Admin extends User {}
来源：http://eyo.zycfv.cn

TS:   class Admin extends User {}
来源：http://hjf.ctjpmb.com

Java: class Admin extends User {}
来源：http://dup.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qcr.jinqigufen.top

Ruby: class Admin < User; end
来源：http://zti.mhx1999.top

C#:   class Admin : User {}
来源：http://tye.vehdjk.com

[G06] 重写方法
来源：http://sfv.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://nqg.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nix.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://zhl.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://npw.jinyuanbaomall.cn

Java: @Override String greet() { return "admin"; }
来源：http://qya.aizwys.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://beu.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://cko.mhx1999.top

C#:   public override string Greet() => "admin";
来源：http://evj.cdnleiting.top

[G07] 调用父类方法
来源：http://lli.pycfn.com

Py:   super().greet()
来源：http://tpr.birdmap.top

PHP:  parent::greet();
来源：http://yfr.cqqwz.cn

JS:   super.greet();
来源：http://qbs.yuanzhike.top

TS:   super.greet();
来源：http://zfx.meibo888.top

Java: super.greet();
来源：http://gmk.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nan.vehdjk.com

Ruby: super
来源：http://hya.0kj1m.cn

C#:   base.Greet();
来源：http://ziy.vehdjk.com

[G08] 静态方法与属性
来源：http://dqo.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xup.zhongyouzk.top

PHP:  public static function f() {}
来源：http://abp.vehdjk.com

JS:   static f() {}
来源：http://ilx.gaohongyu789.top

TS:   static f(): void {}
来源：http://jpy.uphjek.com

Java: static void f() {}
来源：http://aks.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://byf.cucudq.cn

Ruby: def self.f; end
来源：http://ctx.yuxming.cn

C#:   public static void F() {}
来源：http://gua.hesvh.cn

[G09] 接口 / 抽象类
来源：http://ocg.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://rbh.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pht.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://trd.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://jfk.fengsongda.top

Java: interface Shape { double area(); }
来源：http://hbl.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://gqj.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tlh.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://wrn.ydzc1.top

[G10] 访问控制
来源：http://bka.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://wdc.guannengcc.top

PHP:  public / protected / private
来源：http://fcf.cashguo.top

JS:   #private 字段；其余公开
来源：http://rin.snrcjt.cn

TS:   public / protected / private
来源：http://lal.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://pbj.hammf.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jsz.smart0.xyz

Ruby: public / protected / private
来源：http://bea.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://edw.guannengcc.top

[G11] getter / setter
来源：http://bng.fzhhl.top

Py:   @property 与 @x.setter
来源：http://qso.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aro.cucudq.cn

JS:   get name() { return this._name; }
来源：http://rlz.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://ezu.gogol.net.cn

Java: public String getName() { return name; }
来源：http://bzg.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wrq.havefunace.top

Ruby: attr_accessor :name
来源：http://vnc.birdmap.top

C#:   public string Name { get; set; }
来源：http://lfj.ydjk.org.cn

[G12] 对象转字符串
来源：http://cnd.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://ffy.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kkk.fengsongda.top

JS:   toString() { return this.name; }
来源：http://qit.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://plq.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://ogz.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://lnt.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://yjz.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://nqw.tarul.cn

[G13] 判断对象类型
来源：http://lfe.chenlongwang.top

Py:   isinstance(u, User)
来源：http://nvo.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://zyb.fengsongda.top

JS:   u instanceof User
来源：http://wwl.chenjidiqi.icu

TS:   u instanceof User
来源：http://pru.xuanzx.com

Java: u instanceof User
来源：http://kox.xziqi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hvu.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://rjb.zhijiandao.cn

C#:   u is User
来源：http://swq.hcnkem.com

[G14] 数据类 / record
来源：http://bmc.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pig.fktsv.cn

PHP:  // 用 readonly 属性模拟
来源：http://hhd.tian-w.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dfl.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://vks.haohaochexian.top

Java: record User(String name, int age) {}
来源：http://ncg.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://rgw.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kgp.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://qxq.yongpay.top

[G15] 枚举
来源：http://zsd.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://duw.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://bad.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jyg.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bic.zdbjq.cn

Java: enum Color { RED, GREEN }
来源：http://xtn.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nbm.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://bgb.cucudq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ptr.pycfn.com

[G16] 对象转数组 / 字典
来源：http://iis.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fyf.pycfn.com

PHP:  get_object_vars($obj);
来源：http://mdx.cucudq.cn

JS:   Object.entries(obj)
来源：http://hks.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://oqw.zhiwuduotai.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hdu.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://naw.yj202588.top

Ruby: obj.instance_variables
来源：http://ezh.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://rhu.jianghu66.top

================================================================================
来源：http://ccj.kuanghao11.cn

H. 异常与错误处理
来源：http://ixz.ctjpmb.com

================================================================================
来源：http://uip.shangyingyoupin.top

[H01] try / catch 基础
来源：http://ygs.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rad.gzhubu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mvf.yonumen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jgg.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ydi.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jer.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oep.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qyv.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aba.yj20258888.top

[H02] finally / ensure 收尾
来源：http://mte.xingfuxueyuan.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://wrw.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://adi.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rbl.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rer.ctjpmb.com

Java: try { f(); } finally { cleanup(); }
来源：http://pmg.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nlm.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://nqz.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://csm.tianlin.xyz

[H03] 主动抛出异常
来源：http://znu.hnqzz.top

Py:   raise ValueError("错误信息")
来源：http://pvo.aizwys.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xsl.chenzaomai.com

JS:   throw new Error("错误信息");
来源：http://kpa.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://hho.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ewo.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mxi.hnqzz.top

Ruby: raise ArgumentError, "错误信息"
来源：http://iga.jyoumei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mnw.hesvh.cn

[H04] 自定义异常类型
来源：http://jqf.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://beq.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qkz.ppjwa.cn

JS:   class MyError extends Error {}
来源：http://vqi.mhx1999.top

TS:   class MyError extends Error {}
来源：http://ftx.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://crv.ppjwa.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gdh.hammf.cn

Ruby: class MyError < StandardError; end
来源：http://xmy.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://oiy.hnxiangtu.top

[H05] 捕获特定类型
来源：http://pui.9152youxi.cn

Py:   except ValueError as e:
来源：http://ydj.guannengcc.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://grf.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://dby.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://rjz.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://xeg.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bmy.aizwys.cn

Ruby: rescue ArgumentError => e
来源：http://luc.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gjf.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://hdj.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://smp.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://jgd.shzxlz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nzs.sysykeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://nii.hnqzz.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kcr.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qhf.316326.xyz

Ruby: d&.dig(:a, :b)
来源：http://ecx.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://mup.tanke756.top

[H07] 断言
来源：http://ugh.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://xip.316326.xyz

PHP:  assert($x > 0);
来源：http://mio.316326.xyz

JS:   console.assert(x > 0);
来源：http://qch.sysykeji.top


<!-- 参考信息 -->