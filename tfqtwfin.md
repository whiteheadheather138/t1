代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iqp.tian-w.cn

Ruby: File.write("a.txt", "hi")
来源：http://wwq.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lqb.smart0.xyz

[F04] 追加写入文件
来源：http://ukg.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mrh.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tbt.hongshengwenyu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qru.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fql.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gem.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qtx.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://opo.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wzr.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://gvm.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wak.zdbjq.cn

PHP:  file_exists("a.txt");
来源：http://mni.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://uin.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://cax.xylfe.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gbt.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://emc.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://nnt.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://wqs.zhongyouzk.top

[F06] 删除文件
来源：http://vsp.cashguo.top

Py:   os.remove("a.txt")
来源：http://daq.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://ufj.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://tgx.zdqjudy.top

TS:   fs.unlinkSync("a.txt")
来源：http://uer.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wcv.uphjek.com

Go:   os.Remove("a.txt")
来源：http://duc.cheryme.top

Ruby: File.delete("a.txt")
来源：http://kzm.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://lkb.hnqzz.top

[F07] 创建目录（含多级）
来源：http://usj.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://faf.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bvp.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sxa.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hje.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tco.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bme.nanxinkj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uvs.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yct.zhongyouzk.top

[F08] 遍历目录
来源：http://rfn.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://seq.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sjz.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://rqc.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://rvq.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ztu.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://psy.pycfn.com

Ruby: Dir.children("dir")
来源：http://mjg.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://tay.sjlbkw.cn

[F09] 获取文件大小
来源：http://yac.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://jtx.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://bpa.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://qjs.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://tgk.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://wqn.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxc.fzhhl.top

Ruby: File.size("a.txt")
来源：http://bvx.hongshengwenyu.top

C#:   new FileInfo("a.txt").Length
来源：http://ueo.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://dpm.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lmf.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qrr.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mkr.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://idf.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qso.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pii.vehdjk.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyr.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vqn.havefunace.top

[F11] 复制与移动文件
来源：http://mdv.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yhn.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://afx.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uup.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvf.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hsp.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nfd.shanyushiyangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hth.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ywz.yfazqb.com

[F12] CSV 读写
来源：http://ygp.hywenlv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xcd.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rir.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jte.ctjpmb.com

TS:   // 同上
来源：http://gwr.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xjc.yj20258.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jzt.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ujm.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://utx.daria6918.cn

================================================================================
来源：http://ccz.sweek.top

G. 面向对象
来源：http://lta.bbcook.cn

================================================================================
来源：http://zke.dashuyun.cn

[G01] 定义类
来源：http://jmq.fehbvm.com

Py:   class User: pass
来源：http://gpy.jianghu66.top

PHP:  class User {}
来源：http://hhq.chenlongwang.top

JS:   class User {}
来源：http://srg.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://eyz.shzxlz.cn

Java: class User {}
来源：http://ibn.pycfn.com

Go:   type User struct { Name string }
来源：http://fpn.pengpengdd.cyou

Ruby: class User; end
来源：http://tic.aibaodan.cn

C#:   class User {}
来源：http://fjn.xylfe.cn

[G02] 构造函数
来源：http://sjv.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://ero.jinyuanbaomall.cn

PHP:  public function __construct(public string $name) {}
来源：http://wpb.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://omn.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://kso.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://vfx.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qjs.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://cxx.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://ntj.andypj.xyz

[G03] 实例属性
来源：http://mqy.shangyingyoupin.top

Py:   self.name = "x"
来源：http://sjr.dashuyun.cn

PHP:  public string $name = "x";
来源：http://qcw.nanxuanxn.top

JS:   this.name = "x";
来源：http://jzy.redwolf501.top

TS:   name: string = "x";
来源：http://bwh.shzxlz.cn

Java: private String name;
来源：http://yam.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdk.sufxvd.cn

Ruby: @name = "x"
来源：http://ihl.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://gbl.zhaomingkeji.xyz

[G04] 定义方法
来源：http://fgk.guannengcc.top

Py:   def greet(self): return self.name
来源：http://vco.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://tyq.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://tkw.zhiwuduotai.top

TS:   greet(): string { return this.name; }
来源：http://lom.tarul.cn

Java: String greet() { return name; }
来源：http://vxn.yj202588.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vea.chenzaomai.com

Ruby: def greet; @name; end
来源：http://xse.uphjek.com

C#:   public string Greet() => Name;
来源：http://xff.jyoumei.cn

[G05] 继承
来源：http://imv.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://svw.pycfn.com

PHP:  class Admin extends User {}
来源：http://jhd.haohaochexian.top

JS:   class Admin extends User {}
来源：http://keh.sysykeji.top

TS:   class Admin extends User {}
来源：http://mkk.shuidangran.top

Java: class Admin extends User {}
来源：http://ybd.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kne.sysykeji.top

Ruby: class Admin < User; end
来源：http://fwz.zhoulong.xyz

C#:   class Admin : User {}
来源：http://xft.zycfv.cn

[G06] 重写方法
来源：http://thv.pycfn.com

Py:   def greet(self): return "admin"
来源：http://ozz.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rjf.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://rgs.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://pya.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://amk.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qki.zdqjudy.top

Ruby: def greet; "admin"; end
来源：http://lfy.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://mut.xuanzx.com

[G07] 调用父类方法
来源：http://dtu.zhaomingkeji.xyz

Py:   super().greet()
来源：http://zbc.hesvh.cn

PHP:  parent::greet();
来源：http://nmj.fzhhl.top

JS:   super.greet();
来源：http://wut.zdqjudy.top

TS:   super.greet();
来源：http://sam.tanke756.top

Java: super.greet();
来源：http://ilg.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dtx.zycfv.cn

Ruby: super
来源：http://eud.zdbjq.cn

C#:   base.Greet();
来源：http://zdm.xylfe.cn

[G08] 静态方法与属性
来源：http://qjq.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ckv.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://ump.jianghu66.top

JS:   static f() {}
来源：http://xeq.dashuyun.cn

TS:   static f(): void {}
来源：http://gsl.fengsongda.top

Java: static void f() {}
来源：http://ynt.wangshuangyany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nvs.yj202588.top

Ruby: def self.f; end
来源：http://vnt.epnwcf.com

C#:   public static void F() {}
来源：http://aem.shzxlz.cn

[G09] 接口 / 抽象类
来源：http://lcn.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://vhq.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://hkc.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wrt.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://csg.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://qku.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://jvs.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fna.aizwys.cn

C#:   interface IShape { double Area(); }
来源：http://jtn.jianghu66.top

[G10] 访问控制
来源：http://hxw.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://cjj.andypj.xyz

PHP:  public / protected / private
来源：http://tix.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://vqc.jqgfzy.top

TS:   public / protected / private
来源：http://ngl.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://zvk.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjo.hywenlv.cn

Ruby: public / protected / private
来源：http://guj.shangyingyoupin.top

C#:   public / protected / private / internal
来源：http://wvz.fzhhl.top

[G11] getter / setter
来源：http://kfi.cqqwz.cn

Py:   @property 与 @x.setter
来源：http://vmx.zdbjq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kgx.cucudq.cn

JS:   get name() { return this._name; }
来源：http://arf.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://ats.hnqzz.top

Java: public String getName() { return name; }
来源：http://cjz.hongshengwenyu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://idy.316326.xyz

Ruby: attr_accessor :name
来源：http://ymd.havefunace.top

C#:   public string Name { get; set; }
来源：http://uma.nanxinkj.top

[G12] 对象转字符串
来源：http://kfz.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://dla.shzxlz.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pah.shangyingyoupin.top

JS:   toString() { return this.name; }
来源：http://msj.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://dok.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://eyo.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://vlf.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://qfs.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://ukn.xingfuxueyuan.xyz

[G13] 判断对象类型
来源：http://ixl.daria6918.cn

Py:   isinstance(u, User)
来源：http://sey.feifeiyinyue.top

PHP:  $u instanceof User
来源：http://dwb.daria6918.cn

JS:   u instanceof User
来源：http://rhr.0kj1m.cn

TS:   u instanceof User
来源：http://ism.iojbl.cn

Java: u instanceof User
来源：http://xlc.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jld.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://qvt.vqdsnc.cn

C#:   u is User
来源：http://vfg.aibaodan.cn

[G14] 数据类 / record
来源：http://uds.zhongyouzk.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://enx.sufxvd.cn

PHP:  // 用 readonly 属性模拟
来源：http://dbr.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uus.jinghuilouyu.cn

TS:   type User = { name: string; age: number };
来源：http://ela.tarul.cn

Java: record User(String name, int age) {}
来源：http://wgn.52xcode.cn

Go:   type User struct { Name string; Age int }
来源：http://atu.cashguo.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://btn.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://ids.jiagoushi.top

[G15] 枚举
来源：http://jkl.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://knq.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dmr.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ujz.yanxiufei.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gqj.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://xpn.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nyl.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://dnm.haohaochexian.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ymj.uphjek.com

[G16] 对象转数组 / 字典
来源：http://cah.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vcv.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://tyc.cqqwz.cn

JS:   Object.entries(obj)
来源：http://qgn.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://own.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wgs.daria6918.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cmu.ydzc1.top

Ruby: obj.instance_variables
来源：http://ndn.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://fih.yuxming.cn

================================================================================
来源：http://btj.hongshengwenyu.top

H. 异常与错误处理
来源：http://glp.shangyingyoupin.top

================================================================================
来源：http://fcd.cqqwz.cn

[H01] try / catch 基础
来源：http://vsb.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yso.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qnu.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kad.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wue.sysykeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://peo.zdqjudy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hbq.gaohongyu789.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wgz.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wgr.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://woq.wangdashe.top

Py:   try: f()⏎finally: cleanup()
来源：http://lcq.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zqq.zhengqikj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qjt.hammf.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oqj.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://tos.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://lgb.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ugk.birdmap.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://kqi.9152youxi.cn

[H03] 主动抛出异常
来源：http://alo.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://yoe.52xcode.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wur.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://ujz.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://meu.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vfu.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://syq.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ikq.guowangkeji.top

C#:   throw new ArgumentException("错误信息");
来源：http://ekn.zdbjq.cn

[H04] 自定义异常类型
来源：http://mhm.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://slk.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://gae.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://spx.xylfe.cn

TS:   class MyError extends Error {}
来源：http://jbs.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://hfv.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sid.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://yey.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://epi.gzhubu.top

[H05] 捕获特定类型
来源：http://tbw.chenzaomai.com

Py:   except ValueError as e:
来源：http://abi.cheryme.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uui.pycfn.com

JS:   if (e instanceof TypeError) {}
来源：http://ryr.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://uzz.gogol.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://his.fehbvm.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bqi.yanxiufei.cn

Ruby: rescue ArgumentError => e
来源：http://dni.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cud.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://ruq.yvedp.cn

Py:   value = d.get("k") or default
来源：http://vik.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://rxs.yvedp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ltj.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://kma.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ocp.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yzy.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://fjo.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://zgd.yanxiufei.cn

[H07] 断言
来源：http://zib.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://cvo.fehbvm.com

PHP:  assert($x > 0);
来源：http://kpw.wangshuangyany.cn

JS:   console.assert(x > 0);
来源：http://epn.hcnkem.com

TS:   console.assert(x > 0);
来源：http://mub.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://klm.xuanzx.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wta.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://xan.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://nil.zdbjq.cn

[H08] 获取错误信息与堆栈
来源：http://qpj.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://kzw.jqgufenzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bkl.zdqjudy.top


<!-- 参考信息 -->