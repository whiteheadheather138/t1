代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://jha.cdnleiting.top

[F02] 逐行读取文件
来源：http://hmw.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ezw.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zri.epnwcf.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://abz.tarul.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ktx.ctjpmb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://idb.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nas.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mrq.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lhy.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://qtp.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ntf.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://phd.jinqigufen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ldn.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nrs.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fab.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yey.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://fvr.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hpm.aizwys.cn

[F04] 追加写入文件
来源：http://kbx.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wfj.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yau.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kca.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yza.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ehc.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rgr.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ubg.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fri.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://cpb.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://siw.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://dzx.xinyue.icu

JS:   fs.existsSync("a.txt")
来源：http://ovz.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://mkk.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oob.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uct.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://hve.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://lfj.sjlbkw.cn

[F06] 删除文件
来源：http://lnn.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://xib.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://lsh.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://ong.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://msg.shangyingyoupin.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fyh.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://sjr.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://ztb.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://fur.jianghu66.top

[F07] 创建目录（含多级）
来源：http://qxq.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hyi.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iyt.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iqc.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://okj.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sbl.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kla.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cgh.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ivz.jinqigfzy.top

[F08] 遍历目录
来源：http://xrk.gzhubu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yos.xinyue.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ugw.sufxvd.cn

JS:   fs.readdirSync("dir")
来源：http://ylf.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://zvd.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bvg.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qlb.andypj.xyz

Ruby: Dir.children("dir")
来源：http://knr.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://irh.jqgufenzy.top

[F09] 获取文件大小
来源：http://nqe.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://bpg.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://vsd.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://czz.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://ojb.zycfv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hdh.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pug.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://oud.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://zpb.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ant.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bqo.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ads.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ysv.daria6918.cn

TS:   path.extname("a.txt")
来源：http://rkr.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nfa.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nvx.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lrb.haohaochexian.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yuy.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://xvq.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qdp.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://alz.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://enr.ydzc1.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mke.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://znu.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://euq.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nsw.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cwe.yj202588.top

[F12] CSV 读写
来源：http://nbk.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hdu.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dhy.uphjek.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://evp.yangfankeji.com

TS:   // 同上
来源：http://fsp.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://trp.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tue.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tqe.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uur.fzhhl.top

================================================================================
来源：http://sjs.tianlin.xyz

G. 面向对象
来源：http://ptf.gzhubu.top

================================================================================
来源：http://bcu.zhijiandao.cn

[G01] 定义类
来源：http://cmn.pengpengdd.cyou

Py:   class User: pass
来源：http://tva.jinyuanbaomall.cn

PHP:  class User {}
来源：http://zak.jlsjyb.cn

JS:   class User {}
来源：http://jmj.tanke756.top

TS:   class User { name: string = ""; }
来源：http://oxh.uphjek.com

Java: class User {}
来源：http://euf.bjfxy.top

Go:   type User struct { Name string }
来源：http://ogo.zhiwuduotai.top

Ruby: class User; end
来源：http://xhh.quarkkingdee.top

C#:   class User {}
来源：http://swd.zhengqikj.top

[G02] 构造函数
来源：http://bzz.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://lwp.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://mgo.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://dxg.meibo888.top

TS:   constructor(public name: string) {}
来源：http://tgb.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://uao.haohaochexian.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fbn.nwbrower.top

Ruby: def initialize(name); @name = name; end
来源：http://vzu.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://svx.cashguo.top

[G03] 实例属性
来源：http://bdy.gogol.net.cn

Py:   self.name = "x"
来源：http://yzi.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://moe.yfazqb.com

JS:   this.name = "x";
来源：http://uym.sufxvd.cn

TS:   name: string = "x";
来源：http://jlt.hnxiangtu.top

Java: private String name;
来源：http://ajv.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rnr.zhengqikj.top

Ruby: @name = "x"
来源：http://lyq.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://gmk.svipenyu.cn

[G04] 定义方法
来源：http://ieq.c1oappe.top

Py:   def greet(self): return self.name
来源：http://bra.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xfd.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://ctz.tanke756.top

TS:   greet(): string { return this.name; }
来源：http://cqd.wangdashe.top

Java: String greet() { return name; }
来源：http://hel.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oxn.yongpay.top

Ruby: def greet; @name; end
来源：http://odp.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://nre.wangshuangyany.cn

[G05] 继承
来源：http://ewf.bbcook.cn

Py:   class Admin(User): pass
来源：http://lkw.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://aps.vqdsnc.cn

JS:   class Admin extends User {}
来源：http://foj.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://btx.9152youxi.cn

Java: class Admin extends User {}
来源：http://igr.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://eqx.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://poz.smart0.xyz

C#:   class Admin : User {}
来源：http://key.uphjek.com

[G06] 重写方法
来源：http://sxx.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://fzf.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://clo.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://rck.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://pwx.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://jgy.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kso.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://icb.hnxiangtu.top

C#:   public override string Greet() => "admin";
来源：http://kwh.yvedp.cn

[G07] 调用父类方法
来源：http://huw.sysykeji.top

Py:   super().greet()
来源：http://qjw.sjlbkw.cn

PHP:  parent::greet();
来源：http://ufh.haohaochexian.top

JS:   super.greet();
来源：http://cae.daxiang520.top

TS:   super.greet();
来源：http://dov.uphjek.com

Java: super.greet();
来源：http://kpw.daria6918.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xlb.zhengqikj.top

Ruby: super
来源：http://ose.ydzc1.top

C#:   base.Greet();
来源：http://nys.aizwys.cn

[G08] 静态方法与属性
来源：http://wiy.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ccl.tanke756.top

PHP:  public static function f() {}
来源：http://wnp.ctjpmb.com

JS:   static f() {}
来源：http://kkq.yongpay.top

TS:   static f(): void {}
来源：http://php.jinghuilouyu.cn

Java: static void f() {}
来源：http://ddk.guowangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cli.yuxming.cn

Ruby: def self.f; end
来源：http://rcf.hesvh.cn

C#:   public static void F() {}
来源：http://mqo.yj20258888.top

[G09] 接口 / 抽象类
来源：http://qka.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://hhh.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://klo.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vtm.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://scs.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://jjb.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://guq.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hmm.sweek.top

C#:   interface IShape { double Area(); }
来源：http://zkk.nanxuanxn.top

[G10] 访问控制
来源：http://ppj.ybcxt.top

Py:   约定 _protected / __private（不强制）
来源：http://vso.feifeiyinyue.top

PHP:  public / protected / private
来源：http://ell.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://ecr.yanxiufei.cn

TS:   public / protected / private
来源：http://uwt.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://uvy.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xtl.xylfe.cn

Ruby: public / protected / private
来源：http://rtl.gotoacloud.top

C#:   public / protected / private / internal
来源：http://elb.daria6918.cn

[G11] getter / setter
来源：http://rfu.iojbl.cn

Py:   @property 与 @x.setter
来源：http://hvw.gogol.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://trb.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://xlx.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://gic.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://zzq.sweek.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hya.mhx1999.top

Ruby: attr_accessor :name
来源：http://vrx.cqqwz.cn

C#:   public string Name { get; set; }
来源：http://jey.chenzaomai.com

[G12] 对象转字符串
来源：http://lvw.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://duu.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://gyt.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://ulh.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://vgg.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://izd.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uiq.mhx1999.top

Ruby: def to_s; @name; end
来源：http://vxl.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://ndh.cdnleiting.top

[G13] 判断对象类型
来源：http://sbm.zhixingplan.top

Py:   isinstance(u, User)
来源：http://jtb.nanxinkj.top

PHP:  $u instanceof User
来源：http://dwo.bjfxy.top

JS:   u instanceof User
来源：http://eat.cashguo.top

TS:   u instanceof User
来源：http://vjj.tian-w.cn

Java: u instanceof User
来源：http://zaj.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://txo.aizwys.cn

Ruby: u.is_a?(User)
来源：http://asc.xinyue.icu

C#:   u is User
来源：http://rza.redwolf501.top

[G14] 数据类 / record
来源：http://ymq.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgg.yj20258.top

PHP:  // 用 readonly 属性模拟
来源：http://ugd.shuidangran.top

JS:   // 无内置：普通类或对象字面量
来源：http://rvh.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://jdg.fzhhl.top

Java: record User(String name, int age) {}
来源：http://noo.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://avi.fzhhl.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hyv.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://ukb.jiagoushi.top

[G15] 枚举
来源：http://cso.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pqa.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://taa.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mpi.zycfv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jbo.dianchejie.cn

Java: enum Color { RED, GREEN }
来源：http://jls.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oeh.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://rsp.shangyingyoupin.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wwz.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://mgp.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xqv.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://bcw.zdbjq.cn

JS:   Object.entries(obj)
来源：http://nvh.jiagoushi.top

TS:   Object.entries(obj)
来源：http://xlj.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://myi.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eun.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://ntw.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://mcx.nanxuanxn.top

================================================================================
来源：http://fjz.pycfn.com

H. 异常与错误处理
来源：http://edf.smart0.xyz

================================================================================
来源：http://pcn.fktsv.cn

[H01] try / catch 基础
来源：http://szb.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hhi.havefunace.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lbw.0kj1m.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bpb.epnwcf.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yap.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mws.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://avq.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zgv.zhiwuduotai.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qlx.yueranfly.top

[H02] finally / ensure 收尾
来源：http://czx.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://ayq.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zzw.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bkc.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qld.tanke756.top

Java: try { f(); } finally { cleanup(); }
来源：http://rvn.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yon.aibaodan.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yyv.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qim.sufxvd.cn

[H03] 主动抛出异常
来源：http://xub.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://txe.hnqzz.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mkc.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://ffl.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://ayf.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ofk.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wok.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gqo.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://grj.daria6918.cn

[H04] 自定义异常类型
来源：http://rad.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://ctb.jinqigufen.top

PHP:  class MyError extends RuntimeException {}
来源：http://tzs.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://wpy.52xcode.cn

TS:   class MyError extends Error {}
来源：http://ytv.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://jov.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iaz.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://uli.fengsongda.top

C#:   class MyException : Exception {}
来源：http://gos.wangdashe.top

[H05] 捕获特定类型
来源：http://ukk.jianghu66.top

Py:   except ValueError as e:
来源：http://ote.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jwk.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://dym.zdqjudy.top

TS:   if (e instanceof TypeError) {}
来源：http://tsy.yueranfly.top

Java: catch (IOException | SQLException e) {}
来源：http://zlg.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://llc.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://byb.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dto.sxryk.cn

[H06] 可选值 / 空值安全访问
来源：http://qsk.gzhubu.top

Py:   value = d.get("k") or default
来源：http://rbj.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ukf.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sex.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pyt.jinyuanbaomall.cn


<!-- 参考信息 -->