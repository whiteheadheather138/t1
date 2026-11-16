代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://jbs.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://caj.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://jzm.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://sqx.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://cxg.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fuy.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nhi.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://rys.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://mji.yvedp.cn

[F06] 删除文件
来源：http://kzp.mhx1999.top

Py:   os.remove("a.txt")
来源：http://bnz.ydzc1.top

PHP:  unlink("a.txt");
来源：http://tht.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tix.hesvh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lpv.jianghu66.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lrx.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://pzn.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://eri.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://nxn.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://zow.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tox.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cdm.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fgm.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xtl.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dir.zhengqikj.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tfc.kuanghao11.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pmk.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mdn.zhixingplan.top

[F08] 遍历目录
来源：http://yob.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fjd.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jpq.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://lkm.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://giq.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gnn.gaohongyu789.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sbz.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://hbt.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://lgx.ctjpmb.com

[F09] 获取文件大小
来源：http://ddy.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://dvc.ivvv.top

PHP:  filesize("a.txt");
来源：http://qxj.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://zet.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://gjo.andypj.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://mdq.tianlin.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yin.bbcook.cn

Ruby: File.size("a.txt")
来源：http://lgj.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://lda.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://mwy.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nit.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tzn.redwolf501.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yhk.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://sju.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vkf.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bav.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zcc.cqqwz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cwu.sufxvd.cn

[F11] 复制与移动文件
来源：http://wmg.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mxu.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rve.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bco.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zgg.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uyv.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://raz.gogol.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://buo.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://myp.hnqzz.top

[F12] CSV 读写
来源：http://tnj.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zgn.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eit.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://krt.sxryk.cn

TS:   // 同上
来源：http://wnk.zhixingplan.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cno.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vbd.yj202588.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ojs.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://xku.zhengqikj.top

================================================================================
来源：http://ubf.fzhhl.top

G. 面向对象
来源：http://iva.cqqwz.cn

================================================================================
来源：http://pit.birdmap.top

[G01] 定义类
来源：http://nky.xuetiantiany.cn

Py:   class User: pass
来源：http://ktn.316326.xyz

PHP:  class User {}
来源：http://hsy.smart0.xyz

JS:   class User {}
来源：http://vru.hongshengwenyu.top

TS:   class User { name: string = ""; }
来源：http://ysu.zdbjq.cn

Java: class User {}
来源：http://ltq.yj20258.top

Go:   type User struct { Name string }
来源：http://gtt.yuanzhike.top

Ruby: class User; end
来源：http://cvj.shanyushiyangtech.top

C#:   class User {}
来源：http://pmo.shuidangran.top

[G02] 构造函数
来源：http://qjs.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://rzf.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://rxl.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://lcr.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://wzk.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://gdn.kuanghao11.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rlu.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://gpb.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://qpf.yangfankeji.com

[G03] 实例属性
来源：http://hun.sxryk.cn

Py:   self.name = "x"
来源：http://hyv.xziqi.cn

PHP:  public string $name = "x";
来源：http://ylj.hnqzz.top

JS:   this.name = "x";
来源：http://vxc.xuetiantiany.cn

TS:   name: string = "x";
来源：http://fon.hongshengwenyu.top

Java: private String name;
来源：http://bau.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfd.kuanghao11.cn

Ruby: @name = "x"
来源：http://llz.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://abm.shanyushiyangkeji.top

[G04] 定义方法
来源：http://jdh.xziqi.cn

Py:   def greet(self): return self.name
来源：http://mro.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://hcx.daria6918.cn

JS:   greet() { return this.name; }
来源：http://frh.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://cfs.epnwcf.com

Java: String greet() { return name; }
来源：http://cxf.cdnleiting.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ogk.epnwcf.com

Ruby: def greet; @name; end
来源：http://hwc.xylfe.cn

C#:   public string Greet() => Name;
来源：http://rii.vqdsnc.cn

[G05] 继承
来源：http://yiz.hysaishi.cn

Py:   class Admin(User): pass
来源：http://frr.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://kpf.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://htx.yj20258.top

TS:   class Admin extends User {}
来源：http://las.bbcook.cn

Java: class Admin extends User {}
来源：http://utq.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hah.gaohongyu789.top

Ruby: class Admin < User; end
来源：http://xpq.uphjek.com

C#:   class Admin : User {}
来源：http://eig.jlsjyb.cn

[G06] 重写方法
来源：http://tuk.zhixingplan.top

Py:   def greet(self): return "admin"
来源：http://ggq.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qrg.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://qli.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://elf.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://uuj.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://utm.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://uni.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://key.ydzc1.top

[G07] 调用父类方法
来源：http://ong.wangshuangyany.cn

Py:   super().greet()
来源：http://svc.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://kvi.guowangkeji.top

JS:   super.greet();
来源：http://ban.guowangkeji.top

TS:   super.greet();
来源：http://rvp.birdmap.top

Java: super.greet();
来源：http://fhw.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hpp.dashuyun.cn

Ruby: super
来源：http://ujg.havefunace.top

C#:   base.Greet();
来源：http://pis.zhijiandao.cn

[G08] 静态方法与属性
来源：http://wyj.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cpj.zdqjudy.top

PHP:  public static function f() {}
来源：http://nxv.hnxiangtu.top

JS:   static f() {}
来源：http://qcg.yanxiufei.cn

TS:   static f(): void {}
来源：http://mxi.shzxlz.cn

Java: static void f() {}
来源：http://adu.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://bzt.zhixingplan.top

Ruby: def self.f; end
来源：http://mjq.jqgufenzy.top

C#:   public static void F() {}
来源：http://qgd.tian-w.cn

[G09] 接口 / 抽象类
来源：http://ngo.chenzaomai.com

Py:   from abc import ABC, abstractmethod
来源：http://bfw.haohaochexian.top

PHP:  interface Shape { public function area(): float; }
来源：http://oyj.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dks.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://ytf.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://tye.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://cip.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gwi.tanke756.top

C#:   interface IShape { double Area(); }
来源：http://wyi.xylfe.cn

[G10] 访问控制
来源：http://qql.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://cvw.aibaodan.cn

PHP:  public / protected / private
来源：http://yvo.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://tkr.jinghuilouyu.cn

TS:   public / protected / private
来源：http://aad.zdqjudy.top

Java: public / protected / private / 默认包级
来源：http://aex.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://emk.shuidangran.top

Ruby: public / protected / private
来源：http://xfj.fengsongda.top

C#:   public / protected / private / internal
来源：http://fsg.bbcook.cn

[G11] getter / setter
来源：http://jzd.yfazqb.com

Py:   @property 与 @x.setter
来源：http://wwq.xziqi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fmu.guowangkeji.top

JS:   get name() { return this._name; }
来源：http://ynz.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://wbr.wangdashe.top

Java: public String getName() { return name; }
来源：http://crh.xylfe.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yut.andypj.xyz

Ruby: attr_accessor :name
来源：http://qaj.zycfv.cn

C#:   public string Name { get; set; }
来源：http://irq.dianchejie.cn

[G12] 对象转字符串
来源：http://gjc.snrcjt.cn

Py:   def __str__(self): return self.name
来源：http://quq.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dpt.jqgfzy.top

JS:   toString() { return this.name; }
来源：http://epx.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://aqr.yangfankeji.com

Java: @Override public String toString() { return name; }
来源：http://cqs.daria6918.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tkr.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://hsy.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://ahx.ehwqpu.com

[G13] 判断对象类型
来源：http://deo.cheryme.top

Py:   isinstance(u, User)
来源：http://ovq.jqgufenzy.top

PHP:  $u instanceof User
来源：http://bcs.chenjidiqi.icu

JS:   u instanceof User
来源：http://mmq.smart0.xyz

TS:   u instanceof User
来源：http://gzg.pengpengdd.cyou

Java: u instanceof User
来源：http://zzu.fktsv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tft.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://wdh.jinyuanbaomall.cn

C#:   u is User
来源：http://qsn.fengsongda.top

[G14] 数据类 / record
来源：http://wfj.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bdt.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://ynr.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://jhn.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://eww.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://kkc.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://dpv.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zjj.hammf.cn

C#:   record User(string Name, int Age);
来源：http://whk.hongshengwenyu.top

[G15] 枚举
来源：http://hnx.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hoz.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://zyd.cashguo.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vfl.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bjm.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://suf.meibo888.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bdy.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://odf.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://apz.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://tgy.meibo888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://smf.meibo888.top

PHP:  get_object_vars($obj);
来源：http://rjb.hfpthk.cn

JS:   Object.entries(obj)
来源：http://uvc.xziqi.cn

TS:   Object.entries(obj)
来源：http://hmc.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wyh.jinqigfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lnc.yueranfly.top

Ruby: obj.instance_variables
来源：http://hqw.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://xlu.jinghuilouyu.cn

================================================================================
来源：http://fhc.daria6918.cn

H. 异常与错误处理
来源：http://yod.zdqjudy.top

================================================================================
来源：http://azl.yj20258888.top

[H01] try / catch 基础
来源：http://bum.cucudq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jzx.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tqu.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uda.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fqp.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hqo.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lxk.jinqigfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vgs.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bkx.gogol.net.cn

[H02] finally / ensure 收尾
来源：http://vjd.jiagoushi.top

Py:   try: f()⏎finally: cleanup()
来源：http://rim.zhiwuduotai.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kpp.quarkkingdee.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wry.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://tut.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://fpd.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://dme.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gvc.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://rbx.xziqi.cn

[H03] 主动抛出异常
来源：http://njy.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://vie.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fyi.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://dks.ydzc1.top

TS:   throw new Error("错误信息");
来源：http://qov.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xdw.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ijn.sjlbkw.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://itx.tarul.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oaz.9152youxi.cn

[H04] 自定义异常类型
来源：http://pxn.bbcook.cn

Py:   class MyError(Exception): pass
来源：http://lzh.xylfe.cn

PHP:  class MyError extends RuntimeException {}
来源：http://okh.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://wta.xuanzx.com

TS:   class MyError extends Error {}
来源：http://kmr.fanxiaobao.xyz

Java: class MyException extends RuntimeException {}
来源：http://rrb.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rzg.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://acc.52xcode.cn

C#:   class MyException : Exception {}
来源：http://xrv.yfazqb.com

[H05] 捕获特定类型
来源：http://lpc.xuanzx.com

Py:   except ValueError as e:
来源：http://sgl.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tdh.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://lft.ydzc1.top

TS:   if (e instanceof TypeError) {}
来源：http://fev.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://uwy.hywenlv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jcr.snrcjt.cn

Ruby: rescue ArgumentError => e
来源：http://xzt.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kib.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://hrl.chenlongwang.top

Py:   value = d.get("k") or default
来源：http://him.hfpthk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vzm.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gwp.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ezf.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kfe.nanxinkj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jgs.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://vzp.pycfn.com

C#:   obj?.A?.B ?? default
来源：http://pum.ybcxt.top

[H07] 断言
来源：http://ops.jinghuilouyu.cn

Py:   assert x > 0, "必须为正"
来源：http://wmm.shanyushiyangkeji.top

PHP:  assert($x > 0);
来源：http://nqc.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://whd.cheryme.top

TS:   console.assert(x > 0);
来源：http://vfy.yuxming.cn

Java: assert x > 0 : "必须为正";
来源：http://ecp.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bmr.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xzc.hesvh.cn

C#:   Debug.Assert(x > 0);
来源：http://bal.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://cfz.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://qqj.shanyushiyangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wmj.daxiang520.top

JS:   e.message;  e.stack
来源：http://sgb.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ced.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://hbi.aizwys.cn

Go:   err.Error()
来源：http://rlt.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://uak.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://zei.chenlongwang.top

[H09] 带错误码的异常
来源：http://nxw.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hze.hesvh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://guz.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tnm.ctjpmb.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fyx.fanxiaobao.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lzk.kuanghao11.cn


<!-- 参考信息 -->