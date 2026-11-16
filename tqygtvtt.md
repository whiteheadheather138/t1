代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://dry.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lou.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xtp.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zoy.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kui.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://sbz.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://drq.yongpay.top

[F04] 追加写入文件
来源：http://moe.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gmu.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ulp.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uda.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mab.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fbj.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://boo.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://csk.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qnf.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://lvs.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wbv.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://vxl.aizwys.cn

JS:   fs.existsSync("a.txt")
来源：http://ied.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://zwh.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://nuh.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysn.aibaodan.cn

Ruby: File.exist?("a.txt")
来源：http://pqm.yuanzhike.top

C#:   File.Exists("a.txt")
来源：http://vxy.svipenyu.cn

[F06] 删除文件
来源：http://wtl.jinyuanbaomall.cn

Py:   os.remove("a.txt")
来源：http://xvd.uphjek.com

PHP:  unlink("a.txt");
来源：http://dcb.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://ahh.pengpengdd.cyou

TS:   fs.unlinkSync("a.txt")
来源：http://pcl.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nkx.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://xat.tarul.cn

Ruby: File.delete("a.txt")
来源：http://fnk.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://iap.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://waa.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wan.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://poq.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vzn.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpe.hesvh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cij.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gei.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nph.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qjw.yongpay.top

[F08] 遍历目录
来源：http://tmt.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iyg.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kks.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://xjq.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://zku.uphjek.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rdl.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vuc.bjfxy.top

Ruby: Dir.children("dir")
来源：http://vqu.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://ouy.xylfe.cn

[F09] 获取文件大小
来源：http://rfh.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://bke.ivvv.top

PHP:  filesize("a.txt");
来源：http://mgj.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://hxi.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://qwt.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tyf.kuanghao11.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gta.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://ixg.zhixingplan.top

C#:   new FileInfo("a.txt").Length
来源：http://jwy.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://qzs.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ftb.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uat.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nwn.jianghu66.top

TS:   path.extname("a.txt")
来源：http://hxa.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ati.zycfv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ddj.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jbk.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qoj.hfpthk.cn

[F11] 复制与移动文件
来源：http://xnd.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gux.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eld.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ict.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zhj.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://poy.pycfn.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sfc.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ege.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lku.nanxuanxn.top

[F12] CSV 读写
来源：http://uih.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xfe.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uzq.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dhu.316326.xyz

TS:   // 同上
来源：http://kis.c1oappe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phs.jlsjyb.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xor.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xzp.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://quw.fktsv.cn

================================================================================
来源：http://kqg.xylfe.cn

G. 面向对象
来源：http://fkk.jqgufenzy.top

================================================================================
来源：http://izo.dashuyun.cn

[G01] 定义类
来源：http://spw.cashguo.top

Py:   class User: pass
来源：http://rgs.zhengqikj.top

PHP:  class User {}
来源：http://oot.sxryk.cn

JS:   class User {}
来源：http://ecy.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://czb.xziqi.cn

Java: class User {}
来源：http://zvj.kuanghao11.cn

Go:   type User struct { Name string }
来源：http://epk.sxryk.cn

Ruby: class User; end
来源：http://sqw.tianlin.xyz

C#:   class User {}
来源：http://vdc.cheryme.top

[G02] 构造函数
来源：http://akt.zdqjudy.top

Py:   def __init__(self, name): self.name = name
来源：http://eam.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://znt.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://xyb.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://mpc.c1oappe.top

Java: User(String name) { this.name = name; }
来源：http://agv.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mkw.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://sjb.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://idl.shzxlz.cn

[G03] 实例属性
来源：http://xtt.cqqwz.cn

Py:   self.name = "x"
来源：http://uvf.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://nnb.hesvh.cn

JS:   this.name = "x";
来源：http://lzh.zhixingplan.top

TS:   name: string = "x";
来源：http://bof.0kj1m.cn

Java: private String name;
来源：http://ruq.ydjk.org.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tfr.ydjk.org.cn

Ruby: @name = "x"
来源：http://efb.nanxuanxn.top

C#:   public string Name { get; set; } = "x";
来源：http://ulj.52xcode.cn

[G04] 定义方法
来源：http://vzu.zycfv.cn

Py:   def greet(self): return self.name
来源：http://xky.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gzm.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://rqt.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://ojs.nwbrower.top

Java: String greet() { return name; }
来源：http://lrz.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jks.bjfxy.top

Ruby: def greet; @name; end
来源：http://wyy.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://rai.yfazqb.com

[G05] 继承
来源：http://ypj.bjfxy.top

Py:   class Admin(User): pass
来源：http://sca.c1oappe.top

PHP:  class Admin extends User {}
来源：http://fkq.epnwcf.com

JS:   class Admin extends User {}
来源：http://iou.hcnkem.com

TS:   class Admin extends User {}
来源：http://oxm.guowangkeji.top

Java: class Admin extends User {}
来源：http://jid.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xgz.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://yuo.sweek.top

C#:   class Admin : User {}
来源：http://zfo.cqqwz.cn

[G06] 重写方法
来源：http://zic.yj202588.top

Py:   def greet(self): return "admin"
来源：http://cqe.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fgm.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://xwa.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://zqv.xylfe.cn

Java: @Override String greet() { return "admin"; }
来源：http://cde.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xet.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://fgy.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://efk.haohaochexian.top

[G07] 调用父类方法
来源：http://qda.hammf.cn

Py:   super().greet()
来源：http://jcu.aibaodan.cn

PHP:  parent::greet();
来源：http://yhs.jyoumei.cn

JS:   super.greet();
来源：http://toq.hnqzz.top

TS:   super.greet();
来源：http://ccu.ctjpmb.com

Java: super.greet();
来源：http://tzi.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://joy.ivvv.top

Ruby: super
来源：http://gag.zhixingplan.top

C#:   base.Greet();
来源：http://enp.uphjek.com

[G08] 静态方法与属性
来源：http://duf.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tig.zycfv.cn

PHP:  public static function f() {}
来源：http://iyh.zhaomingkeji.xyz

JS:   static f() {}
来源：http://irx.hnqzz.top

TS:   static f(): void {}
来源：http://eke.yj202588.top

Java: static void f() {}
来源：http://ewh.yj20258888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://odo.sxryk.cn

Ruby: def self.f; end
来源：http://vkk.aizwys.cn

C#:   public static void F() {}
来源：http://nin.yvedp.cn

[G09] 接口 / 抽象类
来源：http://upa.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://alw.9152youxi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yri.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yhr.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://isn.xingfuxueyuan.xyz

Java: interface Shape { double area(); }
来源：http://fhl.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://zqg.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rif.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://wvj.svipenyu.cn

[G10] 访问控制
来源：http://xuj.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://qez.shuidangran.top

PHP:  public / protected / private
来源：http://wia.cashguo.top

JS:   #private 字段；其余公开
来源：http://wig.yj20258.top

TS:   public / protected / private
来源：http://iyn.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://lna.shangyingyoupin.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dtq.jianghu66.top

Ruby: public / protected / private
来源：http://nsj.sxryk.cn

C#:   public / protected / private / internal
来源：http://wjw.epnwcf.com

[G11] getter / setter
来源：http://qlo.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://sox.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nqq.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://ktd.jqgufenzy.top

TS:   get name(): string { return this._name; }
来源：http://ood.9152youxi.cn

Java: public String getName() { return name; }
来源：http://mhe.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://abl.andypj.xyz

Ruby: attr_accessor :name
来源：http://ori.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://nry.c1oappe.top

[G12] 对象转字符串
来源：http://pjp.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://pxd.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ayn.jinqigufen.top

JS:   toString() { return this.name; }
来源：http://swr.tianlin.xyz

TS:   toString(): string { return this.name; }
来源：http://sly.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://hse.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://cwr.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://sfd.yfazqb.com

C#:   public override string ToString() => Name;
来源：http://snu.yonumen.top

[G13] 判断对象类型
来源：http://wnb.tarul.cn

Py:   isinstance(u, User)
来源：http://voa.aibaodan.cn

PHP:  $u instanceof User
来源：http://vgi.9152youxi.cn

JS:   u instanceof User
来源：http://dtd.dianchejie.cn

TS:   u instanceof User
来源：http://onw.fzhhl.top

Java: u instanceof User
来源：http://htm.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hrq.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://hid.vehdjk.com

C#:   u is User
来源：http://edi.gzhubu.top

[G14] 数据类 / record
来源：http://osk.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://clu.ctjpmb.com

PHP:  // 用 readonly 属性模拟
来源：http://anu.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://aif.sweek.top

TS:   type User = { name: string; age: number };
来源：http://xfx.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://zlj.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://fap.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ttz.cdnleiting.top

C#:   record User(string Name, int Age);
来源：http://fwv.ywan-chungtsiang.top

[G15] 枚举
来源：http://trd.bbcook.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ztp.shanyushiyangtech.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ahg.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vsj.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://naw.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://kgr.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mey.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://wzv.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lzg.zdbjq.cn

[G16] 对象转数组 / 字典
来源：http://usr.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://och.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://ehr.fehbvm.com

JS:   Object.entries(obj)
来源：http://foa.316326.xyz

TS:   Object.entries(obj)
来源：http://drp.vehdjk.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hxq.hammf.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dfr.meibo888.top

Ruby: obj.instance_variables
来源：http://xxt.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://ijf.hnxiangtu.top

================================================================================
来源：http://gns.uphjek.com

H. 异常与错误处理
来源：http://imb.fanxiaobao.xyz

================================================================================
来源：http://euz.sufxvd.cn

[H01] try / catch 基础
来源：http://gfr.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pzn.zhaomingkeji.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tqh.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jpe.cheryme.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tff.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nqv.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uzk.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xbk.shangyingyoupin.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dmt.xziqi.cn

[H02] finally / ensure 收尾
来源：http://pzn.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oou.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxh.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qdx.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xwe.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://leu.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uhe.redwolf501.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yon.yueranfly.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ypu.vqdsnc.cn

[H03] 主动抛出异常
来源：http://ybj.kuanghao11.cn

Py:   raise ValueError("错误信息")
来源：http://mwx.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zwe.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ieg.nanxuanxn.top

TS:   throw new Error("错误信息");
来源：http://oej.cashguo.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://knx.tian-w.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fcj.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://qbe.hongshengwenyu.top

C#:   throw new ArgumentException("错误信息");
来源：http://ayv.gogol.net.cn

[H04] 自定义异常类型
来源：http://hbv.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://nlq.yueranfly.top

PHP:  class MyError extends RuntimeException {}
来源：http://vnz.yongpay.top

JS:   class MyError extends Error {}
来源：http://lkl.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://aam.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://bnh.jqgufenzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qko.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://taj.hnqzz.top

C#:   class MyException : Exception {}
来源：http://wnb.zdqjudy.top

[H05] 捕获特定类型
来源：http://qwb.ydzc1.top

Py:   except ValueError as e:
来源：http://zws.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mhq.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://poc.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://rdk.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://row.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ozw.cucudq.cn

Ruby: rescue ArgumentError => e
来源：http://vnx.tanke756.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://srs.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://nwa.cashguo.top

Py:   value = d.get("k") or default
来源：http://eui.cheryme.top

PHP:  $v = $d["k"] ?? null;
来源：http://hkf.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gna.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://bbw.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ueo.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mdc.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://rlf.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://qfu.smart0.xyz

[H07] 断言
来源：http://fhe.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://sfm.nanxinkj.top

PHP:  assert($x > 0);
来源：http://zap.jinqigfzy.top

JS:   console.assert(x > 0);
来源：http://isi.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://njc.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://kmr.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://osx.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cgx.cqqwz.cn


<!-- 参考信息 -->