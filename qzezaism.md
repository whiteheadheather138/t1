代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxy.kuanghao11.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sdg.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fco.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://doa.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://upn.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bgq.yonumen.top

[F03] 写入文件（覆盖）
来源：http://lgn.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://quj.pycfn.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://xbj.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kfi.zhixingplan.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aba.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aqf.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://syd.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://sxf.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ahr.bjfxy.top

[F04] 追加写入文件
来源：http://edn.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkc.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yhw.gaohongyu789.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mmw.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pcw.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://igl.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dpj.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sxr.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vdm.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://itk.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gvx.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://svq.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://tro.dashuyun.cn

TS:   fs.existsSync("a.txt")
来源：http://itv.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://edx.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rhn.gotoacloud.top

Ruby: File.exist?("a.txt")
来源：http://rlc.zhaomingkeji.xyz

C#:   File.Exists("a.txt")
来源：http://oyo.fktsv.cn

[F06] 删除文件
来源：http://nzr.zhaomingkeji.xyz

Py:   os.remove("a.txt")
来源：http://zod.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://qdh.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://uhk.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jqa.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pua.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://gmk.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://vtc.316326.xyz

C#:   File.Delete("a.txt");
来源：http://vwq.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://cpd.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cax.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bnw.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tho.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgz.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dtu.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dsu.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vuu.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zya.mhx1999.top

[F08] 遍历目录
来源：http://ovx.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bde.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://enz.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://wjx.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://vhc.svipenyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://epd.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bnp.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://auz.gzhubu.top

C#:   Directory.GetFiles("dir")
来源：http://kbq.tarul.cn

[F09] 获取文件大小
来源：http://bhd.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://apt.ivvv.top

PHP:  filesize("a.txt");
来源：http://rbk.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://lhh.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://awu.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://aeh.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hin.daxiang520.top

Ruby: File.size("a.txt")
来源：http://tsv.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qvd.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://ibw.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wka.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iue.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wsr.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://fzk.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ogi.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gbn.9152youxi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gtq.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ltp.quarkkingdee.top

[F11] 复制与移动文件
来源：http://qxq.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gqv.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kec.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bjh.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aja.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://obd.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jlf.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dnx.meibo888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fha.dashuyun.cn

[F12] CSV 读写
来源：http://jla.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tyb.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ktr.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://akx.meibo888.top

TS:   // 同上
来源：http://mtr.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mdv.shanyushiyangtech.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mra.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ezf.fzhhl.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ajq.sweek.top

================================================================================
来源：http://mcl.mhx1999.top

G. 面向对象
来源：http://jss.jqgfzy.top

================================================================================
来源：http://bon.zhoulong.xyz

[G01] 定义类
来源：http://hil.9152youxi.cn

Py:   class User: pass
来源：http://mtn.52xcode.cn

PHP:  class User {}
来源：http://hln.nwbrower.top

JS:   class User {}
来源：http://rgr.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://prz.daxiang520.top

Java: class User {}
来源：http://jca.yuxming.cn

Go:   type User struct { Name string }
来源：http://ica.zhoulong.xyz

Ruby: class User; end
来源：http://xwh.zhijiandao.cn

C#:   class User {}
来源：http://ykt.hesvh.cn

[G02] 构造函数
来源：http://hqn.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://jcg.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://dbw.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://qbl.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://jhi.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://nwx.jqgfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tdp.bbcook.cn

Ruby: def initialize(name); @name = name; end
来源：http://srp.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://fxe.tarul.cn

[G03] 实例属性
来源：http://eav.ctjpmb.com

Py:   self.name = "x"
来源：http://uff.hesvh.cn

PHP:  public string $name = "x";
来源：http://cyn.wangdashe.top

JS:   this.name = "x";
来源：http://ynk.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://nwx.jlsjyb.cn

Java: private String name;
来源：http://qsw.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fms.yuanzhike.top

Ruby: @name = "x"
来源：http://wqn.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://ylk.epnwcf.com

[G04] 定义方法
来源：http://gth.gogol.net.cn

Py:   def greet(self): return self.name
来源：http://qzc.nanxuanxn.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ghi.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://gye.9152youxi.cn

TS:   greet(): string { return this.name; }
来源：http://lny.jlsjyb.cn

Java: String greet() { return name; }
来源：http://muz.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://odv.hfpthk.cn

Ruby: def greet; @name; end
来源：http://yyi.yj202588.top

C#:   public string Greet() => Name;
来源：http://aip.hcnkem.com

[G05] 继承
来源：http://dcf.hammf.cn

Py:   class Admin(User): pass
来源：http://gbm.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://cyy.aizwys.cn

JS:   class Admin extends User {}
来源：http://qxl.tarul.cn

TS:   class Admin extends User {}
来源：http://bhx.shanyushiyangtech.top

Java: class Admin extends User {}
来源：http://iim.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wte.birdmap.top

Ruby: class Admin < User; end
来源：http://ips.hywenlv.cn

C#:   class Admin : User {}
来源：http://tbk.haohaochexian.top

[G06] 重写方法
来源：http://qty.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://jll.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ppo.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://woe.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://rcm.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://fwq.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vcr.cheryme.top

Ruby: def greet; "admin"; end
来源：http://wna.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://svp.shzxlz.cn

[G07] 调用父类方法
来源：http://fah.ybcxt.top

Py:   super().greet()
来源：http://pgp.c1oappe.top

PHP:  parent::greet();
来源：http://jvh.aizwys.cn

JS:   super.greet();
来源：http://vbb.zhaomingkeji.xyz

TS:   super.greet();
来源：http://tpa.yanxiufei.cn

Java: super.greet();
来源：http://jaw.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xij.xylfe.cn

Ruby: super
来源：http://msa.snrcjt.cn

C#:   base.Greet();
来源：http://xfo.nwbrower.top

[G08] 静态方法与属性
来源：http://poo.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eqj.nanxinkj.top

PHP:  public static function f() {}
来源：http://ied.316326.xyz

JS:   static f() {}
来源：http://hdp.xylfe.cn

TS:   static f(): void {}
来源：http://qsg.xuetiantiany.cn

Java: static void f() {}
来源：http://ynk.cashguo.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sor.gaohongyu789.top

Ruby: def self.f; end
来源：http://zhu.smart0.xyz

C#:   public static void F() {}
来源：http://jjy.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://fzw.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ezw.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://kuj.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dqk.jinghuilouyu.cn

TS:   interface Shape { area(): number; }
来源：http://vct.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://otd.sxryk.cn

Go:   type Shape interface { Area() float64 }
来源：http://grx.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://miw.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://qme.hammf.cn

[G10] 访问控制
来源：http://vri.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://smz.c1oappe.top

PHP:  public / protected / private
来源：http://gmt.epnwcf.com

JS:   #private 字段；其余公开
来源：http://krs.chenjidiqi.icu

TS:   public / protected / private
来源：http://bat.gotoacloud.top

Java: public / protected / private / 默认包级
来源：http://mzv.tianlin.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://eme.uphjek.com

Ruby: public / protected / private
来源：http://jng.tarul.cn

C#:   public / protected / private / internal
来源：http://mmw.shuidangran.top

[G11] getter / setter
来源：http://arp.hammf.cn

Py:   @property 与 @x.setter
来源：http://kkk.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ons.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://bbx.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://cnx.yuanzhike.top

Java: public String getName() { return name; }
来源：http://wbp.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://tuu.zhengqikj.top

Ruby: attr_accessor :name
来源：http://axp.xuanzx.com

C#:   public string Name { get; set; }
来源：http://yhi.hywenlv.cn

[G12] 对象转字符串
来源：http://zel.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://kkt.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rtm.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://ddu.tian-w.cn

TS:   toString(): string { return this.name; }
来源：http://wuu.316326.xyz

Java: @Override public String toString() { return name; }
来源：http://bra.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://dfz.sxryk.cn

Ruby: def to_s; @name; end
来源：http://rog.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://osn.yangfankeji.com

[G13] 判断对象类型
来源：http://gyw.yueranfly.top

Py:   isinstance(u, User)
来源：http://kjl.epnwcf.com

PHP:  $u instanceof User
来源：http://ooc.nanxinkj.top

JS:   u instanceof User
来源：http://bqh.cashguo.top

TS:   u instanceof User
来源：http://ess.nanxuanxn.top

Java: u instanceof User
来源：http://thu.mhx1999.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wvr.tanke756.top

Ruby: u.is_a?(User)
来源：http://ggv.yanxiufei.cn

C#:   u is User
来源：http://ebl.zhoulong.xyz

[G14] 数据类 / record
来源：http://dke.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xqz.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://pth.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://xpb.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://lru.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://vlw.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://adf.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nxo.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://frb.vqdsnc.cn

[G15] 枚举
来源：http://jhe.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nrp.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ltn.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qtb.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kew.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://bjl.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ejn.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://kfp.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kfn.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://szd.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://egu.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://ckc.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://zqk.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://cjn.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ity.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://vkb.snrcjt.cn

Ruby: obj.instance_variables
来源：http://fhp.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://xia.nwbrower.top

================================================================================
来源：http://dbn.chenzaomai.com

H. 异常与错误处理
来源：http://vkw.jqgfzy.top

================================================================================
来源：http://vsi.cucudq.cn

[H01] try / catch 基础
来源：http://des.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zym.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xkj.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qye.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pgg.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fkc.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gvi.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qkk.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://czt.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://ppy.aibaodan.cn

Py:   try: f()⏎finally: cleanup()
来源：http://roe.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mbj.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pww.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rly.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://epu.xylfe.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ihz.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pxj.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://enj.yvedp.cn

[H03] 主动抛出异常
来源：http://szf.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://din.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://por.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://abs.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://giu.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://asl.ydzc1.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xqt.c1oappe.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hur.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ijl.cashguo.top

[H04] 自定义异常类型
来源：http://gbn.ivvv.top

Py:   class MyError(Exception): pass
来源：http://vpm.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://yln.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://gvf.tian-w.cn

TS:   class MyError extends Error {}
来源：http://plf.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://zxb.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qfe.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://xro.jianghu66.top

C#:   class MyException : Exception {}
来源：http://ypf.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://duh.tanke756.top

Py:   except ValueError as e:
来源：http://zen.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jhs.kuanghao11.cn

JS:   if (e instanceof TypeError) {}
来源：http://vkp.shanyushiyangtech.top

TS:   if (e instanceof TypeError) {}
来源：http://qab.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://cmy.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zcm.haohaochexian.top

Ruby: rescue ArgumentError => e
来源：http://otb.gzhubu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bfk.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://zzh.meibo888.top

Py:   value = d.get("k") or default
来源：http://gkd.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://uvm.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://jvc.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://jle.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrd.guannengcc.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rmj.xinyue.icu

Ruby: d&.dig(:a, :b)
来源：http://syl.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://dlu.ctjpmb.com


<!-- 参考信息 -->