代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://qcj.redwolf501.top

[F02] 逐行读取文件
来源：http://rbr.ybcxt.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bzc.zhoulong.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://imj.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pys.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yvg.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://atp.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://khh.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cyk.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rtk.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://ecs.fehbvm.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uan.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wsn.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpu.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ync.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cri.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bme.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://uzg.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uoe.nwbrower.top

[F04] 追加写入文件
来源：http://aqi.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oof.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gxf.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vlg.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yma.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dhj.tanke756.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jde.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xzj.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xwg.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://qkq.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://abk.tanke756.top

PHP:  file_exists("a.txt");
来源：http://hhk.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://qed.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://jvk.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vbm.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tsj.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://qqt.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://yyb.kuanghao11.cn

[F06] 删除文件
来源：http://lbm.zycfv.cn

Py:   os.remove("a.txt")
来源：http://vmo.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://xeg.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://ywf.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://nlo.chenlongwang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qyn.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://ibn.meibo888.top

Ruby: File.delete("a.txt")
来源：http://njg.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://njf.pengpengdd.cyou

[F07] 创建目录（含多级）
来源：http://lvt.bbcook.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ctp.cqqwz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://maz.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://umc.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjl.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nsg.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ugq.guannengcc.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rwc.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jhn.zhixingplan.top

[F08] 遍历目录
来源：http://ynt.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ers.hammf.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zrg.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://kxp.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://pmh.yanxiufei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mpt.ybcxt.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ihp.chenlongwang.top

Ruby: Dir.children("dir")
来源：http://enh.ybcxt.top

C#:   Directory.GetFiles("dir")
来源：http://axe.svipenyu.cn

[F09] 获取文件大小
来源：http://rky.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://qbn.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://wjg.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://dwv.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://wrj.yongpay.top

Java: Files.size(Path.of("a.txt"))
来源：http://ndh.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sbb.yuxming.cn

Ruby: File.size("a.txt")
来源：http://ksw.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://juy.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://sua.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eal.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aav.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msg.xinyue.icu

TS:   path.extname("a.txt")
来源：http://wze.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pmj.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wlw.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jsa.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lbw.ivvv.top

[F11] 复制与移动文件
来源：http://kzf.yj20258.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pnx.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ldb.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fvz.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hmt.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fks.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://omq.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wlx.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zse.jqgfzy.top

[F12] CSV 读写
来源：http://cmt.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qid.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://trt.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ozz.daria6918.cn

TS:   // 同上
来源：http://bab.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://muy.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ect.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fei.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://utt.gzhubu.top

================================================================================
来源：http://zvw.gaohongyu789.top

G. 面向对象
来源：http://pfd.nwbrower.top

================================================================================
来源：http://xxt.iojbl.cn

[G01] 定义类
来源：http://dhn.havefunace.top

Py:   class User: pass
来源：http://rrt.ctjpmb.com

PHP:  class User {}
来源：http://nwl.chenjidiqi.icu

JS:   class User {}
来源：http://fej.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://zit.jinqigfzy.top

Java: class User {}
来源：http://ffp.cucudq.cn

Go:   type User struct { Name string }
来源：http://zyj.fanxiaobao.xyz

Ruby: class User; end
来源：http://uju.zhixingplan.top

C#:   class User {}
来源：http://fgk.yvedp.cn

[G02] 构造函数
来源：http://dah.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://spx.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://luf.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://xjh.cashguo.top

TS:   constructor(public name: string) {}
来源：http://vts.zhoulong.xyz

Java: User(String name) { this.name = name; }
来源：http://etz.fehbvm.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cdy.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://ibk.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://vwr.shangyingyoupin.top

[G03] 实例属性
来源：http://nka.andypj.xyz

Py:   self.name = "x"
来源：http://erb.ivvv.top

PHP:  public string $name = "x";
来源：http://ayz.chenlongwang.top

JS:   this.name = "x";
来源：http://ary.cdnleiting.top

TS:   name: string = "x";
来源：http://kqw.hysaishi.cn

Java: private String name;
来源：http://qhn.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jvb.ppjwa.cn

Ruby: @name = "x"
来源：http://oya.meibo888.top

C#:   public string Name { get; set; } = "x";
来源：http://ong.jinqigufen.top

[G04] 定义方法
来源：http://keg.mhx1999.top

Py:   def greet(self): return self.name
来源：http://udl.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qqm.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://arl.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://vju.zhongyouzk.top

Java: String greet() { return name; }
来源：http://qfc.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ssz.redwolf501.top

Ruby: def greet; @name; end
来源：http://wqn.jinghuilouyu.cn

C#:   public string Greet() => Name;
来源：http://dge.jinyuanbaomall.cn

[G05] 继承
来源：http://fur.sysykeji.top

Py:   class Admin(User): pass
来源：http://qmi.iojbl.cn

PHP:  class Admin extends User {}
来源：http://yqs.zdbjq.cn

JS:   class Admin extends User {}
来源：http://rrg.iojbl.cn

TS:   class Admin extends User {}
来源：http://pua.zhijiandao.cn

Java: class Admin extends User {}
来源：http://mhr.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kjd.shzxlz.cn

Ruby: class Admin < User; end
来源：http://hkr.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://nej.fanxiaobao.xyz

[G06] 重写方法
来源：http://evf.cashguo.top

Py:   def greet(self): return "admin"
来源：http://bno.yuanzhike.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ago.ybcxt.top

JS:   greet() { return "admin"; }
来源：http://fds.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://clu.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://odi.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zjm.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://rqg.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://zqv.sxryk.cn

[G07] 调用父类方法
来源：http://xfo.xziqi.cn

Py:   super().greet()
来源：http://hjy.yangfankeji.com

PHP:  parent::greet();
来源：http://fts.tianlin.xyz

JS:   super.greet();
来源：http://woh.daria6918.cn

TS:   super.greet();
来源：http://non.fehbvm.com

Java: super.greet();
来源：http://odd.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uzt.tarul.cn

Ruby: super
来源：http://ctc.jianghu66.top

C#:   base.Greet();
来源：http://uvh.hammf.cn

[G08] 静态方法与属性
来源：http://vsm.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zct.zdqjudy.top

PHP:  public static function f() {}
来源：http://ujj.cheryme.top

JS:   static f() {}
来源：http://yee.316326.xyz

TS:   static f(): void {}
来源：http://gvd.zhaomingkeji.xyz

Java: static void f() {}
来源：http://jcg.zdbjq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jne.birdmap.top

Ruby: def self.f; end
来源：http://fkp.gzhubu.top

C#:   public static void F() {}
来源：http://rrh.meibo888.top

[G09] 接口 / 抽象类
来源：http://zbo.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://xtp.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://nss.vehdjk.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://vam.sxryk.cn

TS:   interface Shape { area(): number; }
来源：http://cxh.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://xdq.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://qnx.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nfo.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://cgf.0kj1m.cn

[G10] 访问控制
来源：http://umm.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://mll.yuanzhike.top

PHP:  public / protected / private
来源：http://fls.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://tge.sweek.top

TS:   public / protected / private
来源：http://wwp.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://git.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewc.zdqjudy.top

Ruby: public / protected / private
来源：http://rlb.chenlongwang.top

C#:   public / protected / private / internal
来源：http://sad.gzhubu.top

[G11] getter / setter
来源：http://bpl.hnqzz.top

Py:   @property 与 @x.setter
来源：http://znj.nanxinkj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hpw.hesvh.cn

JS:   get name() { return this._name; }
来源：http://wam.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://uje.sjlbkw.cn

Java: public String getName() { return name; }
来源：http://ntq.yongpay.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://pne.meibo888.top

Ruby: attr_accessor :name
来源：http://rhm.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://wnj.hysaishi.cn

[G12] 对象转字符串
来源：http://wgg.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://gzc.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jge.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://tcq.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://kes.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://dqj.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://mls.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://qob.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://buc.tarul.cn

[G13] 判断对象类型
来源：http://yqm.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://rtp.c1oappe.top

PHP:  $u instanceof User
来源：http://kay.fanxiaobao.xyz

JS:   u instanceof User
来源：http://bkb.jqgfzy.top

TS:   u instanceof User
来源：http://uis.feifeiyinyue.top

Java: u instanceof User
来源：http://hmh.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mel.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://jzk.dianchejie.cn

C#:   u is User
来源：http://bpo.uphjek.com

[G14] 数据类 / record
来源：http://wid.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ria.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://kdm.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ncr.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://sfx.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://rgw.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://deo.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ihb.zhixingplan.top

C#:   record User(string Name, int Age);
来源：http://auh.ywan-chungtsiang.top

[G15] 枚举
来源：http://uxh.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bpt.zhiwuduotai.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xhg.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cvu.jinqigufen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dnr.jqgfzy.top

Java: enum Color { RED, GREEN }
来源：http://jwy.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tyo.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://awr.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ghz.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://kst.snrcjt.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ngg.c1oappe.top

PHP:  get_object_vars($obj);
来源：http://bea.kuanghao11.cn

JS:   Object.entries(obj)
来源：http://tcg.fktsv.cn

TS:   Object.entries(obj)
来源：http://ceb.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nde.vehdjk.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://vbj.shanyushiyangkeji.top

Ruby: obj.instance_variables
来源：http://ewi.gaohongyu789.top

C#:   // 用反射或 System.Text.Json
来源：http://dtx.hnxiangtu.top

================================================================================
来源：http://ljk.fehbvm.com

H. 异常与错误处理
来源：http://psz.yuanzhike.top

================================================================================
来源：http://die.nwbrower.top

[H01] try / catch 基础
来源：http://rhp.ivvv.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tnu.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nhm.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wqf.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zds.yuanzhike.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://urj.0kj1m.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ere.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eqj.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://plq.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://jjn.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://cmb.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hcj.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kvm.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://lnm.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://feo.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uhw.iojbl.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hhh.bbcook.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fvo.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://vst.ivvv.top

Py:   raise ValueError("错误信息")
来源：http://adp.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://riz.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://ukp.vqdsnc.cn

TS:   throw new Error("错误信息");
来源：http://ixg.havefunace.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://eae.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kbt.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ixx.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://jyl.zhengqikj.top

[H04] 自定义异常类型
来源：http://pcs.xylfe.cn

Py:   class MyError(Exception): pass
来源：http://vbd.guowangkeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://rkx.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://yhe.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://tbr.zhoulong.xyz

Java: class MyException extends RuntimeException {}
来源：http://dpc.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xhf.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://cqw.nwbrower.top

C#:   class MyException : Exception {}
来源：http://cil.yanxiufei.cn

[H05] 捕获特定类型
来源：http://dpc.xylfe.cn

Py:   except ValueError as e:
来源：http://lna.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tci.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://nvo.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://kdr.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://hyv.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sqc.xuanzx.com

Ruby: rescue ArgumentError => e
来源：http://ckz.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jbg.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://wxh.316326.xyz

Py:   value = d.get("k") or default
来源：http://yqt.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://kfr.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://upe.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://izd.fehbvm.com


<!-- 参考信息 -->