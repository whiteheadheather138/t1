代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cvr.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hje.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cnm.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bhd.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yaa.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cxa.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kzs.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzm.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://lff.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cmz.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://dft.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://pvh.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://dxv.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ihl.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nsc.daxiang520.top

Ruby: File.exist?("a.txt")
来源：http://qhf.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://zep.cqqwz.cn

[F06] 删除文件
来源：http://apt.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://yvs.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://zik.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://gyb.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://jxd.yfazqb.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lps.cashguo.top

Go:   os.Remove("a.txt")
来源：http://dpn.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://vvm.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://yrx.hesvh.cn

[F07] 创建目录（含多级）
来源：http://tdn.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wjh.xziqi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pci.52xcode.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ryg.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dns.ppjwa.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nqi.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rzt.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mch.jiagoushi.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ygt.redwolf501.top

[F08] 遍历目录
来源：http://suo.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fen.bbcook.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jnl.chenzaomai.com

JS:   fs.readdirSync("dir")
来源：http://uac.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://kyx.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tip.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sqe.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://cud.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://iti.fzhhl.top

[F09] 获取文件大小
来源：http://pzv.xinyue.icu

Py:   os.path.getsize("a.txt")
来源：http://ppp.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://hhd.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://ekq.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://hux.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://vkg.vehdjk.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uac.xuanzx.com

Ruby: File.size("a.txt")
来源：http://ucd.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://ofn.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://krt.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dxc.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wxs.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wus.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://kdb.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fuo.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://epo.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://red.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ane.ybcxt.top

[F11] 复制与移动文件
来源：http://pld.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oug.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wqh.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lzv.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://shj.gzhubu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zmd.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wod.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uif.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lgt.jianghu66.top

[F12] CSV 读写
来源：http://mqs.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ykw.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bou.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jzd.zhengqikj.top

TS:   // 同上
来源：http://xfo.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mms.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xct.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wtu.zhiwuduotai.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xiu.shangyingyoupin.top

================================================================================
来源：http://xbx.jqgfzy.top

G. 面向对象
来源：http://vwr.shanyushiyangtech.top

================================================================================
来源：http://lfk.cqqwz.cn

[G01] 定义类
来源：http://esm.chenlongwang.top

Py:   class User: pass
来源：http://aum.sysykeji.top

PHP:  class User {}
来源：http://qlq.jinqigfzy.top

JS:   class User {}
来源：http://wpd.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://egn.shuidangran.top

Java: class User {}
来源：http://ybi.zhengqikj.top

Go:   type User struct { Name string }
来源：http://uao.epnwcf.com

Ruby: class User; end
来源：http://tob.sjlbkw.cn

C#:   class User {}
来源：http://exq.yueranfly.top

[G02] 构造函数
来源：http://nli.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://bvb.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://vyh.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://iun.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://tab.tian-w.cn

Java: User(String name) { this.name = name; }
来源：http://ysb.guannengcc.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myr.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rtj.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://haq.hnqzz.top

[G03] 实例属性
来源：http://lje.316326.xyz

Py:   self.name = "x"
来源：http://maf.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://dre.pycfn.com

JS:   this.name = "x";
来源：http://uua.fzhhl.top

TS:   name: string = "x";
来源：http://eef.ppjwa.cn

Java: private String name;
来源：http://ywn.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tsz.hnxiangtu.top

Ruby: @name = "x"
来源：http://oob.wangdashe.top

C#:   public string Name { get; set; } = "x";
来源：http://cpa.sufxvd.cn

[G04] 定义方法
来源：http://maf.aibaodan.cn

Py:   def greet(self): return self.name
来源：http://okj.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wik.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://jlc.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://rmc.hammf.cn

Java: String greet() { return name; }
来源：http://prx.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ita.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://izy.jinqigfzy.top

C#:   public string Greet() => Name;
来源：http://gfo.yueranfly.top

[G05] 继承
来源：http://ifb.yj202588.top

Py:   class Admin(User): pass
来源：http://ybq.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://qmd.hfpthk.cn

JS:   class Admin extends User {}
来源：http://doz.xuanzx.com

TS:   class Admin extends User {}
来源：http://ajj.yanxiufei.cn

Java: class Admin extends User {}
来源：http://lmx.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vrb.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://aoh.dianchejie.cn

C#:   class Admin : User {}
来源：http://ida.cqqwz.cn

[G06] 重写方法
来源：http://gtn.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://hgx.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pvq.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://gou.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://xnv.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://xxm.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pyq.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://aav.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://fht.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://uzy.smart0.xyz

Py:   super().greet()
来源：http://iwk.sxryk.cn

PHP:  parent::greet();
来源：http://llo.xuetiantiany.cn

JS:   super.greet();
来源：http://vfs.xylfe.cn

TS:   super.greet();
来源：http://exm.zhongyouzk.top

Java: super.greet();
来源：http://uvg.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://guk.smart0.xyz

Ruby: super
来源：http://luh.birdmap.top

C#:   base.Greet();
来源：http://cun.hammf.cn

[G08] 静态方法与属性
来源：http://ryh.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xby.xziqi.cn

PHP:  public static function f() {}
来源：http://aez.nanxinkj.top

JS:   static f() {}
来源：http://par.cqqwz.cn

TS:   static f(): void {}
来源：http://tlo.gaohongyu789.top

Java: static void f() {}
来源：http://rcc.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tog.xuetiantiany.cn

Ruby: def self.f; end
来源：http://ddk.yj20258888.top

C#:   public static void F() {}
来源：http://quj.aizwys.cn

[G09] 接口 / 抽象类
来源：http://cfi.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://xuo.chenjidiqi.icu

PHP:  interface Shape { public function area(): float; }
来源：http://ahe.chenlongwang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xgr.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://nfd.iojbl.cn

Java: interface Shape { double area(); }
来源：http://cuv.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://swq.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://duu.chenzaomai.com

C#:   interface IShape { double Area(); }
来源：http://joh.zdqjudy.top

[G10] 访问控制
来源：http://ssp.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://mkg.jinqigufen.top

PHP:  public / protected / private
来源：http://iym.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://yma.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://ejs.cucudq.cn

Java: public / protected / private / 默认包级
来源：http://meu.kuanghao11.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://otu.pengpengdd.cyou

Ruby: public / protected / private
来源：http://ntt.aibaodan.cn

C#:   public / protected / private / internal
来源：http://afo.chenzaomai.com

[G11] getter / setter
来源：http://edq.c1oappe.top

Py:   @property 与 @x.setter
来源：http://fqc.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wdg.zycfv.cn

JS:   get name() { return this._name; }
来源：http://jkr.wangdashe.top

TS:   get name(): string { return this._name; }
来源：http://kda.zdqjudy.top

Java: public String getName() { return name; }
来源：http://ihz.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sii.tianlin.xyz

Ruby: attr_accessor :name
来源：http://pry.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://nla.xuanzx.com

[G12] 对象转字符串
来源：http://hgn.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://put.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ypr.fktsv.cn

JS:   toString() { return this.name; }
来源：http://yuw.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://mth.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://omb.gogol.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xzd.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://xxu.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://bzf.hnqzz.top

[G13] 判断对象类型
来源：http://gbo.zhengqikj.top

Py:   isinstance(u, User)
来源：http://jsl.xylfe.cn

PHP:  $u instanceof User
来源：http://igy.dianchejie.cn

JS:   u instanceof User
来源：http://elf.52xcode.cn

TS:   u instanceof User
来源：http://grc.svipenyu.cn

Java: u instanceof User
来源：http://otk.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://sta.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://hpm.guannengcc.top

C#:   u is User
来源：http://grp.smart0.xyz

[G14] 数据类 / record
来源：http://zug.gaohongyu789.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://and.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://qmo.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://sgp.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://frn.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://let.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://igs.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xkn.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://hqq.chenjidiqi.icu

[G15] 枚举
来源：http://gze.zhijiandao.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://awo.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ysb.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://piv.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ijj.cdnleiting.top

Java: enum Color { RED, GREEN }
来源：http://poh.gogol.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ibh.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://pab.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fjy.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://vsc.yangfankeji.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ilk.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://rwg.hywenlv.cn

JS:   Object.entries(obj)
来源：http://tnp.tanke756.top

TS:   Object.entries(obj)
来源：http://sbv.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mur.fehbvm.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://zrx.tanke756.top

Ruby: obj.instance_variables
来源：http://fpq.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://hbz.havefunace.top

================================================================================
来源：http://znl.cucudq.cn

H. 异常与错误处理
来源：http://mce.316326.xyz

================================================================================
来源：http://fuo.chenzaomai.com

[H01] try / catch 基础
来源：http://wvu.jinqigfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qlp.yonumen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qfs.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fql.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yfw.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwm.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://acs.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ckb.vqdsnc.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ulo.yj20258888.top

[H02] finally / ensure 收尾
来源：http://coa.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zru.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dvy.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gsd.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wkp.gotoacloud.top

Java: try { f(); } finally { cleanup(); }
来源：http://arp.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zid.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://uvv.dianchejie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://abc.guowangkeji.top

[H03] 主动抛出异常
来源：http://gmg.guowangkeji.top

Py:   raise ValueError("错误信息")
来源：http://bmb.shanyushiyangtech.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dqf.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://adw.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://gav.tianlin.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ins.yuxming.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zpm.zhiwuduotai.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lka.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mtf.epnwcf.com

[H04] 自定义异常类型
来源：http://kwc.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://epa.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ndg.cashguo.top

JS:   class MyError extends Error {}
来源：http://dhj.havefunace.top

TS:   class MyError extends Error {}
来源：http://juf.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://gjk.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ckk.gaohongyu789.top

Ruby: class MyError < StandardError; end
来源：http://ejt.tanke756.top

C#:   class MyException : Exception {}
来源：http://hwg.ivvv.top

[H05] 捕获特定类型
来源：http://mdm.dianchejie.cn

Py:   except ValueError as e:
来源：http://jby.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://flu.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://pve.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://mua.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://zwg.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gap.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://jwr.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lnj.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://iqt.meibo888.top

Py:   value = d.get("k") or default
来源：http://ivp.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uhz.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://eyf.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://doq.kuanghao11.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rxs.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uxh.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://qgl.zhiwuduotai.top

C#:   obj?.A?.B ?? default
来源：http://vhl.tian-w.cn

[H07] 断言
来源：http://vox.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://wym.epnwcf.com

PHP:  assert($x > 0);
来源：http://fzs.bbcook.cn

JS:   console.assert(x > 0);
来源：http://ecs.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://pys.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://jjn.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ijg.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://ipb.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://qdc.meibo888.top

[H08] 获取错误信息与堆栈
来源：http://ebx.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://rcq.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lye.chenlongwang.top

JS:   e.message;  e.stack
来源：http://ppe.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ilb.xuanzx.com

Java: e.getMessage();  e.printStackTrace()
来源：http://arn.chenjidiqi.icu

Go:   err.Error()
来源：http://urm.haohaochexian.top


<!-- 参考信息 -->