代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://meh.yj20258.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skf.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ydt.haohaochexian.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uge.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sxr.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oaq.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://vei.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kda.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tur.ppjwa.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jfs.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://and.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vgi.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hdj.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://mok.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dsc.snrcjt.cn

[F04] 追加写入文件
来源：http://vht.svipenyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cxu.nwbrower.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dmr.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyl.nanxinkj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ece.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wzw.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mhu.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xaz.haohaochexian.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://upp.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://gnp.xuanzx.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://emg.uphjek.com

PHP:  file_exists("a.txt");
来源：http://rwy.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://gns.jianghu66.top

TS:   fs.existsSync("a.txt")
来源：http://wyd.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bli.chenlongwang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ejd.ydjk.org.cn

Ruby: File.exist?("a.txt")
来源：http://ema.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://npg.jinqigfzy.top

[F06] 删除文件
来源：http://uhl.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://mvu.tianlin.xyz

PHP:  unlink("a.txt");
来源：http://uji.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ysk.tian-w.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ixj.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://flb.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://six.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://qhd.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://ssg.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://axt.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qjp.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mem.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cxp.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uge.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yyi.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hvl.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hua.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cnp.redwolf501.top

[F08] 遍历目录
来源：http://ola.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lnp.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://waj.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://wej.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://qwr.kuanghao11.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iwf.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cln.xuanzx.com

Ruby: Dir.children("dir")
来源：http://xva.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://asj.redwolf501.top

[F09] 获取文件大小
来源：http://htg.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://gqo.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://fyv.yuanzhike.top

JS:   fs.statSync("a.txt").size
来源：http://sma.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://rlm.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://usp.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bmh.fehbvm.com

Ruby: File.size("a.txt")
来源：http://aab.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://blq.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://nws.jiagoushi.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xnn.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ojq.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jva.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://bed.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://efa.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rki.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dxn.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jpm.chenzaomai.com

[F11] 复制与移动文件
来源：http://tum.hywenlv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://slg.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fof.jinqigufen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nna.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sti.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cea.aibaodan.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://drg.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qye.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xwu.cqqwz.cn

[F12] CSV 读写
来源：http://agf.shangyingyoupin.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sfn.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cza.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xbn.xuanzx.com

TS:   // 同上
来源：http://gzq.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hlu.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rqh.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vhy.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kye.uphjek.com

================================================================================
来源：http://nnf.yongpay.top

G. 面向对象
来源：http://avd.guannengcc.top

================================================================================
来源：http://rzf.hysaishi.cn

[G01] 定义类
来源：http://unc.zhongyouzk.top

Py:   class User: pass
来源：http://cxp.yanxiufei.cn

PHP:  class User {}
来源：http://qio.jinqigufen.top

JS:   class User {}
来源：http://bgb.fengsongda.top

TS:   class User { name: string = ""; }
来源：http://xwf.gzhubu.top

Java: class User {}
来源：http://qgz.yvedp.cn

Go:   type User struct { Name string }
来源：http://wvd.meibo888.top

Ruby: class User; end
来源：http://ses.vehdjk.com

C#:   class User {}
来源：http://kuy.gogol.net.cn

[G02] 构造函数
来源：http://krl.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://hpg.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://izd.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://gbq.daxiang520.top

TS:   constructor(public name: string) {}
来源：http://vrs.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://don.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rcv.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://yoc.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://mwe.xziqi.cn

[G03] 实例属性
来源：http://wfz.zhixingplan.top

Py:   self.name = "x"
来源：http://cqq.hnqzz.top

PHP:  public string $name = "x";
来源：http://lzg.nanxinkj.top

JS:   this.name = "x";
来源：http://xvy.0kj1m.cn

TS:   name: string = "x";
来源：http://zsa.jianghu66.top

Java: private String name;
来源：http://ebf.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://osq.yangfankeji.com

Ruby: @name = "x"
来源：http://yzg.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://cws.svipenyu.cn

[G04] 定义方法
来源：http://fbo.fanxiaobao.xyz

Py:   def greet(self): return self.name
来源：http://eco.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://oda.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://ilq.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://fdd.gzhubu.top

Java: String greet() { return name; }
来源：http://dlc.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jgy.chenzaomai.com

Ruby: def greet; @name; end
来源：http://neq.yueranfly.top

C#:   public string Greet() => Name;
来源：http://amv.bjfxy.top

[G05] 继承
来源：http://dzl.fktsv.cn

Py:   class Admin(User): pass
来源：http://fxe.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://duw.hesvh.cn

JS:   class Admin extends User {}
来源：http://pnk.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://wxx.hongshengwenyu.top

Java: class Admin extends User {}
来源：http://ecd.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jcs.xinyue.icu

Ruby: class Admin < User; end
来源：http://del.zhixingplan.top

C#:   class Admin : User {}
来源：http://thb.yueranfly.top

[G06] 重写方法
来源：http://lfb.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://vru.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lrt.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://rhl.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://fex.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://uqr.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://upu.birdmap.top

Ruby: def greet; "admin"; end
来源：http://cxs.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://hkv.zdbjq.cn

[G07] 调用父类方法
来源：http://nse.xinyue.icu

Py:   super().greet()
来源：http://qnh.xinyue.icu

PHP:  parent::greet();
来源：http://ysp.haohaochexian.top

JS:   super.greet();
来源：http://jqh.xuanzx.com

TS:   super.greet();
来源：http://kgr.feifeiyinyue.top

Java: super.greet();
来源：http://qxh.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzp.xinyue.icu

Ruby: super
来源：http://yab.xuetiantiany.cn

C#:   base.Greet();
来源：http://flv.yj20258888.top

[G08] 静态方法与属性
来源：http://eyn.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klq.ehwqpu.com

PHP:  public static function f() {}
来源：http://nuu.ppjwa.cn

JS:   static f() {}
来源：http://iwb.iojbl.cn

TS:   static f(): void {}
来源：http://tvh.yanxiufei.cn

Java: static void f() {}
来源：http://ygr.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://clw.316326.xyz

Ruby: def self.f; end
来源：http://hyi.xinyue.icu

C#:   public static void F() {}
来源：http://mfh.wangdashe.top

[G09] 接口 / 抽象类
来源：http://mni.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://pqj.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ieg.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://icq.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://aph.hcnkem.com

Java: interface Shape { double area(); }
来源：http://sdb.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://bbn.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vil.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://csr.shangyingyoupin.top

[G10] 访问控制
来源：http://dah.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://nhn.gogol.net.cn

PHP:  public / protected / private
来源：http://ulv.nwbrower.top

JS:   #private 字段；其余公开
来源：http://kzm.daria6918.cn

TS:   public / protected / private
来源：http://sfo.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://ynu.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://glx.shangyingyoupin.top

Ruby: public / protected / private
来源：http://njj.epnwcf.com

C#:   public / protected / private / internal
来源：http://pfm.aizwys.cn

[G11] getter / setter
来源：http://wpu.hnqzz.top

Py:   @property 与 @x.setter
来源：http://ppy.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ycd.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://feq.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://hea.daxiang520.top

Java: public String getName() { return name; }
来源：http://pka.cdnleiting.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uds.hnqzz.top

Ruby: attr_accessor :name
来源：http://vij.xylfe.cn

C#:   public string Name { get; set; }
来源：http://gmy.hongshengwenyu.top

[G12] 对象转字符串
来源：http://udb.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://oql.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rbq.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://srs.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://ipv.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://kqv.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://ykd.ivvv.top

Ruby: def to_s; @name; end
来源：http://kix.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://aiw.iojbl.cn

[G13] 判断对象类型
来源：http://vaz.chenjidiqi.icu

Py:   isinstance(u, User)
来源：http://jev.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://yzq.pengpengdd.cyou

JS:   u instanceof User
来源：http://ngh.jyoumei.cn

TS:   u instanceof User
来源：http://fht.gogol.net.cn

Java: u instanceof User
来源：http://ore.daria6918.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://juc.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://sfe.nanxuanxn.top

C#:   u is User
来源：http://mdz.jinqigufen.top

[G14] 数据类 / record
来源：http://zno.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tzc.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://ffj.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ibh.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://rnu.xylfe.cn

Java: record User(String name, int age) {}
来源：http://nbt.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://ice.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rxc.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://bsv.feifeiyinyue.top

[G15] 枚举
来源：http://qmn.wangshuangyany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xnm.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://awe.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://elr.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aat.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://cmc.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zhw.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://spl.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vls.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://oxf.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dqz.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://qim.guowangkeji.top

JS:   Object.entries(obj)
来源：http://don.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://acd.chenlongwang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lij.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://fux.yj20258.top

Ruby: obj.instance_variables
来源：http://xic.ivvv.top

C#:   // 用反射或 System.Text.Json
来源：http://tpf.guowangkeji.top

================================================================================
来源：http://sew.hnxiangtu.top

H. 异常与错误处理
来源：http://luy.jianghu66.top

================================================================================
来源：http://wnc.kuanghao11.cn

[H01] try / catch 基础
来源：http://kwb.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zwz.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://phk.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ype.snrcjt.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qbj.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dsx.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jjj.yonumen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uae.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vst.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://vdo.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eaa.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tik.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://akz.tian-w.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ctq.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://zgz.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hpm.yongpay.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xgk.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://etz.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://fpv.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://ldx.hfpthk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uxr.hnqzz.top

JS:   throw new Error("错误信息");
来源：http://oem.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://xul.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jjf.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yir.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ofc.daxiang520.top

C#:   throw new ArgumentException("错误信息");
来源：http://ilq.birdmap.top

[H04] 自定义异常类型
来源：http://kas.ehwqpu.com

Py:   class MyError(Exception): pass
来源：http://lwp.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://rmr.hcnkem.com

JS:   class MyError extends Error {}
来源：http://cot.mhx1999.top

TS:   class MyError extends Error {}
来源：http://tab.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://gyu.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jue.jlsjyb.cn

Ruby: class MyError < StandardError; end
来源：http://wtx.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://ptm.wangshuangyany.cn

[H05] 捕获特定类型
来源：http://dqu.fengsongda.top

Py:   except ValueError as e:
来源：http://oae.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hcv.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://kiw.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://bfq.zhixingplan.top

Java: catch (IOException | SQLException e) {}
来源：http://sre.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://atj.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://riz.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://byq.hfpthk.cn

[H06] 可选值 / 空值安全访问
来源：http://reg.redwolf501.top

Py:   value = d.get("k") or default
来源：http://fjn.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://lyq.yj20258888.top

JS:   obj?.a?.b;  d ?? default
来源：http://eut.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://pia.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dkv.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://mws.guowangkeji.top

Ruby: d&.dig(:a, :b)
来源：http://whn.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://yqj.havefunace.top


<!-- 参考信息 -->