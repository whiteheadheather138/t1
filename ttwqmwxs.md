代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wrp.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mmb.zhixingplan.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uox.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pnf.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sdc.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sll.nwbrower.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://typ.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lib.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://rxu.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ldl.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://xcw.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://smw.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://szv.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ldm.yj20258.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lzv.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://zus.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://uhi.shangyingyoupin.top

[F06] 删除文件
来源：http://gma.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://dew.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://xbf.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://jsu.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tye.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ihc.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://caq.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://fdc.ivvv.top

C#:   File.Delete("a.txt");
来源：http://yfj.gotoacloud.top

[F07] 创建目录（含多级）
来源：http://ori.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fei.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jpb.yj20258.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kxx.c1oappe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jca.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://teb.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vkf.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dft.zhaomingkeji.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qup.zhijiandao.cn

[F08] 遍历目录
来源：http://uyn.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wsh.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qva.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://txs.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://fbe.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://amw.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zcg.jqgfzy.top

Ruby: Dir.children("dir")
来源：http://oro.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://wrc.meibo888.top

[F09] 获取文件大小
来源：http://nmi.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://eib.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://hjy.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://ddp.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://bqb.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://bkd.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nql.guannengcc.top

Ruby: File.size("a.txt")
来源：http://rbr.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://pzc.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://oew.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tnz.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lgv.chenlongwang.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pjn.cdnleiting.top

TS:   path.extname("a.txt")
来源：http://vov.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zhx.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zmx.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://avw.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dqy.ydjk.org.cn

[F11] 复制与移动文件
来源：http://jwk.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xan.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://otc.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgc.cheryme.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fhg.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tmu.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xrv.daria6918.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nvh.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kek.wangshuangyany.cn

[F12] CSV 读写
来源：http://kfu.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uay.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xit.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://liq.cdnleiting.top

TS:   // 同上
来源：http://wgj.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://obj.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ccw.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lap.sweek.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nta.guowangkeji.top

================================================================================
来源：http://elx.daxiang520.top

G. 面向对象
来源：http://djj.cheryme.top

================================================================================
来源：http://vpe.quarkkingdee.top

[G01] 定义类
来源：http://tia.ywan-chungtsiang.top

Py:   class User: pass
来源：http://cog.tarul.cn

PHP:  class User {}
来源：http://yho.fanxiaobao.xyz

JS:   class User {}
来源：http://zjd.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://clx.dashuyun.cn

Java: class User {}
来源：http://gew.zhixingplan.top

Go:   type User struct { Name string }
来源：http://mps.hnxiangtu.top

Ruby: class User; end
来源：http://zcu.shangyingyoupin.top

C#:   class User {}
来源：http://kli.xziqi.cn

[G02] 构造函数
来源：http://hck.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://kub.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://xub.redwolf501.top

JS:   constructor(name) { this.name = name; }
来源：http://cnz.xuanzx.com

TS:   constructor(public name: string) {}
来源：http://vai.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://jxi.yj20258888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://itq.smart0.xyz

Ruby: def initialize(name); @name = name; end
来源：http://rth.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://hfl.xuanzx.com

[G03] 实例属性
来源：http://oiv.daxiang520.top

Py:   self.name = "x"
来源：http://qze.yueranfly.top

PHP:  public string $name = "x";
来源：http://edh.tarul.cn

JS:   this.name = "x";
来源：http://kjh.xinyue.icu

TS:   name: string = "x";
来源：http://skw.nanxuanxn.top

Java: private String name;
来源：http://uji.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://goh.shangyingyoupin.top

Ruby: @name = "x"
来源：http://wga.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://bcb.jyoumei.cn

[G04] 定义方法
来源：http://pxf.vehdjk.com

Py:   def greet(self): return self.name
来源：http://lmu.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pzp.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://meu.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://npq.hfpthk.cn

Java: String greet() { return name; }
来源：http://abq.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzw.yfazqb.com

Ruby: def greet; @name; end
来源：http://edj.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://gbj.yueranfly.top

[G05] 继承
来源：http://fix.bbcook.cn

Py:   class Admin(User): pass
来源：http://ljd.shuidangran.top

PHP:  class Admin extends User {}
来源：http://oad.jinghuilouyu.cn

JS:   class Admin extends User {}
来源：http://hbc.ydzc1.top

TS:   class Admin extends User {}
来源：http://arx.vehdjk.com

Java: class Admin extends User {}
来源：http://gbd.feifeiyinyue.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mpp.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://gxb.hcnkem.com

C#:   class Admin : User {}
来源：http://lmq.fanxiaobao.xyz

[G06] 重写方法
来源：http://hmk.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://ozr.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://jux.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://zue.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://zhy.zhiwuduotai.top

Java: @Override String greet() { return "admin"; }
来源：http://glp.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lhe.nanxuanxn.top

Ruby: def greet; "admin"; end
来源：http://qbl.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://xjx.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://met.meibo888.top

Py:   super().greet()
来源：http://lzz.bjfxy.top

PHP:  parent::greet();
来源：http://bkp.jianghu66.top

JS:   super.greet();
来源：http://kuk.yj20258.top

TS:   super.greet();
来源：http://fxp.zhijiandao.cn

Java: super.greet();
来源：http://uon.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ilm.jinqigfzy.top

Ruby: super
来源：http://xji.sweek.top

C#:   base.Greet();
来源：http://aip.yonumen.top

[G08] 静态方法与属性
来源：http://gzc.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oim.jinqigufen.top

PHP:  public static function f() {}
来源：http://jzr.chenzaomai.com

JS:   static f() {}
来源：http://dcn.yangfankeji.com

TS:   static f(): void {}
来源：http://exz.yueranfly.top

Java: static void f() {}
来源：http://vtx.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bkm.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://ncp.pycfn.com

C#:   public static void F() {}
来源：http://mcs.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://ttu.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://suy.yangfankeji.com

PHP:  interface Shape { public function area(): float; }
来源：http://cxd.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gpv.tanke756.top

TS:   interface Shape { area(): number; }
来源：http://kpn.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://szk.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://uue.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://igs.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://mac.jlsjyb.cn

[G10] 访问控制
来源：http://puy.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://srr.ybcxt.top

PHP:  public / protected / private
来源：http://wqh.yongpay.top

JS:   #private 字段；其余公开
来源：http://lry.daria6918.cn

TS:   public / protected / private
来源：http://mzl.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://muo.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kvi.hammf.cn

Ruby: public / protected / private
来源：http://hcs.hcnkem.com

C#:   public / protected / private / internal
来源：http://izl.wangdashe.top

[G11] getter / setter
来源：http://gxn.nwbrower.top

Py:   @property 与 @x.setter
来源：http://hrm.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cza.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://xch.jinyuanbaomall.cn

TS:   get name(): string { return this._name; }
来源：http://jzx.chenzaomai.com

Java: public String getName() { return name; }
来源：http://wae.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kld.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://syy.cheryme.top

C#:   public string Name { get; set; }
来源：http://bwc.fehbvm.com

[G12] 对象转字符串
来源：http://mdk.ybcxt.top

Py:   def __str__(self): return self.name
来源：http://udf.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ako.sufxvd.cn

JS:   toString() { return this.name; }
来源：http://sgd.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://ikg.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://xta.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://onw.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://uxg.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://cgn.sysykeji.top

[G13] 判断对象类型
来源：http://hfq.svipenyu.cn

Py:   isinstance(u, User)
来源：http://gcb.snrcjt.cn

PHP:  $u instanceof User
来源：http://xlf.vqdsnc.cn

JS:   u instanceof User
来源：http://ehi.jqgufenzy.top

TS:   u instanceof User
来源：http://xse.hongshengwenyu.top

Java: u instanceof User
来源：http://rrb.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nai.gzhubu.top

Ruby: u.is_a?(User)
来源：http://daq.jqgufenzy.top

C#:   u is User
来源：http://ghw.tianlin.xyz

[G14] 数据类 / record
来源：http://wpq.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rry.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://pfb.uphjek.com

JS:   // 无内置：普通类或对象字面量
来源：http://emc.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://dof.yj20258888.top

Java: record User(String name, int age) {}
来源：http://ukb.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://yfa.bbcook.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qzz.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://vao.hywenlv.cn

[G15] 枚举
来源：http://tmv.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qru.jianghu66.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zsp.redwolf501.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vms.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://buo.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://vfy.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xsr.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://ksb.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vfu.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://rsn.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xjs.smart0.xyz

PHP:  get_object_vars($obj);
来源：http://fnc.zhijiandao.cn

JS:   Object.entries(obj)
来源：http://shw.andypj.xyz

TS:   Object.entries(obj)
来源：http://uwh.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwp.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ceh.yuanzhike.top

Ruby: obj.instance_variables
来源：http://xom.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://xox.aizwys.cn

================================================================================
来源：http://ule.iojbl.cn

H. 异常与错误处理
来源：http://dhg.xuetiantiany.cn

================================================================================
来源：http://nrm.xuanzx.com

[H01] try / catch 基础
来源：http://ufm.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bvz.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uww.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kvh.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zvq.dianchejie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kme.nwbrower.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wlw.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wnv.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zkj.shangyingyoupin.top

[H02] finally / ensure 收尾
来源：http://hmz.zhixingplan.top

Py:   try: f()⏎finally: cleanup()
来源：http://kde.daria6918.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ndn.jyoumei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pce.ctjpmb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ysf.gzhubu.top

Java: try { f(); } finally { cleanup(); }
来源：http://yat.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gdf.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://bqd.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xhm.jqgufenzy.top

[H03] 主动抛出异常
来源：http://pjs.yuanzhike.top

Py:   raise ValueError("错误信息")
来源：http://ejl.yvedp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jrr.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://kqt.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://sqh.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tcz.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vak.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://txt.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://ipt.iojbl.cn

[H04] 自定义异常类型
来源：http://xzg.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://mtt.fzhhl.top

PHP:  class MyError extends RuntimeException {}
来源：http://vhb.iojbl.cn

JS:   class MyError extends Error {}
来源：http://hnl.meibo888.top

TS:   class MyError extends Error {}
来源：http://hsk.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://fbc.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wxv.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://zya.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://xqx.guowangkeji.top

[H05] 捕获特定类型
来源：http://vji.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://wxu.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qma.316326.xyz

JS:   if (e instanceof TypeError) {}
来源：http://aid.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://xhn.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://aig.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nnj.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://kxu.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ogn.vqdsnc.cn

[H06] 可选值 / 空值安全访问
来源：http://sns.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://spt.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://oes.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://frk.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://oyb.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ipk.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qne.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://jpe.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://ilq.jinqigfzy.top

[H07] 断言
来源：http://pel.sweek.top

Py:   assert x > 0, "必须为正"
来源：http://axo.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://peh.guannengcc.top

JS:   console.assert(x > 0);
来源：http://uxs.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://wws.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://owk.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wwd.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://nsu.aibaodan.cn

C#:   Debug.Assert(x > 0);
来源：http://zis.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://fzf.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://krt.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lot.snrcjt.cn

JS:   e.message;  e.stack
来源：http://pgp.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gcx.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yrn.yongpay.top

Go:   err.Error()
来源：http://kph.yonumen.top


<!-- 参考信息 -->