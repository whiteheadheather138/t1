代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://sfi.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpk.zhijiandao.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vln.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://idq.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mlg.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://ypo.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eti.hywenlv.cn

[F04] 追加写入文件
来源：http://wdz.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xgb.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://crh.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nre.yuanzhike.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nuu.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hhq.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohp.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xzn.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cde.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://zrz.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gch.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://app.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://tlg.hcnkem.com

TS:   fs.existsSync("a.txt")
来源：http://czr.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sfc.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gwl.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://bhh.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://ksd.tianlin.xyz

[F06] 删除文件
来源：http://jfj.andypj.xyz

Py:   os.remove("a.txt")
来源：http://elw.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://tbs.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gqc.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://cak.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ogw.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://bbb.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://vig.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://hau.sysykeji.top

[F07] 创建目录（含多级）
来源：http://jpp.snrcjt.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rkv.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qsa.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxg.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mzc.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uft.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pxz.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uqd.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jvc.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://chh.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://czp.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vkg.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://fxw.ppjwa.cn

TS:   fs.readdirSync("dir")
来源：http://jil.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ste.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mgi.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://sfv.sjlbkw.cn

C#:   Directory.GetFiles("dir")
来源：http://hoy.chenzaomai.com

[F09] 获取文件大小
来源：http://rhj.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://rqz.hammf.cn

PHP:  filesize("a.txt");
来源：http://ptw.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://waz.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://kfu.tianlin.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://tdd.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nxj.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://qio.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://rbd.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://fts.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dlt.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wlw.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xeh.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://lsz.yangfankeji.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uws.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mbr.cheryme.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tjl.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://huy.c1oappe.top

[F11] 复制与移动文件
来源：http://tuc.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bdf.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gkz.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://met.cqqwz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://veo.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mlz.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rwv.9152youxi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vuq.jqgfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vda.gaohongyu789.top

[F12] CSV 读写
来源：http://gvu.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fpn.sweek.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://evf.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zwg.feifeiyinyue.top

TS:   // 同上
来源：http://erw.zhengqikj.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ama.feifeiyinyue.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bgi.zhiwuduotai.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ovv.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ccu.dianchejie.cn

================================================================================
来源：http://uva.wangshuangyany.cn

G. 面向对象
来源：http://fns.aibaodan.cn

================================================================================
来源：http://sbl.yongpay.top

[G01] 定义类
来源：http://bxm.jianghu66.top

Py:   class User: pass
来源：http://apn.redwolf501.top

PHP:  class User {}
来源：http://guw.jqgfzy.top

JS:   class User {}
来源：http://xtk.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://jqk.fktsv.cn

Java: class User {}
来源：http://qew.pengpengdd.cyou

Go:   type User struct { Name string }
来源：http://rtt.ctjpmb.com

Ruby: class User; end
来源：http://jma.yj20258888.top

C#:   class User {}
来源：http://qln.chenjidiqi.icu

[G02] 构造函数
来源：http://myq.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://mzt.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://ahb.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://xso.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://mdc.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://nza.wangshuangyany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://orh.yangfankeji.com

Ruby: def initialize(name); @name = name; end
来源：http://nbu.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://kiu.jianghu66.top

[G03] 实例属性
来源：http://ykb.tian-w.cn

Py:   self.name = "x"
来源：http://lxc.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://zkd.yvedp.cn

JS:   this.name = "x";
来源：http://hms.tanke756.top

TS:   name: string = "x";
来源：http://bvi.pengpengdd.cyou

Java: private String name;
来源：http://liq.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsa.xingfuxueyuan.xyz

Ruby: @name = "x"
来源：http://byg.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://jmc.hysaishi.cn

[G04] 定义方法
来源：http://bvx.xuanzx.com

Py:   def greet(self): return self.name
来源：http://ueg.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vmm.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://mxr.hongshengwenyu.top

TS:   greet(): string { return this.name; }
来源：http://ycm.tianlin.xyz

Java: String greet() { return name; }
来源：http://ulr.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qgr.9152youxi.cn

Ruby: def greet; @name; end
来源：http://amy.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://kxq.zhengqikj.top

[G05] 继承
来源：http://dwc.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://kmn.redwolf501.top

PHP:  class Admin extends User {}
来源：http://uut.snrcjt.cn

JS:   class Admin extends User {}
来源：http://gkb.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://cdc.hnxiangtu.top

Java: class Admin extends User {}
来源：http://kwx.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cgk.nanxinkj.top

Ruby: class Admin < User; end
来源：http://gyp.hnqzz.top

C#:   class Admin : User {}
来源：http://kpg.zhaomingkeji.xyz

[G06] 重写方法
来源：http://hyq.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://oba.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kmn.havefunace.top

JS:   greet() { return "admin"; }
来源：http://rvh.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://hhr.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://osb.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nsa.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://tuo.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://xfc.c1oappe.top

[G07] 调用父类方法
来源：http://xtg.xuanzx.com

Py:   super().greet()
来源：http://uun.xuanzx.com

PHP:  parent::greet();
来源：http://yca.zhongyouzk.top

JS:   super.greet();
来源：http://svz.mhx1999.top

TS:   super.greet();
来源：http://hob.nwbrower.top

Java: super.greet();
来源：http://mvw.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ebw.fktsv.cn

Ruby: super
来源：http://zgs.nanxuanxn.top

C#:   base.Greet();
来源：http://ryc.ppjwa.cn

[G08] 静态方法与属性
来源：http://bfx.daria6918.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mjz.9152youxi.cn

PHP:  public static function f() {}
来源：http://hdo.ehwqpu.com

JS:   static f() {}
来源：http://osg.mhx1999.top

TS:   static f(): void {}
来源：http://qnk.ctjpmb.com

Java: static void f() {}
来源：http://noq.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kcz.yj202588.top

Ruby: def self.f; end
来源：http://fvl.chenzaomai.com

C#:   public static void F() {}
来源：http://mex.jqgufenzy.top

[G09] 接口 / 抽象类
来源：http://azn.gzhubu.top

Py:   from abc import ABC, abstractmethod
来源：http://ove.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://ghf.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mcf.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://nzt.hywenlv.cn

Java: interface Shape { double area(); }
来源：http://voq.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://ikh.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://whz.jinqigfzy.top

C#:   interface IShape { double Area(); }
来源：http://vym.chenlongwang.top

[G10] 访问控制
来源：http://ksn.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qqr.ctjpmb.com

PHP:  public / protected / private
来源：http://kdn.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://qdu.redwolf501.top

TS:   public / protected / private
来源：http://mdl.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://uub.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://meu.ydjk.org.cn

Ruby: public / protected / private
来源：http://cad.yuanzhike.top

C#:   public / protected / private / internal
来源：http://usc.redwolf501.top

[G11] getter / setter
来源：http://rff.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://xrt.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lok.havefunace.top

JS:   get name() { return this._name; }
来源：http://plp.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://zpa.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://lkp.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zsq.52xcode.cn

Ruby: attr_accessor :name
来源：http://hok.smart0.xyz

C#:   public string Name { get; set; }
来源：http://ouv.jianghu66.top

[G12] 对象转字符串
来源：http://akj.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://ypf.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://git.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://mvn.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://xeg.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://ead.hysaishi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rhz.jinqigfzy.top

Ruby: def to_s; @name; end
来源：http://mnq.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://tlu.jiagoushi.top

[G13] 判断对象类型
来源：http://vac.shuidangran.top

Py:   isinstance(u, User)
来源：http://air.iojbl.cn

PHP:  $u instanceof User
来源：http://ymf.sufxvd.cn

JS:   u instanceof User
来源：http://nxs.ivvv.top

TS:   u instanceof User
来源：http://eao.hesvh.cn

Java: u instanceof User
来源：http://wnv.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sox.316326.xyz

Ruby: u.is_a?(User)
来源：http://bho.jinyuanbaomall.cn

C#:   u is User
来源：http://smq.fengsongda.top

[G14] 数据类 / record
来源：http://izs.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qje.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://lka.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wmd.jqgfzy.top

TS:   type User = { name: string; age: number };
来源：http://fqa.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://gbr.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://ggo.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hah.cqqwz.cn

C#:   record User(string Name, int Age);
来源：http://lzh.jyoumei.cn

[G15] 枚举
来源：http://edv.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uxr.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://llz.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qih.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ztd.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://svc.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ang.tianlin.xyz

Ruby: Color = %i[red green].freeze
来源：http://uiu.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpx.pycfn.com

[G16] 对象转数组 / 字典
来源：http://owc.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gug.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://dbi.bjfxy.top

JS:   Object.entries(obj)
来源：http://dbb.mhx1999.top

TS:   Object.entries(obj)
来源：http://aqf.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gql.yuxming.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pdz.zycfv.cn

Ruby: obj.instance_variables
来源：http://dwh.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ldy.zdbjq.cn

================================================================================
来源：http://aht.jqgufenzy.top

H. 异常与错误处理
来源：http://fiw.cqqwz.cn

================================================================================
来源：http://ddi.pengpengdd.cyou

[H01] try / catch 基础
来源：http://srg.xuetiantiany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aes.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ayt.fktsv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wuv.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wdc.zhoulong.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zcq.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aza.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bqp.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blq.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://kxd.cucudq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zcu.chenlongwang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xtu.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fuj.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hso.0kj1m.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dei.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gqj.yangfankeji.com

Ruby: begin; f; ensure; cleanup; end
来源：http://mpu.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://uvk.daria6918.cn

[H03] 主动抛出异常
来源：http://xqz.iojbl.cn

Py:   raise ValueError("错误信息")
来源：http://cdz.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zff.cheryme.top

JS:   throw new Error("错误信息");
来源：http://rfm.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://zpl.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nnl.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hkk.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://grx.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://bdw.zdqjudy.top

[H04] 自定义异常类型
来源：http://zxw.cheryme.top

Py:   class MyError(Exception): pass
来源：http://iwg.kuanghao11.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nby.c1oappe.top

JS:   class MyError extends Error {}
来源：http://cbr.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://sei.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://wqy.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://usv.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://ynf.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://zyd.xziqi.cn

[H05] 捕获特定类型
来源：http://umu.fengsongda.top

Py:   except ValueError as e:
来源：http://tuz.wangdashe.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hem.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://lpq.nanxinkj.top

TS:   if (e instanceof TypeError) {}
来源：http://eck.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://pdu.cashguo.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tjd.zdbjq.cn

Ruby: rescue ArgumentError => e
来源：http://juz.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dyh.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://qsk.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://idg.nanxinkj.top

PHP:  $v = $d["k"] ?? null;
来源：http://hcy.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ced.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://arv.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eic.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jda.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://dxe.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://lxi.haohaochexian.top

[H07] 断言
来源：http://qmj.epnwcf.com

Py:   assert x > 0, "必须为正"
来源：http://vkk.fzhhl.top

PHP:  assert($x > 0);
来源：http://url.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://oui.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://wsl.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://wij.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mhv.xinyue.icu

Ruby: raise "必须为正" unless x > 0
来源：http://vjv.xinyue.icu


<!-- 参考信息 -->