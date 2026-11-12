代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fsh.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nry.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ygi.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sld.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lno.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lgs.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://vvo.yanxiufei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://say.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kkl.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztt.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pit.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eym.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qxf.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://mnl.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yhp.yueranfly.top

[F04] 追加写入文件
来源：http://gny.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://skb.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ihm.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vic.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wad.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ngc.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ywa.shzxlz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://stv.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hkk.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://zhz.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kjj.chenzaomai.com

PHP:  file_exists("a.txt");
来源：http://hll.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://mkt.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://kbs.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wad.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://til.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://uxq.cheryme.top

C#:   File.Exists("a.txt")
来源：http://uje.xuanzx.com

[F06] 删除文件
来源：http://jxg.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://lqc.hnqzz.top

PHP:  unlink("a.txt");
来源：http://aws.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://ksy.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://gnl.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vqr.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://pvn.havefunace.top

Ruby: File.delete("a.txt")
来源：http://jpy.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://ual.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://cib.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://emz.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ljk.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbh.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hvg.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alf.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gfb.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cks.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://byp.tarul.cn

[F08] 遍历目录
来源：http://poi.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qwi.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mwx.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://hzs.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://jof.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fdg.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://smj.fktsv.cn

Ruby: Dir.children("dir")
来源：http://zay.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://oeq.yongpay.top

[F09] 获取文件大小
来源：http://pvb.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://krz.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://jab.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://tff.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://blh.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://jwy.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pwy.meibo888.top

Ruby: File.size("a.txt")
来源：http://xjt.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://vpk.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://tgk.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://usg.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zms.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jbw.andypj.xyz

TS:   path.extname("a.txt")
来源：http://tyn.birdmap.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sow.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qjo.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gva.nwbrower.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ifo.guowangkeji.top

[F11] 复制与移动文件
来源：http://soa.sufxvd.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nnw.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pnm.yongpay.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etp.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktu.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oei.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://joz.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tzh.wangdashe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://icb.ivvv.top

[F12] CSV 读写
来源：http://lyh.chenzaomai.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kut.ppjwa.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nxw.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vtl.cqqwz.cn

TS:   // 同上
来源：http://aha.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yoy.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ybz.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jkf.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lxy.hysaishi.cn

================================================================================
来源：http://xcm.snrcjt.cn

G. 面向对象
来源：http://ekp.redwolf501.top

================================================================================
来源：http://may.havefunace.top

[G01] 定义类
来源：http://njd.hfpthk.cn

Py:   class User: pass
来源：http://kwm.tarul.cn

PHP:  class User {}
来源：http://zuw.epnwcf.com

JS:   class User {}
来源：http://fou.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://ypz.jqgufenzy.top

Java: class User {}
来源：http://ehe.c1oappe.top

Go:   type User struct { Name string }
来源：http://cdi.ivvv.top

Ruby: class User; end
来源：http://hjy.smart0.xyz

C#:   class User {}
来源：http://uzi.svipenyu.cn

[G02] 构造函数
来源：http://eoe.smart0.xyz

Py:   def __init__(self, name): self.name = name
来源：http://yon.shanyushiyangtech.top

PHP:  public function __construct(public string $name) {}
来源：http://pij.ybcxt.top

JS:   constructor(name) { this.name = name; }
来源：http://unq.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://bwq.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://fih.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qtx.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://pjd.cashguo.top

C#:   public User(string name) { Name = name; }
来源：http://who.jiagoushi.top

[G03] 实例属性
来源：http://gwk.gzhubu.top

Py:   self.name = "x"
来源：http://guc.9152youxi.cn

PHP:  public string $name = "x";
来源：http://njo.daxiang520.top

JS:   this.name = "x";
来源：http://wst.sxryk.cn

TS:   name: string = "x";
来源：http://puf.yonumen.top

Java: private String name;
来源：http://ioi.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vxt.shuidangran.top

Ruby: @name = "x"
来源：http://vhd.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://dte.yangfankeji.com

[G04] 定义方法
来源：http://cig.daria6918.cn

Py:   def greet(self): return self.name
来源：http://oaf.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vai.cashguo.top

JS:   greet() { return this.name; }
来源：http://kri.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://wuu.andypj.xyz

Java: String greet() { return name; }
来源：http://esp.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ilm.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://iip.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://dil.mhx1999.top

[G05] 继承
来源：http://hlk.xuanzx.com

Py:   class Admin(User): pass
来源：http://lxb.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://xwo.redwolf501.top

JS:   class Admin extends User {}
来源：http://lzx.guowangkeji.top

TS:   class Admin extends User {}
来源：http://zkt.gzhubu.top

Java: class Admin extends User {}
来源：http://lbi.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eor.0kj1m.cn

Ruby: class Admin < User; end
来源：http://zub.gzhubu.top

C#:   class Admin : User {}
来源：http://vje.hcnkem.com

[G06] 重写方法
来源：http://vcm.hongshengwenyu.top

Py:   def greet(self): return "admin"
来源：http://lmf.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://smh.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://gdc.yj202588.top

TS:   greet(): string { return "admin"; }
来源：http://aqu.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://gto.bbcook.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vxz.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://xrw.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://xve.yonumen.top

[G07] 调用父类方法
来源：http://onf.shanyushiyangkeji.top

Py:   super().greet()
来源：http://tgr.jiagoushi.top

PHP:  parent::greet();
来源：http://dxm.hywenlv.cn

JS:   super.greet();
来源：http://kse.jianghu66.top

TS:   super.greet();
来源：http://sqj.jinqigfzy.top

Java: super.greet();
来源：http://kaj.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jkc.jiagoushi.top

Ruby: super
来源：http://awl.ehwqpu.com

C#:   base.Greet();
来源：http://btn.svipenyu.cn

[G08] 静态方法与属性
来源：http://kqg.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://foi.9152youxi.cn

PHP:  public static function f() {}
来源：http://zbm.mhx1999.top

JS:   static f() {}
来源：http://hnh.tanke756.top

TS:   static f(): void {}
来源：http://joh.zhoulong.xyz

Java: static void f() {}
来源：http://dcn.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://mpv.ivvv.top

Ruby: def self.f; end
来源：http://bpq.chenlongwang.top

C#:   public static void F() {}
来源：http://ivo.ybcxt.top

[G09] 接口 / 抽象类
来源：http://fiy.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://lfn.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hqi.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oaw.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://biv.yj20258.top

Java: interface Shape { double area(); }
来源：http://ttn.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://osk.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kel.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://ttl.zhixingplan.top

[G10] 访问控制
来源：http://fow.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://war.tian-w.cn

PHP:  public / protected / private
来源：http://vaz.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://vav.cashguo.top

TS:   public / protected / private
来源：http://tkg.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://uzu.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gdd.cheryme.top

Ruby: public / protected / private
来源：http://egh.zhengqikj.top

C#:   public / protected / private / internal
来源：http://noq.nanxuanxn.top

[G11] getter / setter
来源：http://lfj.andypj.xyz

Py:   @property 与 @x.setter
来源：http://luu.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kel.epnwcf.com

JS:   get name() { return this._name; }
来源：http://ljz.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://jxq.0kj1m.cn

Java: public String getName() { return name; }
来源：http://nnz.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lio.cucudq.cn

Ruby: attr_accessor :name
来源：http://xed.iojbl.cn

C#:   public string Name { get; set; }
来源：http://swi.xuetiantiany.cn

[G12] 对象转字符串
来源：http://thn.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://cmr.pycfn.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://tvh.hesvh.cn

JS:   toString() { return this.name; }
来源：http://gnh.sweek.top

TS:   toString(): string { return this.name; }
来源：http://ycz.fktsv.cn

Java: @Override public String toString() { return name; }
来源：http://meg.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://btb.daria6918.cn

Ruby: def to_s; @name; end
来源：http://zdo.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://cqu.hfpthk.cn

[G13] 判断对象类型
来源：http://jyl.cheryme.top

Py:   isinstance(u, User)
来源：http://esb.zdbjq.cn

PHP:  $u instanceof User
来源：http://oui.iojbl.cn

JS:   u instanceof User
来源：http://zrx.cashguo.top

TS:   u instanceof User
来源：http://coz.ctjpmb.com

Java: u instanceof User
来源：http://wbd.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sdh.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://kcp.yueranfly.top

C#:   u is User
来源：http://nda.tian-w.cn

[G14] 数据类 / record
来源：http://qbo.andypj.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mro.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://lds.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ftd.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://tzz.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://ars.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://ktc.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mrj.wangshuangyany.cn

C#:   record User(string Name, int Age);
来源：http://kxz.ppjwa.cn

[G15] 枚举
来源：http://ecc.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kax.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bfw.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tic.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tle.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://jxs.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rbn.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://vzd.iojbl.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tgx.9152youxi.cn

[G16] 对象转数组 / 字典
来源：http://rge.ivvv.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yye.xuanzx.com

PHP:  get_object_vars($obj);
来源：http://mjr.svipenyu.cn

JS:   Object.entries(obj)
来源：http://wjq.hammf.cn

TS:   Object.entries(obj)
来源：http://zst.yj202588.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mci.yj20258888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nyg.fehbvm.com

Ruby: obj.instance_variables
来源：http://zxm.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://fen.9152youxi.cn

================================================================================
来源：http://mzs.yueranfly.top

H. 异常与错误处理
来源：http://ugz.zhixingplan.top

================================================================================
来源：http://hpe.fanxiaobao.xyz

[H01] try / catch 基础
来源：http://koy.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aql.snrcjt.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://imu.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lqh.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kpg.xziqi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nyj.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://law.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mvq.jlsjyb.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xwj.gzhubu.top

[H02] finally / ensure 收尾
来源：http://ppj.tian-w.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iaf.yuanzhike.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://bxy.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://out.ywan-chungtsiang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://unl.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://thz.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ssv.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ptx.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jbw.yvedp.cn

[H03] 主动抛出异常
来源：http://jju.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://gmm.tarul.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vhq.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://aca.epnwcf.com

TS:   throw new Error("错误信息");
来源：http://spo.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fff.sxryk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dwu.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ioi.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://nxo.ybcxt.top

[H04] 自定义异常类型
来源：http://fnd.sweek.top

Py:   class MyError(Exception): pass
来源：http://lwj.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://jdn.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://rov.uphjek.com

TS:   class MyError extends Error {}
来源：http://jzq.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://euu.yanxiufei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pmr.0kj1m.cn

Ruby: class MyError < StandardError; end
来源：http://qjj.aizwys.cn

C#:   class MyException : Exception {}
来源：http://yfl.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://hly.xylfe.cn

Py:   except ValueError as e:
来源：http://aii.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhq.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://yau.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://dfx.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://igl.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bpu.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://elt.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hhv.cdnleiting.top

[H06] 可选值 / 空值安全访问
来源：http://vay.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://ige.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ptt.bjfxy.top

JS:   obj?.a?.b;  d ?? default
来源：http://nta.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://wqx.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rbn.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kms.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://dnm.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://urw.shanyushiyangkeji.top


<!-- 参考信息 -->