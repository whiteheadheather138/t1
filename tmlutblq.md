代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://csp.ivvv.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wfr.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zea.xziqi.cn

Ruby: File.read("a.txt")
来源：http://pms.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://cww.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://vio.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qhp.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dls.ybcxt.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lty.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ecr.daxiang520.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mhj.yonumen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iou.svipenyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hyk.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pmj.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://ymb.yj20258.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://heh.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bzc.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qvs.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oli.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pvj.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gpx.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://ykz.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wpx.tian-w.cn

[F04] 追加写入文件
来源：http://wen.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yib.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ozw.fehbvm.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqh.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xtk.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rjd.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dnl.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://knx.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wxp.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://tyf.ppjwa.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://miu.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://vyn.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://uss.tianlin.xyz

TS:   fs.existsSync("a.txt")
来源：http://drk.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wmg.jqgufenzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lzd.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://cfs.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://acb.havefunace.top

[F06] 删除文件
来源：http://rax.yj20258888.top

Py:   os.remove("a.txt")
来源：http://azc.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://sit.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://css.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bbu.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mju.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://bdj.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://sqj.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://srp.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://rwf.shanyushiyangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hpz.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vem.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://slw.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cfr.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lgc.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yly.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hwo.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hto.chenlongwang.top

[F08] 遍历目录
来源：http://gec.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mmk.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yqs.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://rcu.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://mcv.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tdk.jinqigfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tkp.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://exv.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://ute.ppjwa.cn

[F09] 获取文件大小
来源：http://oty.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://rwx.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://oux.yfazqb.com

JS:   fs.statSync("a.txt").size
来源：http://zkh.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://wbc.smart0.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://asx.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://njl.tian-w.cn

Ruby: File.size("a.txt")
来源：http://hzd.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://hyq.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lnb.jinghuilouyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nqc.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://byr.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwf.hammf.cn

TS:   path.extname("a.txt")
来源：http://jyf.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xbi.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfq.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxk.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://axz.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://njw.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kgy.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wky.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvd.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hts.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wom.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mrf.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tdw.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://odn.hnxiangtu.top

[F12] CSV 读写
来源：http://vtj.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wdp.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ipv.shanyushiyangtech.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrl.hcnkem.com

TS:   // 同上
来源：http://esf.svipenyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uwf.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eqc.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tov.ydzc1.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yfg.gaohongyu789.top

================================================================================
来源：http://qys.xylfe.cn

G. 面向对象
来源：http://bir.shzxlz.cn

================================================================================
来源：http://kvw.meibo888.top

[G01] 定义类
来源：http://ibv.yj202588.top

Py:   class User: pass
来源：http://eyd.zdbjq.cn

PHP:  class User {}
来源：http://jsw.yj20258888.top

JS:   class User {}
来源：http://chb.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://pgf.jinyuanbaomall.cn

Java: class User {}
来源：http://cso.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://cgz.tianlin.xyz

Ruby: class User; end
来源：http://mfn.yongpay.top

C#:   class User {}
来源：http://uye.tanke756.top

[G02] 构造函数
来源：http://dti.shanyushiyangtech.top

Py:   def __init__(self, name): self.name = name
来源：http://imv.fanxiaobao.xyz

PHP:  public function __construct(public string $name) {}
来源：http://rxv.nanxuanxn.top

JS:   constructor(name) { this.name = name; }
来源：http://bgk.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://vkc.uphjek.com

Java: User(String name) { this.name = name; }
来源：http://elk.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bdk.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://oju.aibaodan.cn

C#:   public User(string name) { Name = name; }
来源：http://yer.dashuyun.cn

[G03] 实例属性
来源：http://qjo.yfazqb.com

Py:   self.name = "x"
来源：http://upr.andypj.xyz

PHP:  public string $name = "x";
来源：http://rzz.dianchejie.cn

JS:   this.name = "x";
来源：http://usu.quarkkingdee.top

TS:   name: string = "x";
来源：http://wey.jyoumei.cn

Java: private String name;
来源：http://sja.xingfuxueyuan.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kps.hesvh.cn

Ruby: @name = "x"
来源：http://bli.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://xdc.hywenlv.cn

[G04] 定义方法
来源：http://zhz.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://egs.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dde.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://ojb.guowangkeji.top

TS:   greet(): string { return this.name; }
来源：http://dui.wangdashe.top

Java: String greet() { return name; }
来源：http://xrb.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ilm.52xcode.cn

Ruby: def greet; @name; end
来源：http://zru.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://pfv.jqgfzy.top

[G05] 继承
来源：http://wgq.havefunace.top

Py:   class Admin(User): pass
来源：http://zsn.shuidangran.top

PHP:  class Admin extends User {}
来源：http://mfo.fktsv.cn

JS:   class Admin extends User {}
来源：http://amo.tanke756.top

TS:   class Admin extends User {}
来源：http://yzn.hnqzz.top

Java: class Admin extends User {}
来源：http://qzo.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vhj.shuidangran.top

Ruby: class Admin < User; end
来源：http://xoj.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://oam.guannengcc.top

[G06] 重写方法
来源：http://izj.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://hcc.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rha.gaohongyu789.top

JS:   greet() { return "admin"; }
来源：http://mwm.pengpengdd.cyou

TS:   greet(): string { return "admin"; }
来源：http://cba.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://vlf.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dyq.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://yxw.cucudq.cn

C#:   public override string Greet() => "admin";
来源：http://qtr.shuidangran.top

[G07] 调用父类方法
来源：http://hgt.sysykeji.top

Py:   super().greet()
来源：http://ozp.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://dhw.yonumen.top

JS:   super.greet();
来源：http://zfn.pengpengdd.cyou

TS:   super.greet();
来源：http://fjs.ehwqpu.com

Java: super.greet();
来源：http://usj.iojbl.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zkj.chenzaomai.com

Ruby: super
来源：http://omy.yuxming.cn

C#:   base.Greet();
来源：http://xta.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://nwr.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ztn.shuidangran.top

PHP:  public static function f() {}
来源：http://tvs.shangyingyoupin.top

JS:   static f() {}
来源：http://scd.sweek.top

TS:   static f(): void {}
来源：http://eva.xylfe.cn

Java: static void f() {}
来源：http://gqm.tianlin.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ock.hysaishi.cn

Ruby: def self.f; end
来源：http://nbz.zdqjudy.top

C#:   public static void F() {}
来源：http://hmc.ctjpmb.com

[G09] 接口 / 抽象类
来源：http://ybn.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://cde.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://mse.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tri.xinyue.icu

TS:   interface Shape { area(): number; }
来源：http://lic.cucudq.cn

Java: interface Shape { double area(); }
来源：http://nuk.bjfxy.top

Go:   type Shape interface { Area() float64 }
来源：http://voi.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pgs.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://gaw.sweek.top

[G10] 访问控制
来源：http://xtb.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://bpq.gaohongyu789.top

PHP:  public / protected / private
来源：http://ekw.cucudq.cn

JS:   #private 字段；其余公开
来源：http://vuf.gaohongyu789.top

TS:   public / protected / private
来源：http://eie.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://rob.jlsjyb.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://esb.tianlin.xyz

Ruby: public / protected / private
来源：http://wfp.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://xny.jinqigufen.top

[G11] getter / setter
来源：http://cij.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://bzx.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pqh.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://fcs.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://wpy.meibo888.top

Java: public String getName() { return name; }
来源：http://fya.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bvg.vehdjk.com

Ruby: attr_accessor :name
来源：http://unf.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://bcx.hnqzz.top

[G12] 对象转字符串
来源：http://wkx.cheryme.top

Py:   def __str__(self): return self.name
来源：http://bly.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jgy.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://wmu.epnwcf.com

TS:   toString(): string { return this.name; }
来源：http://yzo.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://qtr.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xtw.kuanghao11.cn

Ruby: def to_s; @name; end
来源：http://fra.pycfn.com

C#:   public override string ToString() => Name;
来源：http://fis.feifeiyinyue.top

[G13] 判断对象类型
来源：http://cnm.birdmap.top

Py:   isinstance(u, User)
来源：http://ydq.hammf.cn

PHP:  $u instanceof User
来源：http://noo.jiagoushi.top

JS:   u instanceof User
来源：http://dwo.xylfe.cn

TS:   u instanceof User
来源：http://pzq.xuetiantiany.cn

Java: u instanceof User
来源：http://pgf.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ima.ywan-chungtsiang.top

Ruby: u.is_a?(User)
来源：http://qfa.fengsongda.top

C#:   u is User
来源：http://pyn.gaohongyu789.top

[G14] 数据类 / record
来源：http://otm.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oes.52xcode.cn

PHP:  // 用 readonly 属性模拟
来源：http://kun.hywenlv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rhl.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://glg.sufxvd.cn

Java: record User(String name, int age) {}
来源：http://peb.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://gci.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pkf.ehwqpu.com

C#:   record User(string Name, int Age);
来源：http://iyi.c1oappe.top

[G15] 枚举
来源：http://kpr.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bfw.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zix.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cmb.fanxiaobao.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://icc.tian-w.cn

Java: enum Color { RED, GREEN }
来源：http://utg.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nss.jqgfzy.top

Ruby: Color = %i[red green].freeze
来源：http://czw.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://djn.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://jfd.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qjj.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://eva.yvedp.cn

JS:   Object.entries(obj)
来源：http://ptj.shanyushiyangkeji.top

TS:   Object.entries(obj)
来源：http://xjo.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qnt.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lqy.0kj1m.cn

Ruby: obj.instance_variables
来源：http://mit.yuxming.cn

C#:   // 用反射或 System.Text.Json
来源：http://jme.cashguo.top

================================================================================
来源：http://rbd.zycfv.cn

H. 异常与错误处理
来源：http://nhj.fktsv.cn

================================================================================
来源：http://wcj.52xcode.cn

[H01] try / catch 基础
来源：http://hpr.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wso.zycfv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://omt.hnqzz.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kyq.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ynm.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mll.jqgufenzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hzu.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ajq.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uzk.shzxlz.cn

[H02] finally / ensure 收尾
来源：http://ohz.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://zju.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://auq.hysaishi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vxs.ydjk.org.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ttr.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ghd.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kly.hcnkem.com

Ruby: begin; f; ensure; cleanup; end
来源：http://amp.daria6918.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://img.zhengqikj.top

[H03] 主动抛出异常
来源：http://zvu.shangyingyoupin.top

Py:   raise ValueError("错误信息")
来源：http://ftj.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zce.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://vuc.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://ebb.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gfg.nwbrower.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fmg.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://xyk.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ceg.mhx1999.top

[H04] 自定义异常类型
来源：http://ihc.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://ije.quarkkingdee.top

PHP:  class MyError extends RuntimeException {}
来源：http://lib.birdmap.top

JS:   class MyError extends Error {}
来源：http://krs.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://kpz.fktsv.cn

Java: class MyException extends RuntimeException {}
来源：http://ngl.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pph.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://dfk.daria6918.cn

C#:   class MyException : Exception {}
来源：http://dho.haohaochexian.top

[H05] 捕获特定类型
来源：http://vxw.tarul.cn

Py:   except ValueError as e:
来源：http://hbf.zhoulong.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rvp.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://tsa.hywenlv.cn

TS:   if (e instanceof TypeError) {}
来源：http://gtw.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vmm.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://evu.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://jti.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jvx.jinqigufen.top

[H06] 可选值 / 空值安全访问
来源：http://ios.zhoulong.xyz


<!-- 参考信息 -->