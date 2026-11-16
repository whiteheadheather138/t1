代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://rta.jiagoushi.top

[F02] 逐行读取文件
来源：http://hqu.shangyingyoupin.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xpf.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bwa.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vnq.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nvl.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jkg.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dbr.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gua.aizwys.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bzr.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://zut.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xyl.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://que.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uqh.vqdsnc.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qcz.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://icd.zdbjq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lme.feifeiyinyue.top

Ruby: File.write("a.txt", "hi")
来源：http://xoc.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mzx.ydjk.org.cn

[F04] 追加写入文件
来源：http://yzc.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pgx.dianchejie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qed.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yri.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bzm.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uek.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://whb.zhijiandao.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://taj.cheryme.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ckg.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://bhk.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mmd.svipenyu.cn

PHP:  file_exists("a.txt");
来源：http://glz.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://qyy.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://zlh.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://usd.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nyp.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://xff.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://uwg.hcnkem.com

[F06] 删除文件
来源：http://hda.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://wlu.shuidangran.top

PHP:  unlink("a.txt");
来源：http://lwe.pycfn.com

JS:   fs.unlinkSync("a.txt")
来源：http://pfk.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://dlh.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ggy.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://hcg.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://aze.cashguo.top

C#:   File.Delete("a.txt");
来源：http://uxz.bjfxy.top

[F07] 创建目录（含多级）
来源：http://jks.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdd.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gpv.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iss.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxh.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rei.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://din.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ier.redwolf501.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cwa.redwolf501.top

[F08] 遍历目录
来源：http://wil.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vor.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://svh.hcnkem.com

JS:   fs.readdirSync("dir")
来源：http://aub.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://bkv.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fko.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://tcf.guannengcc.top

Ruby: Dir.children("dir")
来源：http://vat.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://cyj.yonumen.top

[F09] 获取文件大小
来源：http://boi.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://jic.xylfe.cn

PHP:  filesize("a.txt");
来源：http://ggc.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://pmj.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://qin.zdbjq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zqg.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jhb.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://alm.birdmap.top

C#:   new FileInfo("a.txt").Length
来源：http://qib.yfazqb.com

[F10] 取文件扩展名 / 文件名
来源：http://qqf.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hwc.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ivg.xziqi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://spu.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://cjn.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qdf.jinqigfzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kcd.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://smk.sxryk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yky.yongpay.top

[F11] 复制与移动文件
来源：http://gfd.yj20258888.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iac.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://boc.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aql.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wcf.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aju.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qju.chenjidiqi.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bur.fanxiaobao.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://coz.ydjk.org.cn

[F12] CSV 读写
来源：http://dib.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ilo.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nvh.snrcjt.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://htq.hnqzz.top

TS:   // 同上
来源：http://bwt.aizwys.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://deh.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jtu.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ebe.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://hjq.ywan-chungtsiang.top

================================================================================
来源：http://cmo.ehwqpu.com

G. 面向对象
来源：http://skq.tanke756.top

================================================================================
来源：http://ore.nanxinkj.top

[G01] 定义类
来源：http://rqu.tianlin.xyz

Py:   class User: pass
来源：http://bpg.jiagoushi.top

PHP:  class User {}
来源：http://rey.meibo888.top

JS:   class User {}
来源：http://uhb.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://rve.zhengqikj.top

Java: class User {}
来源：http://ivs.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://yho.fengsongda.top

Ruby: class User; end
来源：http://gog.jinyuanbaomall.cn

C#:   class User {}
来源：http://ros.yueranfly.top

[G02] 构造函数
来源：http://zva.redwolf501.top

Py:   def __init__(self, name): self.name = name
来源：http://tph.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://iyg.ctjpmb.com

JS:   constructor(name) { this.name = name; }
来源：http://qpn.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://iaf.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://lwa.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pxu.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://yqt.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://byd.sysykeji.top

[G03] 实例属性
来源：http://ivb.sweek.top

Py:   self.name = "x"
来源：http://fjf.svipenyu.cn

PHP:  public string $name = "x";
来源：http://mhi.sysykeji.top

JS:   this.name = "x";
来源：http://oup.xinyue.icu

TS:   name: string = "x";
来源：http://fqh.sxryk.cn

Java: private String name;
来源：http://jdt.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://awn.cheryme.top

Ruby: @name = "x"
来源：http://vfn.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://zew.zhoulong.xyz

[G04] 定义方法
来源：http://crr.ydzc1.top

Py:   def greet(self): return self.name
来源：http://rbz.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dwy.tarul.cn

JS:   greet() { return this.name; }
来源：http://zxz.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://avr.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://ruj.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uxn.gzhubu.top

Ruby: def greet; @name; end
来源：http://kkw.cashguo.top

C#:   public string Greet() => Name;
来源：http://mwp.zhixingplan.top

[G05] 继承
来源：http://kwx.cqqwz.cn

Py:   class Admin(User): pass
来源：http://hdl.redwolf501.top

PHP:  class Admin extends User {}
来源：http://ewh.havefunace.top

JS:   class Admin extends User {}
来源：http://zvl.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://soc.yvedp.cn

Java: class Admin extends User {}
来源：http://snn.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://moa.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://vca.bbcook.cn

C#:   class Admin : User {}
来源：http://ojp.svipenyu.cn

[G06] 重写方法
来源：http://mwz.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://qmg.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://fgt.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://joo.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://pky.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://qzc.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kcz.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://dpn.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://fyp.zhongyouzk.top

[G07] 调用父类方法
来源：http://yjz.hesvh.cn

Py:   super().greet()
来源：http://ygo.mhx1999.top

PHP:  parent::greet();
来源：http://gyh.fengsongda.top

JS:   super.greet();
来源：http://rox.zdqjudy.top

TS:   super.greet();
来源：http://olg.bbcook.cn

Java: super.greet();
来源：http://emj.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vlv.xuanzx.com

Ruby: super
来源：http://xnf.cqqwz.cn

C#:   base.Greet();
来源：http://rxr.epnwcf.com

[G08] 静态方法与属性
来源：http://peg.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gej.bbcook.cn

PHP:  public static function f() {}
来源：http://auh.nanxuanxn.top

JS:   static f() {}
来源：http://sgg.yueranfly.top

TS:   static f(): void {}
来源：http://chu.yj202588.top

Java: static void f() {}
来源：http://vby.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ddd.yangfankeji.com

Ruby: def self.f; end
来源：http://vuj.vehdjk.com

C#:   public static void F() {}
来源：http://ieu.zhongyouzk.top

[G09] 接口 / 抽象类
来源：http://ozr.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://lwz.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lsi.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wfc.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://uef.uphjek.com

Java: interface Shape { double area(); }
来源：http://gwl.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://jez.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://grn.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://vqq.xylfe.cn

[G10] 访问控制
来源：http://kge.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://lxd.meibo888.top

PHP:  public / protected / private
来源：http://sni.tianlin.xyz

JS:   #private 字段；其余公开
来源：http://oqo.redwolf501.top

TS:   public / protected / private
来源：http://ack.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://cek.ctjpmb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://efy.chenjidiqi.icu

Ruby: public / protected / private
来源：http://pko.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://gfs.mhx1999.top

[G11] getter / setter
来源：http://dyb.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://gnj.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ijz.52xcode.cn

JS:   get name() { return this._name; }
来源：http://ath.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://gnd.tanke756.top

Java: public String getName() { return name; }
来源：http://bky.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cge.bjfxy.top

Ruby: attr_accessor :name
来源：http://sog.sufxvd.cn

C#:   public string Name { get; set; }
来源：http://cik.ehwqpu.com

[G12] 对象转字符串
来源：http://dro.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://mdm.sxryk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gto.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://hux.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://oiw.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://sqf.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://ctz.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://glc.yj202588.top

C#:   public override string ToString() => Name;
来源：http://ehc.yuxming.cn

[G13] 判断对象类型
来源：http://vuf.nanxinkj.top

Py:   isinstance(u, User)
来源：http://bbm.snrcjt.cn

PHP:  $u instanceof User
来源：http://whf.zycfv.cn

JS:   u instanceof User
来源：http://nen.vehdjk.com

TS:   u instanceof User
来源：http://acp.chenzaomai.com

Java: u instanceof User
来源：http://lka.guannengcc.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lsd.yonumen.top

Ruby: u.is_a?(User)
来源：http://awv.jinghuilouyu.cn

C#:   u is User
来源：http://qdc.gotoacloud.top

[G14] 数据类 / record
来源：http://clh.yangfankeji.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fqz.yvedp.cn

PHP:  // 用 readonly 属性模拟
来源：http://sjc.jianghu66.top

JS:   // 无内置：普通类或对象字面量
来源：http://lrc.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://hpe.ybcxt.top

Java: record User(String name, int age) {}
来源：http://zkd.zhixingplan.top

Go:   type User struct { Name string; Age int }
来源：http://fhm.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fzy.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://wgb.xuetiantiany.cn

[G15] 枚举
来源：http://vzg.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gav.shuidangran.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sru.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kmw.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xka.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://nlh.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ayp.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://eqv.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jua.yonumen.top

[G16] 对象转数组 / 字典
来源：http://xfm.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rzd.nwbrower.top

PHP:  get_object_vars($obj);
来源：http://bfv.cashguo.top

JS:   Object.entries(obj)
来源：http://nly.nanxuanxn.top

TS:   Object.entries(obj)
来源：http://iub.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ual.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://twq.xuanzx.com

Ruby: obj.instance_variables
来源：http://trr.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://dee.mhx1999.top

================================================================================
来源：http://dyy.pycfn.com

H. 异常与错误处理
来源：http://flr.ivvv.top

================================================================================
来源：http://mdi.hongshengwenyu.top

[H01] try / catch 基础
来源：http://jrg.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rcn.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ykh.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://abs.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ytd.meibo888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfa.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qyx.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gmo.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eje.fengsongda.top

[H02] finally / ensure 收尾
来源：http://eql.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://mhx.fengsongda.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eno.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://acz.meibo888.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sin.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bwy.shuidangran.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yhg.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://zaz.jqgufenzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cie.ehwqpu.com

[H03] 主动抛出异常
来源：http://szn.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://xxz.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mts.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://fzw.jinyuanbaomall.cn

TS:   throw new Error("错误信息");
来源：http://lnp.0kj1m.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://orw.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fgz.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://twf.zhengqikj.top

C#:   throw new ArgumentException("错误信息");
来源：http://wus.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://sex.wangshuangyany.cn

Py:   class MyError(Exception): pass
来源：http://fky.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://rvi.gaohongyu789.top

JS:   class MyError extends Error {}
来源：http://vtz.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://jpq.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://ovh.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mxw.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://hcu.aibaodan.cn

C#:   class MyException : Exception {}
来源：http://zmh.guowangkeji.top

[H05] 捕获特定类型
来源：http://gvg.bbcook.cn

Py:   except ValueError as e:
来源：http://eib.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wce.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://ano.tian-w.cn

TS:   if (e instanceof TypeError) {}
来源：http://ezf.mhx1999.top

Java: catch (IOException | SQLException e) {}
来源：http://yjn.hfpthk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ghz.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://fyk.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jqq.jlsjyb.cn

[H06] 可选值 / 空值安全访问
来源：http://nfi.cheryme.top

Py:   value = d.get("k") or default
来源：http://eef.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zdn.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://xmz.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://bmo.ywan-chungtsiang.top


<!-- 参考信息 -->