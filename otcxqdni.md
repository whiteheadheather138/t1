代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://syz.jiagoushi.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yln.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qxu.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://aot.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://nbk.ydjk.org.cn

[F02] 逐行读取文件
来源：http://niz.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://osl.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fll.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xsj.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yfk.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zkd.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nny.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://exc.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wde.tarul.cn

[F03] 写入文件（覆盖）
来源：http://jpj.uphjek.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yup.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ghv.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ara.zhaomingkeji.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vod.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://svf.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xtz.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://uuz.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lxq.bbcook.cn

[F04] 追加写入文件
来源：http://rjt.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mwf.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://thh.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kvm.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mjq.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fdu.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mrq.tian-w.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nvz.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://avy.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://pql.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ydt.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://kvu.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://jzb.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://koh.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zhc.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://umj.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://qlg.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://goe.gaohongyu789.top

[F06] 删除文件
来源：http://skj.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://bbh.ydzc1.top

PHP:  unlink("a.txt");
来源：http://imy.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://fvy.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://pxg.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hur.yanxiufei.cn

Go:   os.Remove("a.txt")
来源：http://mco.hammf.cn

Ruby: File.delete("a.txt")
来源：http://qrf.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://wjq.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://fdk.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nnp.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cnt.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ufs.yj20258888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zmy.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qtb.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://shc.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tik.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hok.guannengcc.top

[F08] 遍历目录
来源：http://pcj.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fwu.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://olx.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://gsz.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://toz.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nbz.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wiw.sysykeji.top

Ruby: Dir.children("dir")
来源：http://yyh.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://uar.yj20258888.top

[F09] 获取文件大小
来源：http://ynn.sjlbkw.cn

Py:   os.path.getsize("a.txt")
来源：http://sqs.gaohongyu789.top

PHP:  filesize("a.txt");
来源：http://ntv.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://jrw.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://nee.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://fte.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rwk.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://ghk.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://vnq.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://ywi.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nyf.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bik.gzhubu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cef.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://mrz.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yct.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iwl.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bez.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fid.tarul.cn

[F11] 复制与移动文件
来源：http://jox.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wag.tianlin.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rgj.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfg.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfr.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xij.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zuk.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ijz.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ayy.hfpthk.cn

[F12] CSV 读写
来源：http://dbd.shuidangran.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zcc.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qoi.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xny.quarkkingdee.top

TS:   // 同上
来源：http://uzu.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ovm.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jsm.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tcj.sufxvd.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vtm.pengpengdd.cyou

================================================================================
来源：http://rdp.andypj.xyz

G. 面向对象
来源：http://pok.bbcook.cn

================================================================================
来源：http://oei.hnqzz.top

[G01] 定义类
来源：http://rbm.ybcxt.top

Py:   class User: pass
来源：http://wvt.fzhhl.top

PHP:  class User {}
来源：http://dyl.hcnkem.com

JS:   class User {}
来源：http://cml.sjlbkw.cn

TS:   class User { name: string = ""; }
来源：http://efw.ydjk.org.cn

Java: class User {}
来源：http://ycb.zhengqikj.top

Go:   type User struct { Name string }
来源：http://ohg.cqqwz.cn

Ruby: class User; end
来源：http://hov.316326.xyz

C#:   class User {}
来源：http://qge.hcnkem.com

[G02] 构造函数
来源：http://fed.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://sjg.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://cgn.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://gws.shuidangran.top

TS:   constructor(public name: string) {}
来源：http://xie.xingfuxueyuan.xyz

Java: User(String name) { this.name = name; }
来源：http://qfw.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jef.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://mnl.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://pkn.yj20258.top

[G03] 实例属性
来源：http://fuy.jyoumei.cn

Py:   self.name = "x"
来源：http://fjk.iojbl.cn

PHP:  public string $name = "x";
来源：http://prl.mhx1999.top

JS:   this.name = "x";
来源：http://qeq.fzhhl.top

TS:   name: string = "x";
来源：http://ysm.epnwcf.com

Java: private String name;
来源：http://ntn.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uhk.shangyingyoupin.top

Ruby: @name = "x"
来源：http://hzv.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://xzm.zdbjq.cn

[G04] 定义方法
来源：http://kyt.yj202588.top

Py:   def greet(self): return self.name
来源：http://suj.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://prb.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://nsa.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://iug.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://odj.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dok.pycfn.com

Ruby: def greet; @name; end
来源：http://jie.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://blq.fanxiaobao.xyz

[G05] 继承
来源：http://zbe.tanke756.top

Py:   class Admin(User): pass
来源：http://geh.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://uos.ydzc1.top

JS:   class Admin extends User {}
来源：http://ceb.sysykeji.top

TS:   class Admin extends User {}
来源：http://kuo.cucudq.cn

Java: class Admin extends User {}
来源：http://uil.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mjn.ydzc1.top

Ruby: class Admin < User; end
来源：http://tmg.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://kgr.cdnleiting.top

[G06] 重写方法
来源：http://fvh.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://uqo.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fde.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://yuk.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://phz.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://uml.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dsg.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://mci.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://lka.sxryk.cn

[G07] 调用父类方法
来源：http://bom.cheryme.top

Py:   super().greet()
来源：http://pqo.jiagoushi.top

PHP:  parent::greet();
来源：http://pkn.uphjek.com

JS:   super.greet();
来源：http://gwf.ydzc1.top

TS:   super.greet();
来源：http://jey.jqgfzy.top

Java: super.greet();
来源：http://mss.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dic.fehbvm.com

Ruby: super
来源：http://geu.ctjpmb.com

C#:   base.Greet();
来源：http://zfp.xingfuxueyuan.xyz

[G08] 静态方法与属性
来源：http://lij.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ibx.cashguo.top

PHP:  public static function f() {}
来源：http://kaq.zhengqikj.top

JS:   static f() {}
来源：http://fii.uphjek.com

TS:   static f(): void {}
来源：http://wae.feifeiyinyue.top

Java: static void f() {}
来源：http://cml.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://knu.hysaishi.cn

Ruby: def self.f; end
来源：http://okl.pycfn.com

C#:   public static void F() {}
来源：http://alv.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://iiw.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://yvy.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://eap.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rfu.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://llm.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://plf.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://ktt.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kvy.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://cqz.smart0.xyz

[G10] 访问控制
来源：http://vzb.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://bub.zhiwuduotai.top

PHP:  public / protected / private
来源：http://qen.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://ens.yuxming.cn

TS:   public / protected / private
来源：http://kgx.316326.xyz

Java: public / protected / private / 默认包级
来源：http://gnh.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://crd.hcnkem.com

Ruby: public / protected / private
来源：http://qow.cashguo.top

C#:   public / protected / private / internal
来源：http://clz.iojbl.cn

[G11] getter / setter
来源：http://qno.smart0.xyz

Py:   @property 与 @x.setter
来源：http://rsw.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tuc.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://zbv.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://mlg.nanxinkj.top

Java: public String getName() { return name; }
来源：http://fdm.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lvp.gzhubu.top

Ruby: attr_accessor :name
来源：http://vfe.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://wuv.c1oappe.top

[G12] 对象转字符串
来源：http://fxs.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://dfa.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tlg.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://hit.c1oappe.top

TS:   toString(): string { return this.name; }
来源：http://txk.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://orh.ydzc1.top

Go:   func (u User) String() string { return u.Name }
来源：http://yro.hesvh.cn

Ruby: def to_s; @name; end
来源：http://dsc.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://xyp.cqqwz.cn

[G13] 判断对象类型
来源：http://ugi.fzhhl.top

Py:   isinstance(u, User)
来源：http://wpo.yuxming.cn

PHP:  $u instanceof User
来源：http://wtn.fehbvm.com

JS:   u instanceof User
来源：http://ofc.hesvh.cn

TS:   u instanceof User
来源：http://kty.316326.xyz

Java: u instanceof User
来源：http://ivw.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://emx.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://ddp.yonumen.top

C#:   u is User
来源：http://ktu.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://xln.52xcode.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://obq.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://mus.zhaomingkeji.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://uvk.tian-w.cn

TS:   type User = { name: string; age: number };
来源：http://wpn.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://twh.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://hze.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oop.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://tsj.cheryme.top

[G15] 枚举
来源：http://mdt.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ben.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ump.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://icl.chenzaomai.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dvd.jinyuanbaomall.cn

Java: enum Color { RED, GREEN }
来源：http://yll.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://voh.xinyue.icu

Ruby: Color = %i[red green].freeze
来源：http://aoz.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://axj.hammf.cn

[G16] 对象转数组 / 字典
来源：http://wum.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uqs.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://htf.316326.xyz

JS:   Object.entries(obj)
来源：http://vom.nanxinkj.top

TS:   Object.entries(obj)
来源：http://fxo.dashuyun.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xsb.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jdh.zdqjudy.top

Ruby: obj.instance_variables
来源：http://orq.epnwcf.com

C#:   // 用反射或 System.Text.Json
来源：http://jlm.aizwys.cn

================================================================================
来源：http://xbo.yvedp.cn

H. 异常与错误处理
来源：http://lel.fehbvm.com

================================================================================
来源：http://aif.gaohongyu789.top

[H01] try / catch 基础
来源：http://yny.yj20258888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qqu.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bqz.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://trb.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://flx.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gnf.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtj.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ipu.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qtt.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://gwx.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lox.cqqwz.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://klj.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://irc.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://msf.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://oip.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://wkj.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ihq.dashuyun.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nwb.chenlongwang.top

[H03] 主动抛出异常
来源：http://ozi.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://xom.sysykeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lvg.hfpthk.cn

JS:   throw new Error("错误信息");
来源：http://udo.smart0.xyz

TS:   throw new Error("错误信息");
来源：http://nto.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qgq.hfpthk.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qdc.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://teq.cashguo.top

C#:   throw new ArgumentException("错误信息");
来源：http://orx.birdmap.top

[H04] 自定义异常类型
来源：http://ghu.pycfn.com

Py:   class MyError(Exception): pass
来源：http://cxu.haohaochexian.top

PHP:  class MyError extends RuntimeException {}
来源：http://bfa.yuxming.cn

JS:   class MyError extends Error {}
来源：http://fuh.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://ung.fengsongda.top

Java: class MyException extends RuntimeException {}
来源：http://fsr.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qon.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://eol.xuanzx.com

C#:   class MyException : Exception {}
来源：http://tsl.zhixingplan.top

[H05] 捕获特定类型
来源：http://tkl.cqqwz.cn

Py:   except ValueError as e:
来源：http://etj.smart0.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pvl.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://cob.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://gkn.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://edf.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rww.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://lrf.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qyq.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://wsm.jinghuilouyu.cn


<!-- 参考信息 -->