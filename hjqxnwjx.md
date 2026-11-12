代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tfo.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lhd.xuanzx.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dnj.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pbr.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://fcy.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hqr.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://elk.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://oqn.feifeiyinyue.top

TS:   fs.existsSync("a.txt")
来源：http://jfa.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vgt.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zzw.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://ful.cheryme.top

C#:   File.Exists("a.txt")
来源：http://fdu.xziqi.cn

[F06] 删除文件
来源：http://naz.aibaodan.cn

Py:   os.remove("a.txt")
来源：http://kir.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://gwk.vehdjk.com

JS:   fs.unlinkSync("a.txt")
来源：http://vfq.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uof.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ocu.haohaochexian.top

Go:   os.Remove("a.txt")
来源：http://exu.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://dau.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://nii.bbcook.cn

[F07] 创建目录（含多级）
来源：http://obl.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mby.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cpj.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fke.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yag.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dua.feifeiyinyue.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lfe.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uqb.dianchejie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dpw.bjfxy.top

[F08] 遍历目录
来源：http://uji.yj202588.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xfm.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://geh.hongshengwenyu.top

JS:   fs.readdirSync("dir")
来源：http://jfi.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://jat.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dzi.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://hld.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://ruv.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://ctw.mhx1999.top

[F09] 获取文件大小
来源：http://mfi.andypj.xyz

Py:   os.path.getsize("a.txt")
来源：http://htq.316326.xyz

PHP:  filesize("a.txt");
来源：http://tzn.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://gkq.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://jff.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://jcb.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wym.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://zuy.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://mkv.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://xme.haohaochexian.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dyd.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uut.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vtw.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://dpw.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dlv.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rxg.redwolf501.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kvj.hesvh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tmh.gaohongyu789.top

[F11] 复制与移动文件
来源：http://vgy.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uap.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ztv.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rkd.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nse.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yor.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://itq.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://beb.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qxu.epnwcf.com

[F12] CSV 读写
来源：http://ybh.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tyj.nanxuanxn.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://skf.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pjj.yj20258888.top

TS:   // 同上
来源：http://zrn.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cdw.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wcf.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gon.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gyh.xuetiantiany.cn

================================================================================
来源：http://evq.xuanzx.com

G. 面向对象
来源：http://sgf.hysaishi.cn

================================================================================
来源：http://jzp.jqgufenzy.top

[G01] 定义类
来源：http://wkv.sweek.top

Py:   class User: pass
来源：http://jim.tarul.cn

PHP:  class User {}
来源：http://urt.tian-w.cn

JS:   class User {}
来源：http://yxn.smart0.xyz

TS:   class User { name: string = ""; }
来源：http://lpk.ydzc1.top

Java: class User {}
来源：http://kgq.daria6918.cn

Go:   type User struct { Name string }
来源：http://csm.0kj1m.cn

Ruby: class User; end
来源：http://mhw.bjfxy.top

C#:   class User {}
来源：http://tbh.yuxming.cn

[G02] 构造函数
来源：http://fsb.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://bag.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://frx.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://itr.jqgfzy.top

TS:   constructor(public name: string) {}
来源：http://qgq.yangfankeji.com

Java: User(String name) { this.name = name; }
来源：http://fqe.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ivx.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://iod.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://mgs.jlsjyb.cn

[G03] 实例属性
来源：http://orq.jlsjyb.cn

Py:   self.name = "x"
来源：http://dcj.yvedp.cn

PHP:  public string $name = "x";
来源：http://fxj.tian-w.cn

JS:   this.name = "x";
来源：http://mpp.wangdashe.top

TS:   name: string = "x";
来源：http://kts.hesvh.cn

Java: private String name;
来源：http://ilh.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://arb.xylfe.cn

Ruby: @name = "x"
来源：http://qck.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://jwz.zhixingplan.top

[G04] 定义方法
来源：http://yid.fehbvm.com

Py:   def greet(self): return self.name
来源：http://hjb.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://lgo.yueranfly.top

JS:   greet() { return this.name; }
来源：http://jjv.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://hec.hywenlv.cn

Java: String greet() { return name; }
来源：http://njs.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aiu.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://ebo.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://mmt.tian-w.cn

[G05] 继承
来源：http://tsi.vqdsnc.cn

Py:   class Admin(User): pass
来源：http://ycm.sxryk.cn

PHP:  class Admin extends User {}
来源：http://zxw.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://nej.shuidangran.top

TS:   class Admin extends User {}
来源：http://swi.zdbjq.cn

Java: class Admin extends User {}
来源：http://pxs.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bev.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://htx.hnqzz.top

C#:   class Admin : User {}
来源：http://obn.nanxuanxn.top

[G06] 重写方法
来源：http://awe.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://yhy.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://feq.ydzc1.top

JS:   greet() { return "admin"; }
来源：http://cgv.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://zhe.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://esz.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://alq.ivvv.top

Ruby: def greet; "admin"; end
来源：http://dln.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://fyw.xziqi.cn

[G07] 调用父类方法
来源：http://hpj.bjfxy.top

Py:   super().greet()
来源：http://iep.hnqzz.top

PHP:  parent::greet();
来源：http://efh.wangdashe.top

JS:   super.greet();
来源：http://yhp.c1oappe.top

TS:   super.greet();
来源：http://jwv.dashuyun.cn

Java: super.greet();
来源：http://lgr.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hur.c1oappe.top

Ruby: super
来源：http://ovj.ctjpmb.com

C#:   base.Greet();
来源：http://kgb.jlsjyb.cn

[G08] 静态方法与属性
来源：http://svc.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pvu.quarkkingdee.top

PHP:  public static function f() {}
来源：http://isq.9152youxi.cn

JS:   static f() {}
来源：http://ydp.hfpthk.cn

TS:   static f(): void {}
来源：http://qxp.sjlbkw.cn

Java: static void f() {}
来源：http://key.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hgg.vqdsnc.cn

Ruby: def self.f; end
来源：http://ioj.yj20258.top

C#:   public static void F() {}
来源：http://prh.sweek.top

[G09] 接口 / 抽象类
来源：http://brg.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://plx.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://axx.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fcv.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://ktp.meibo888.top

Java: interface Shape { double area(); }
来源：http://amx.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://lys.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bzo.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://ymt.wangdashe.top

[G10] 访问控制
来源：http://eyi.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://tbe.snrcjt.cn

PHP:  public / protected / private
来源：http://oto.sjlbkw.cn

JS:   #private 字段；其余公开
来源：http://syr.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://cjf.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://yrl.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bct.vehdjk.com

Ruby: public / protected / private
来源：http://syx.nanxinkj.top

C#:   public / protected / private / internal
来源：http://eud.ywan-chungtsiang.top

[G11] getter / setter
来源：http://zqa.fengsongda.top

Py:   @property 与 @x.setter
来源：http://qta.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wee.feifeiyinyue.top

JS:   get name() { return this._name; }
来源：http://xns.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://tud.mhx1999.top

Java: public String getName() { return name; }
来源：http://eiw.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tqv.aizwys.cn

Ruby: attr_accessor :name
来源：http://xbe.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://vmb.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://tqz.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://boh.birdmap.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://enf.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://jxi.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://jlf.cdnleiting.top

Java: @Override public String toString() { return name; }
来源：http://itl.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://zkl.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://odd.9152youxi.cn

C#:   public override string ToString() => Name;
来源：http://yfv.zhoulong.xyz

[G13] 判断对象类型
来源：http://ltc.chenzaomai.com

Py:   isinstance(u, User)
来源：http://kzp.ppjwa.cn

PHP:  $u instanceof User
来源：http://txa.shanyushiyangtech.top

JS:   u instanceof User
来源：http://grk.jyoumei.cn

TS:   u instanceof User
来源：http://xue.ehwqpu.com

Java: u instanceof User
来源：http://rjt.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nba.zhongyouzk.top

Ruby: u.is_a?(User)
来源：http://aqr.redwolf501.top

C#:   u is User
来源：http://rdu.jianghu66.top

[G14] 数据类 / record
来源：http://qzp.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yyc.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://uje.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sru.zdbjq.cn

TS:   type User = { name: string; age: number };
来源：http://evu.yfazqb.com

Java: record User(String name, int age) {}
来源：http://obr.nwbrower.top

Go:   type User struct { Name string; Age int }
来源：http://fiz.nwbrower.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://liy.hysaishi.cn

C#:   record User(string Name, int Age);
来源：http://efx.quarkkingdee.top

[G15] 枚举
来源：http://hjg.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qnu.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ive.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dem.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qka.jinqigufen.top

Java: enum Color { RED, GREEN }
来源：http://myq.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lcr.fanxiaobao.xyz

Ruby: Color = %i[red green].freeze
来源：http://hmn.316326.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dnm.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://ipj.zhoulong.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://piu.yanxiufei.cn

PHP:  get_object_vars($obj);
来源：http://qtv.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://rjl.zycfv.cn

TS:   Object.entries(obj)
来源：http://glg.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wva.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://guu.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://ype.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://jsj.dianchejie.cn

================================================================================
来源：http://qvb.jinqigfzy.top

H. 异常与错误处理
来源：http://tli.gogol.net.cn

================================================================================
来源：http://eye.shuidangran.top

[H01] try / catch 基础
来源：http://zke.daxiang520.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yhn.xuanzx.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jum.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uss.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mhu.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fek.vehdjk.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aei.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nbg.wangdashe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://giu.sysykeji.top

[H02] finally / ensure 收尾
来源：http://plr.hfpthk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bxv.chenjidiqi.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://nde.shangyingyoupin.top

JS:   try { f(); } finally { cleanup(); }
来源：http://czu.haohaochexian.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mpd.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://sum.zycfv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zuw.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://njq.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nxz.cqqwz.cn

[H03] 主动抛出异常
来源：http://axe.gaohongyu789.top

Py:   raise ValueError("错误信息")
来源：http://rmx.kuanghao11.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uag.hesvh.cn

JS:   throw new Error("错误信息");
来源：http://bcr.cqqwz.cn

TS:   throw new Error("错误信息");
来源：http://wkh.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://lrw.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uwy.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fwv.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://oie.zhaomingkeji.xyz

[H04] 自定义异常类型
来源：http://apj.cqqwz.cn

Py:   class MyError(Exception): pass
来源：http://cmq.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ivg.fengsongda.top

JS:   class MyError extends Error {}
来源：http://pqn.jinyuanbaomall.cn

TS:   class MyError extends Error {}
来源：http://srq.sufxvd.cn

Java: class MyException extends RuntimeException {}
来源：http://abk.jlsjyb.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://msa.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://poe.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://tik.ydzc1.top

[H05] 捕获特定类型
来源：http://vmk.cqqwz.cn

Py:   except ValueError as e:
来源：http://yxu.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kqe.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://evq.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://iaw.daria6918.cn

Java: catch (IOException | SQLException e) {}
来源：http://hqo.sufxvd.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lih.zhoulong.xyz

Ruby: rescue ArgumentError => e
来源：http://evn.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xen.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://pys.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://vun.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sso.hfpthk.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eau.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://iam.shangyingyoupin.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tmj.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bjk.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://zmy.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://mfz.yanxiufei.cn

[H07] 断言
来源：http://aio.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://yrg.hcnkem.com

PHP:  assert($x > 0);
来源：http://ptk.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://ygu.hfpthk.cn

TS:   console.assert(x > 0);
来源：http://itv.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://agu.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://phj.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://git.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://tug.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://dow.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://bcg.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://brq.pycfn.com

JS:   e.message;  e.stack
来源：http://ssx.svipenyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kil.ctjpmb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://dfz.tianlin.xyz

Go:   err.Error()
来源：http://dsg.0kj1m.cn

Ruby: e.message;  e.backtrace
来源：http://ckm.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://yyn.uphjek.com

[H09] 带错误码的异常
来源：http://onw.52xcode.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cpq.meibo888.top


<!-- 参考信息 -->