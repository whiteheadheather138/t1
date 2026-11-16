代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dtj.chenjidiqi.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://srd.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zze.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lxv.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rgh.nanxinkj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hbd.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://smx.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hoe.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://izl.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://glf.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wfc.quarkkingdee.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jew.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lsk.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://xah.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qaz.chenjidiqi.icu

[F04] 追加写入文件
来源：http://zho.316326.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tug.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ajf.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gub.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmc.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lua.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ghh.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kvd.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://izw.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://nnw.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fud.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://uai.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://pci.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://hkc.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wag.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rnm.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://kxk.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://leg.shangyingyoupin.top

[F06] 删除文件
来源：http://avr.zycfv.cn

Py:   os.remove("a.txt")
来源：http://skb.yvedp.cn

PHP:  unlink("a.txt");
来源：http://krm.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://qti.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://qsi.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ctg.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://kdk.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://tjq.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://irl.gzhubu.top

[F07] 创建目录（含多级）
来源：http://avr.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jpb.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zqy.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nzl.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://frq.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hkh.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bef.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rqq.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mew.nanxuanxn.top

[F08] 遍历目录
来源：http://vef.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hne.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jts.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://nsx.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://xkl.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qnn.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pdc.cashguo.top

Ruby: Dir.children("dir")
来源：http://nzf.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://oej.ehwqpu.com

[F09] 获取文件大小
来源：http://qji.jlsjyb.cn

Py:   os.path.getsize("a.txt")
来源：http://qty.havefunace.top

PHP:  filesize("a.txt");
来源：http://wyy.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://gew.shzxlz.cn

TS:   fs.statSync("a.txt").size
来源：http://lar.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://tmq.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fcz.wangdashe.top

Ruby: File.size("a.txt")
来源：http://tbk.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://fsl.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://irv.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://env.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tbr.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://szf.ybcxt.top

TS:   path.extname("a.txt")
来源：http://rbt.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ppo.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hqa.meibo888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jti.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fes.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://evb.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bep.jyoumei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oot.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hls.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iqb.xziqi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fta.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tse.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yzr.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sro.jlsjyb.cn

[F12] CSV 读写
来源：http://nix.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ldu.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uln.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rst.guannengcc.top

TS:   // 同上
来源：http://zeq.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zcr.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rtd.jlsjyb.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zmr.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://isf.yonumen.top

================================================================================
来源：http://lah.kuanghao11.cn

G. 面向对象
来源：http://csf.cashguo.top

================================================================================
来源：http://lcn.jinyuanbaomall.cn

[G01] 定义类
来源：http://jse.gaohongyu789.top

Py:   class User: pass
来源：http://wrs.yonumen.top

PHP:  class User {}
来源：http://hir.zdqjudy.top

JS:   class User {}
来源：http://sni.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://sqs.wangshuangyany.cn

Java: class User {}
来源：http://wiq.hammf.cn

Go:   type User struct { Name string }
来源：http://rvo.epnwcf.com

Ruby: class User; end
来源：http://jzf.zycfv.cn

C#:   class User {}
来源：http://xkb.yj202588.top

[G02] 构造函数
来源：http://eqf.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://rnl.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://axg.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://qgj.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://ygv.yueranfly.top

Java: User(String name) { this.name = name; }
来源：http://oub.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ksg.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://lni.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://uig.yj202588.top

[G03] 实例属性
来源：http://ywy.yuanzhike.top

Py:   self.name = "x"
来源：http://nod.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://akt.zhixingplan.top

JS:   this.name = "x";
来源：http://meu.nwbrower.top

TS:   name: string = "x";
来源：http://ons.hysaishi.cn

Java: private String name;
来源：http://nak.uphjek.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hfl.wangshuangyany.cn

Ruby: @name = "x"
来源：http://djt.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://gmg.gotoacloud.top

[G04] 定义方法
来源：http://nxm.cheryme.top

Py:   def greet(self): return self.name
来源：http://kxy.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xbc.yuxming.cn

JS:   greet() { return this.name; }
来源：http://eqv.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://mgg.chenlongwang.top

Java: String greet() { return name; }
来源：http://ccz.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wgj.yfazqb.com

Ruby: def greet; @name; end
来源：http://dzl.cashguo.top

C#:   public string Greet() => Name;
来源：http://xsr.xylfe.cn

[G05] 继承
来源：http://knj.yonumen.top

Py:   class Admin(User): pass
来源：http://egm.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://pig.hesvh.cn

JS:   class Admin extends User {}
来源：http://bin.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://ewz.svipenyu.cn

Java: class Admin extends User {}
来源：http://oja.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qmb.ydzc1.top

Ruby: class Admin < User; end
来源：http://ifw.chenjidiqi.icu

C#:   class Admin : User {}
来源：http://gwc.hesvh.cn

[G06] 重写方法
来源：http://xkf.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://zdg.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ljf.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://gwo.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://kyj.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://qic.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mam.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://ckx.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://hqx.jianghu66.top

[G07] 调用父类方法
来源：http://pzt.jqgfzy.top

Py:   super().greet()
来源：http://fba.dashuyun.cn

PHP:  parent::greet();
来源：http://gfo.aizwys.cn

JS:   super.greet();
来源：http://gur.meibo888.top

TS:   super.greet();
来源：http://tsu.iojbl.cn

Java: super.greet();
来源：http://lwp.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tyo.zhiwuduotai.top

Ruby: super
来源：http://qwp.hongshengwenyu.top

C#:   base.Greet();
来源：http://nkv.yfazqb.com

[G08] 静态方法与属性
来源：http://gjk.ydzc1.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jsa.vehdjk.com

PHP:  public static function f() {}
来源：http://kvq.zdqjudy.top

JS:   static f() {}
来源：http://gbf.ivvv.top

TS:   static f(): void {}
来源：http://eva.xziqi.cn

Java: static void f() {}
来源：http://ymk.shuidangran.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eif.uphjek.com

Ruby: def self.f; end
来源：http://hqt.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://fwu.xinyue.icu

[G09] 接口 / 抽象类
来源：http://ynv.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://wpj.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://xfu.svipenyu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mwo.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://bsj.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://mmf.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://cux.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zub.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://smu.jinqigufen.top

[G10] 访问控制
来源：http://hpj.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://brj.aibaodan.cn

PHP:  public / protected / private
来源：http://vcj.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://daa.vqdsnc.cn

TS:   public / protected / private
来源：http://zqq.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://hwl.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ctd.yvedp.cn

Ruby: public / protected / private
来源：http://omn.jqgfzy.top

C#:   public / protected / private / internal
来源：http://mxu.xziqi.cn

[G11] getter / setter
来源：http://jup.epnwcf.com

Py:   @property 与 @x.setter
来源：http://uwv.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://svb.xuanzx.com

JS:   get name() { return this._name; }
来源：http://nzo.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://nvz.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://zpx.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tpo.shuidangran.top

Ruby: attr_accessor :name
来源：http://ffw.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://jxy.uphjek.com

[G12] 对象转字符串
来源：http://lvk.vehdjk.com

Py:   def __str__(self): return self.name
来源：http://phb.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://brm.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://mjj.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://sqx.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://bez.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://wie.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://asv.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://tmk.sweek.top

[G13] 判断对象类型
来源：http://idc.chenzaomai.com

Py:   isinstance(u, User)
来源：http://qgq.sjlbkw.cn

PHP:  $u instanceof User
来源：http://twz.ppjwa.cn

JS:   u instanceof User
来源：http://ekf.yfazqb.com

TS:   u instanceof User
来源：http://kks.sxryk.cn

Java: u instanceof User
来源：http://utt.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nwa.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://gvp.ybcxt.top

C#:   u is User
来源：http://dvs.cashguo.top

[G14] 数据类 / record
来源：http://kwq.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wte.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://sxz.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://qfu.snrcjt.cn

TS:   type User = { name: string; age: number };
来源：http://xkm.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://qvo.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://fed.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zhe.jinqigufen.top

C#:   record User(string Name, int Age);
来源：http://dvt.yangfankeji.com

[G15] 枚举
来源：http://mnq.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pbm.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://lgt.jqgufenzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hwr.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://imf.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://ist.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxx.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://kxr.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tdw.zhiwuduotai.top

[G16] 对象转数组 / 字典
来源：http://mfx.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ybm.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://jfi.hywenlv.cn

JS:   Object.entries(obj)
来源：http://dvt.hysaishi.cn

TS:   Object.entries(obj)
来源：http://ipg.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://txa.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nct.c1oappe.top

Ruby: obj.instance_variables
来源：http://hjl.tian-w.cn

C#:   // 用反射或 System.Text.Json
来源：http://xpq.yangfankeji.com

================================================================================
来源：http://rfc.yanxiufei.cn

H. 异常与错误处理
来源：http://jbf.nanxuanxn.top

================================================================================
来源：http://eje.bjfxy.top

[H01] try / catch 基础
来源：http://eoa.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bdd.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uvq.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://twv.9152youxi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://snu.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gjz.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cnp.zhixingplan.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qsw.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bmj.pengpengdd.cyou

[H02] finally / ensure 收尾
来源：http://azr.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nlj.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rkp.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://spn.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oyo.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://akq.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://acp.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wil.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ord.iojbl.cn

[H03] 主动抛出异常
来源：http://dmg.jinghuilouyu.cn

Py:   raise ValueError("错误信息")
来源：http://uny.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sjf.daxiang520.top

JS:   throw new Error("错误信息");
来源：http://dzn.zdqjudy.top

TS:   throw new Error("错误信息");
来源：http://ypf.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://jre.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yis.birdmap.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ttm.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://qgc.aizwys.cn

[H04] 自定义异常类型
来源：http://rvj.dianchejie.cn

Py:   class MyError(Exception): pass
来源：http://zto.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://drk.yvedp.cn

JS:   class MyError extends Error {}
来源：http://rzp.52xcode.cn

TS:   class MyError extends Error {}
来源：http://xld.bjfxy.top

Java: class MyException extends RuntimeException {}
来源：http://vyc.uphjek.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iqx.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://uei.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://jvq.tanke756.top

[H05] 捕获特定类型
来源：http://gwb.tarul.cn

Py:   except ValueError as e:
来源：http://mgo.fehbvm.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://beq.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://xsk.cucudq.cn

TS:   if (e instanceof TypeError) {}
来源：http://atv.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://xfu.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fps.nwbrower.top

Ruby: rescue ArgumentError => e
来源：http://fyn.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tgk.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://pdh.fzhhl.top

Py:   value = d.get("k") or default
来源：http://bia.gzhubu.top

PHP:  $v = $d["k"] ?? null;
来源：http://voq.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rsm.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://zdr.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dag.hongshengwenyu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://csj.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://ahb.yonumen.top

C#:   obj?.A?.B ?? default
来源：http://sdt.yuxming.cn


<!-- 参考信息 -->