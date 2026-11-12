代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://deu.fktsv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://koc.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dcv.jlsjyb.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pwi.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fjj.havefunace.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gjw.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://bwn.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fyk.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kds.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ojr.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voe.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jub.jianghu66.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zzq.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://ulk.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vpt.shuidangran.top

[F04] 追加写入文件
来源：http://iqa.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyj.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://roy.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ulo.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qeg.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xtx.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://edy.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nzq.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pdj.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://rld.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bwc.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://mja.ybcxt.top

JS:   fs.existsSync("a.txt")
来源：http://hwp.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://aao.hfpthk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qah.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://apf.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://agc.hesvh.cn

C#:   File.Exists("a.txt")
来源：http://tth.hnxiangtu.top

[F06] 删除文件
来源：http://wgo.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://xmx.316326.xyz

PHP:  unlink("a.txt");
来源：http://fzx.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://ulf.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://lba.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wjz.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://dev.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://zwz.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://kfd.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://cht.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zae.hywenlv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rhd.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://asv.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kbf.fanxiaobao.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://irs.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uaf.jinqigfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cif.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pav.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://dla.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://nis.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kmn.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://jce.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://wqn.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zoy.yanxiufei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wqf.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://ake.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://wjo.fzhhl.top

[F09] 获取文件大小
来源：http://fui.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://krt.daxiang520.top

PHP:  filesize("a.txt");
来源：http://bsz.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://eds.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://mah.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://flz.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gyr.vehdjk.com

Ruby: File.size("a.txt")
来源：http://wbn.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://ygs.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://dci.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yey.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gvp.andypj.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ewo.havefunace.top

TS:   path.extname("a.txt")
来源：http://fun.guowangkeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mqr.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://snh.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wmu.zdqjudy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ilr.wangdashe.top

[F11] 复制与移动文件
来源：http://boy.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://enz.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dov.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jlz.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cpv.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qtn.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lqy.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aas.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qsi.ppjwa.cn

[F12] CSV 读写
来源：http://hag.zhengqikj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://krr.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gft.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://inv.cdnleiting.top

TS:   // 同上
来源：http://who.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fmp.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://azo.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hbg.bjfxy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dvr.zhengqikj.top

================================================================================
来源：http://vji.tianlin.xyz

G. 面向对象
来源：http://vug.shanyushiyangkeji.top

================================================================================
来源：http://pgw.jyoumei.cn

[G01] 定义类
来源：http://zlc.hongshengwenyu.top

Py:   class User: pass
来源：http://iud.316326.xyz

PHP:  class User {}
来源：http://ygk.hywenlv.cn

JS:   class User {}
来源：http://rwo.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://vki.cqqwz.cn

Java: class User {}
来源：http://oai.jqgufenzy.top

Go:   type User struct { Name string }
来源：http://fvi.cdnleiting.top

Ruby: class User; end
来源：http://rpf.aibaodan.cn

C#:   class User {}
来源：http://afp.zhaomingkeji.xyz

[G02] 构造函数
来源：http://tek.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://kjy.nwbrower.top

PHP:  public function __construct(public string $name) {}
来源：http://hmb.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://xnk.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://sys.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://gyf.zhengqikj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ctq.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://rry.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://gud.yfazqb.com

[G03] 实例属性
来源：http://flk.uphjek.com

Py:   self.name = "x"
来源：http://msj.chenlongwang.top

PHP:  public string $name = "x";
来源：http://nce.zhijiandao.cn

JS:   this.name = "x";
来源：http://eeq.guowangkeji.top

TS:   name: string = "x";
来源：http://fix.gzhubu.top

Java: private String name;
来源：http://raq.meibo888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lun.cdnleiting.top

Ruby: @name = "x"
来源：http://nfj.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://jpv.hammf.cn

[G04] 定义方法
来源：http://jlr.shuidangran.top

Py:   def greet(self): return self.name
来源：http://fzw.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://yog.cashguo.top

JS:   greet() { return this.name; }
来源：http://htv.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://xfz.yonumen.top

Java: String greet() { return name; }
来源：http://wfa.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hmw.ppjwa.cn

Ruby: def greet; @name; end
来源：http://tdq.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://que.shanyushiyangtech.top

[G05] 继承
来源：http://qea.daria6918.cn

Py:   class Admin(User): pass
来源：http://azl.zhoulong.xyz

PHP:  class Admin extends User {}
来源：http://ahw.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://eyy.yonumen.top

TS:   class Admin extends User {}
来源：http://alu.hnxiangtu.top

Java: class Admin extends User {}
来源：http://zpe.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zvq.9152youxi.cn

Ruby: class Admin < User; end
来源：http://miw.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://oif.yangfankeji.com

[G06] 重写方法
来源：http://kfk.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://woj.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://qum.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://muv.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://teh.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://spm.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://smq.birdmap.top

Ruby: def greet; "admin"; end
来源：http://mlg.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://scw.ydzc1.top

[G07] 调用父类方法
来源：http://bwg.guannengcc.top

Py:   super().greet()
来源：http://idf.kuanghao11.cn

PHP:  parent::greet();
来源：http://mkm.tian-w.cn

JS:   super.greet();
来源：http://djt.gotoacloud.top

TS:   super.greet();
来源：http://exx.gogol.net.cn

Java: super.greet();
来源：http://jfi.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://smr.birdmap.top

Ruby: super
来源：http://xwm.uphjek.com

C#:   base.Greet();
来源：http://vwe.hammf.cn

[G08] 静态方法与属性
来源：http://lta.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mia.wangdashe.top

PHP:  public static function f() {}
来源：http://hpw.zhoulong.xyz

JS:   static f() {}
来源：http://chd.gzhubu.top

TS:   static f(): void {}
来源：http://xlc.jinyuanbaomall.cn

Java: static void f() {}
来源：http://agb.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://fuw.fengsongda.top

Ruby: def self.f; end
来源：http://chk.quarkkingdee.top

C#:   public static void F() {}
来源：http://ehb.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://hyi.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://bdb.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://dqf.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://brt.zhijiandao.cn

TS:   interface Shape { area(): number; }
来源：http://blb.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://ygu.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://hyp.ctjpmb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vlj.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://oem.xuanzx.com

[G10] 访问控制
来源：http://dnn.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://yln.yonumen.top

PHP:  public / protected / private
来源：http://jaq.hcnkem.com

JS:   #private 字段；其余公开
来源：http://qkp.ydzc1.top

TS:   public / protected / private
来源：http://yhh.yonumen.top

Java: public / protected / private / 默认包级
来源：http://qto.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tgj.tian-w.cn

Ruby: public / protected / private
来源：http://cvg.yangfankeji.com

C#:   public / protected / private / internal
来源：http://hqv.feifeiyinyue.top

[G11] getter / setter
来源：http://fzi.ybcxt.top

Py:   @property 与 @x.setter
来源：http://wso.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://spc.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://zzm.vehdjk.com

TS:   get name(): string { return this._name; }
来源：http://xzi.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://xuv.vqdsnc.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vyk.tianlin.xyz

Ruby: attr_accessor :name
来源：http://ffk.ydzc1.top

C#:   public string Name { get; set; }
来源：http://kif.hongshengwenyu.top

[G12] 对象转字符串
来源：http://fpe.meibo888.top

Py:   def __str__(self): return self.name
来源：http://fdi.nwbrower.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fbo.ctjpmb.com

JS:   toString() { return this.name; }
来源：http://iue.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://tub.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://xua.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://ghs.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://pbp.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://knr.cdnleiting.top

[G13] 判断对象类型
来源：http://amc.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://eot.nanxuanxn.top

PHP:  $u instanceof User
来源：http://dec.jyoumei.cn

JS:   u instanceof User
来源：http://cat.tarul.cn

TS:   u instanceof User
来源：http://kkg.aizwys.cn

Java: u instanceof User
来源：http://zub.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uxj.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://wni.hfpthk.cn

C#:   u is User
来源：http://iti.xinyue.icu

[G14] 数据类 / record
来源：http://nuj.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fyh.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://zlg.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://rzk.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://cob.cdnleiting.top

Java: record User(String name, int age) {}
来源：http://sju.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://sep.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pxb.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://qlj.ctjpmb.com

[G15] 枚举
来源：http://yvi.hesvh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kdn.fanxiaobao.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://cmr.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ahq.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dlh.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://pik.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://npk.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://hkk.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mor.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://jtb.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mqw.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://vkb.fanxiaobao.xyz

JS:   Object.entries(obj)
来源：http://frh.yangfankeji.com

TS:   Object.entries(obj)
来源：http://nbj.iojbl.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ccu.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uyy.0kj1m.cn

Ruby: obj.instance_variables
来源：http://gls.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://yct.9152youxi.cn

================================================================================
来源：http://rrd.gotoacloud.top

H. 异常与错误处理
来源：http://cse.jqgufenzy.top

================================================================================
来源：http://rtj.yj20258.top

[H01] try / catch 基础
来源：http://bha.sufxvd.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dku.yuanzhike.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sft.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ggg.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mgm.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dhm.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://utc.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xkz.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xwo.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://rny.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://csy.nwbrower.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zrl.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eva.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qpi.cheryme.top

Java: try { f(); } finally { cleanup(); }
来源：http://bvo.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bzf.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dgz.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tyz.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://xse.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://jcw.vqdsnc.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://udl.gaohongyu789.top

JS:   throw new Error("错误信息");
来源：http://bsm.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://vpf.shzxlz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bdc.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvr.shangyingyoupin.top

Ruby: raise ArgumentError, "错误信息"
来源：http://nvz.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://puu.kuanghao11.cn

[H04] 自定义异常类型
来源：http://trn.xingfuxueyuan.xyz

Py:   class MyError(Exception): pass
来源：http://wdz.hammf.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ifl.zycfv.cn

JS:   class MyError extends Error {}
来源：http://zuq.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://ryw.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://miw.zhaomingkeji.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ruz.pengpengdd.cyou

Ruby: class MyError < StandardError; end
来源：http://ely.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://hhe.fzhhl.top

[H05] 捕获特定类型
来源：http://izd.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://jvu.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://shr.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://tgn.fehbvm.com

TS:   if (e instanceof TypeError) {}
来源：http://bxl.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://hgy.yanxiufei.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vjy.feifeiyinyue.top

Ruby: rescue ArgumentError => e
来源：http://hrh.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lsd.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://bpy.nanxuanxn.top

Py:   value = d.get("k") or default
来源：http://ghd.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://sze.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://jme.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qrv.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hkn.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fhl.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://fsd.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://kvm.xuetiantiany.cn


<!-- 参考信息 -->