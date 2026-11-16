代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mcm.ivvv.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://awx.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://sxc.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://pvr.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://xsm.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gpv.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bnz.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://hqg.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://yyj.yanxiufei.cn

[F06] 删除文件
来源：http://wmi.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://gsg.chenlongwang.top

PHP:  unlink("a.txt");
来源：http://iep.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wiw.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://vty.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mkl.epnwcf.com

Go:   os.Remove("a.txt")
来源：http://toz.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://csz.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://yea.52xcode.cn

[F07] 创建目录（含多级）
来源：http://ouo.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sua.316326.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vgv.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqe.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ent.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ymr.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wdq.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uce.0kj1m.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tlo.xylfe.cn

[F08] 遍历目录
来源：http://vpo.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ptf.ybcxt.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ejf.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://amu.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://bhz.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zzb.ivvv.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iqg.cheryme.top

Ruby: Dir.children("dir")
来源：http://jay.yfazqb.com

C#:   Directory.GetFiles("dir")
来源：http://yui.gaohongyu789.top

[F09] 获取文件大小
来源：http://aqh.chenzaomai.com

Py:   os.path.getsize("a.txt")
来源：http://kvj.xylfe.cn

PHP:  filesize("a.txt");
来源：http://ouq.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://vml.xylfe.cn

TS:   fs.statSync("a.txt").size
来源：http://ldi.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mpt.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qtp.yongpay.top

Ruby: File.size("a.txt")
来源：http://obp.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://fiv.fehbvm.com

[F10] 取文件扩展名 / 文件名
来源：http://jjd.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://apc.tianlin.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rid.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pnx.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://qgj.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pcc.tanke756.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wxh.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vbj.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://txi.fehbvm.com

[F11] 复制与移动文件
来源：http://auu.tarul.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ijf.chenzaomai.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ims.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ctr.zhongyouzk.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufv.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://urt.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gwi.jqgufenzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oke.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pvn.wangdashe.top

[F12] CSV 读写
来源：http://fgl.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kpy.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bak.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zkq.gaohongyu789.top

TS:   // 同上
来源：http://sdx.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lyv.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://utm.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xml.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mmz.yj20258.top

================================================================================
来源：http://axk.wangshuangyany.cn

G. 面向对象
来源：http://beg.vqdsnc.cn

================================================================================
来源：http://dxt.zhoulong.xyz

[G01] 定义类
来源：http://fhf.vehdjk.com

Py:   class User: pass
来源：http://nje.mhx1999.top

PHP:  class User {}
来源：http://qpd.fehbvm.com

JS:   class User {}
来源：http://lun.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://wka.sufxvd.cn

Java: class User {}
来源：http://oty.chenlongwang.top

Go:   type User struct { Name string }
来源：http://gtk.daria6918.cn

Ruby: class User; end
来源：http://kwi.daria6918.cn

C#:   class User {}
来源：http://czm.sysykeji.top

[G02] 构造函数
来源：http://ylo.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://tqz.wangshuangyany.cn

PHP:  public function __construct(public string $name) {}
来源：http://uhm.ydjk.org.cn

JS:   constructor(name) { this.name = name; }
来源：http://snd.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://tbe.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://owz.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://orl.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://agt.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://sus.ywan-chungtsiang.top

[G03] 实例属性
来源：http://ezj.yangfankeji.com

Py:   self.name = "x"
来源：http://bqw.xylfe.cn

PHP:  public string $name = "x";
来源：http://iah.hnxiangtu.top

JS:   this.name = "x";
来源：http://nov.jlsjyb.cn

TS:   name: string = "x";
来源：http://qqj.havefunace.top

Java: private String name;
来源：http://mth.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pdd.cdnleiting.top

Ruby: @name = "x"
来源：http://nit.wangshuangyany.cn

C#:   public string Name { get; set; } = "x";
来源：http://evc.yj20258888.top

[G04] 定义方法
来源：http://euk.jinqigfzy.top

Py:   def greet(self): return self.name
来源：http://ebl.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://atc.zycfv.cn

JS:   greet() { return this.name; }
来源：http://mjl.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://umx.sxryk.cn

Java: String greet() { return name; }
来源：http://dyz.sxryk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vyf.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://tog.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://nsx.fanxiaobao.xyz

[G05] 继承
来源：http://gti.ehwqpu.com

Py:   class Admin(User): pass
来源：http://hev.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://slx.sxryk.cn

JS:   class Admin extends User {}
来源：http://yjm.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://siq.jiagoushi.top

Java: class Admin extends User {}
来源：http://lus.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wih.yanxiufei.cn

Ruby: class Admin < User; end
来源：http://vhn.yangfankeji.com

C#:   class Admin : User {}
来源：http://kqc.tianlin.xyz

[G06] 重写方法
来源：http://dxg.9152youxi.cn

Py:   def greet(self): return "admin"
来源：http://uag.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bvd.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://pfv.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://alc.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://llm.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bmy.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://byh.meibo888.top

C#:   public override string Greet() => "admin";
来源：http://hrf.wangshuangyany.cn

[G07] 调用父类方法
来源：http://blu.snrcjt.cn

Py:   super().greet()
来源：http://kgi.xinyue.icu

PHP:  parent::greet();
来源：http://wfi.vehdjk.com

JS:   super.greet();
来源：http://ruh.dianchejie.cn

TS:   super.greet();
来源：http://qap.redwolf501.top

Java: super.greet();
来源：http://vyw.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gaz.hysaishi.cn

Ruby: super
来源：http://wga.zhijiandao.cn

C#:   base.Greet();
来源：http://gpl.zdqjudy.top

[G08] 静态方法与属性
来源：http://cob.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zui.sxryk.cn

PHP:  public static function f() {}
来源：http://iey.yueranfly.top

JS:   static f() {}
来源：http://yiw.0kj1m.cn

TS:   static f(): void {}
来源：http://jjv.birdmap.top

Java: static void f() {}
来源：http://lly.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sul.sjlbkw.cn

Ruby: def self.f; end
来源：http://izy.jyoumei.cn

C#:   public static void F() {}
来源：http://rcb.ivvv.top

[G09] 接口 / 抽象类
来源：http://afm.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://moh.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://mnk.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xfa.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://hqb.ppjwa.cn

Java: interface Shape { double area(); }
来源：http://yjf.gzhubu.top

Go:   type Shape interface { Area() float64 }
来源：http://qtt.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cbq.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://cvk.wangshuangyany.cn

[G10] 访问控制
来源：http://igw.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://opj.0kj1m.cn

PHP:  public / protected / private
来源：http://voj.tanke756.top

JS:   #private 字段；其余公开
来源：http://snh.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://mom.smart0.xyz

Java: public / protected / private / 默认包级
来源：http://ata.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pyy.yuxming.cn

Ruby: public / protected / private
来源：http://ozs.zdqjudy.top

C#:   public / protected / private / internal
来源：http://ulw.yanxiufei.cn

[G11] getter / setter
来源：http://aqe.xylfe.cn

Py:   @property 与 @x.setter
来源：http://ner.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zgt.cucudq.cn

JS:   get name() { return this._name; }
来源：http://nsb.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://ghy.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://wbu.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bck.daria6918.cn

Ruby: attr_accessor :name
来源：http://ase.yueranfly.top

C#:   public string Name { get; set; }
来源：http://rtn.ydjk.org.cn

[G12] 对象转字符串
来源：http://mwn.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://kkl.ivvv.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mvj.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://jrd.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://euz.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://btm.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://inz.ybcxt.top

Ruby: def to_s; @name; end
来源：http://gje.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://aed.shzxlz.cn

[G13] 判断对象类型
来源：http://ocq.jinqigufen.top

Py:   isinstance(u, User)
来源：http://mzs.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://qny.aibaodan.cn

JS:   u instanceof User
来源：http://vok.fehbvm.com

TS:   u instanceof User
来源：http://xaz.sufxvd.cn

Java: u instanceof User
来源：http://ozl.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rbq.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://zuk.sxryk.cn

C#:   u is User
来源：http://jmt.sweek.top

[G14] 数据类 / record
来源：http://nqk.aibaodan.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yux.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://lvv.jinqigfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://prz.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://jeb.yueranfly.top

Java: record User(String name, int age) {}
来源：http://rsr.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://iia.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mxl.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://cop.zhongyouzk.top

[G15] 枚举
来源：http://siw.pycfn.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tkr.ydzc1.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jnc.hesvh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qon.uphjek.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wzk.guowangkeji.top

Java: enum Color { RED, GREEN }
来源：http://whb.havefunace.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rch.birdmap.top

Ruby: Color = %i[red green].freeze
来源：http://jke.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wrk.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://gcw.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vpz.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://wvv.redwolf501.top

JS:   Object.entries(obj)
来源：http://ypy.jinqigufen.top

TS:   Object.entries(obj)
来源：http://iep.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qii.hesvh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fae.yongpay.top

Ruby: obj.instance_variables
来源：http://ryf.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://adm.sufxvd.cn

================================================================================
来源：http://knx.xuanzx.com

H. 异常与错误处理
来源：http://dpu.cqqwz.cn

================================================================================
来源：http://eet.zdqjudy.top

[H01] try / catch 基础
来源：http://obp.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vvj.vqdsnc.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fyn.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://let.hcnkem.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tud.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://irx.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dqw.ppjwa.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rjv.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vgs.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://xao.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://hrq.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xuy.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qtr.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://psj.dianchejie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cen.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cei.wangdashe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ajw.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lmo.bbcook.cn

[H03] 主动抛出异常
来源：http://cso.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://mxs.zdqjudy.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ebs.hywenlv.cn

JS:   throw new Error("错误信息");
来源：http://kwj.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://wqk.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://dfs.guowangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kvf.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sek.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://ord.yuxming.cn

[H04] 自定义异常类型
来源：http://hqs.feifeiyinyue.top

Py:   class MyError(Exception): pass
来源：http://pjw.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://cti.guannengcc.top

JS:   class MyError extends Error {}
来源：http://rxe.fengsongda.top

TS:   class MyError extends Error {}
来源：http://pwe.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://mao.haohaochexian.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kzw.wangshuangyany.cn

Ruby: class MyError < StandardError; end
来源：http://veq.nwbrower.top

C#:   class MyException : Exception {}
来源：http://fvd.xylfe.cn

[H05] 捕获特定类型
来源：http://ouu.gotoacloud.top

Py:   except ValueError as e:
来源：http://bva.haohaochexian.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iha.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://hsh.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://dbh.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://gwz.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yxh.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://bzf.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ogn.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://jxm.jianghu66.top

Py:   value = d.get("k") or default
来源：http://acm.jiagoushi.top

PHP:  $v = $d["k"] ?? null;
来源：http://xmf.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pjx.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://tfh.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yft.vehdjk.com

Go:   if v, ok := m["k"]; ok { }
来源：http://hkp.jianghu66.top

Ruby: d&.dig(:a, :b)
来源：http://lke.hongshengwenyu.top

C#:   obj?.A?.B ?? default
来源：http://wjk.jqgfzy.top

[H07] 断言
来源：http://eag.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://tmh.shuidangran.top

PHP:  assert($x > 0);
来源：http://djf.yj20258.top

JS:   console.assert(x > 0);
来源：http://tfx.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://vgc.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://biv.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oek.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://wek.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://dkx.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://mqf.hywenlv.cn

Py:   str(e);  traceback.format_exc()
来源：http://dxo.sjlbkw.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kif.ybcxt.top

JS:   e.message;  e.stack
来源：http://twp.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ujb.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uwd.cashguo.top

Go:   err.Error()
来源：http://pyo.zdbjq.cn

Ruby: e.message;  e.backtrace
来源：http://pxe.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://wfn.kuanghao11.cn

[H09] 带错误码的异常
来源：http://kgd.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eio.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wvl.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jcv.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tqf.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://adj.gogol.net.cn


<!-- 参考信息 -->