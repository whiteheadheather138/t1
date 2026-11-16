代发 wailian999

C#:   File.Exists("a.txt")
来源：http://uee.cdnleiting.top

[F06] 删除文件
来源：http://pfj.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://bcd.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://fqm.gaohongyu789.top

JS:   fs.unlinkSync("a.txt")
来源：http://qfp.jinghuilouyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jmy.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eyo.zdbjq.cn

Go:   os.Remove("a.txt")
来源：http://ntc.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://yah.tarul.cn

C#:   File.Delete("a.txt");
来源：http://rnc.andypj.xyz

[F07] 创建目录（含多级）
来源：http://ksb.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dtc.shzxlz.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://czq.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://msw.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hbt.cashguo.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zxv.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lft.cdnleiting.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://efv.jqgufenzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kfa.shangyingyoupin.top

[F08] 遍历目录
来源：http://nud.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lgl.jinyuanbaomall.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nhr.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://pgj.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://xhd.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zge.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pla.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://kfg.zdqjudy.top

C#:   Directory.GetFiles("dir")
来源：http://joq.sxryk.cn

[F09] 获取文件大小
来源：http://fys.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://mvh.c1oappe.top

PHP:  filesize("a.txt");
来源：http://nsr.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://kpj.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://kwd.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://myk.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://boc.sysykeji.top

Ruby: File.size("a.txt")
来源：http://ivd.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://eir.mhx1999.top

[F10] 取文件扩展名 / 文件名
来源：http://ogo.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iqc.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dyj.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://phe.ppjwa.cn

TS:   path.extname("a.txt")
来源：http://gte.yvedp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mjk.hnqzz.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ayv.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rjc.meibo888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bdw.yongpay.top

[F11] 复制与移动文件
来源：http://wda.yongpay.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ofq.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pwm.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ewe.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmv.jinyuanbaomall.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gde.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wse.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wwv.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kmc.zhoulong.xyz

[F12] CSV 读写
来源：http://ysh.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mwu.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xuf.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mbm.snrcjt.cn

TS:   // 同上
来源：http://hld.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xod.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dlp.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gtt.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hsp.zhaomingkeji.xyz

================================================================================
来源：http://swb.dianchejie.cn

G. 面向对象
来源：http://qzy.xingfuxueyuan.xyz

================================================================================
来源：http://otw.sjlbkw.cn

[G01] 定义类
来源：http://ogm.yuanzhike.top

Py:   class User: pass
来源：http://vmo.iojbl.cn

PHP:  class User {}
来源：http://dry.pengpengdd.cyou

JS:   class User {}
来源：http://vdg.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://cnc.nwbrower.top

Java: class User {}
来源：http://ryd.svipenyu.cn

Go:   type User struct { Name string }
来源：http://cgh.epnwcf.com

Ruby: class User; end
来源：http://oxm.yueranfly.top

C#:   class User {}
来源：http://ebe.hongshengwenyu.top

[G02] 构造函数
来源：http://gvo.shuidangran.top

Py:   def __init__(self, name): self.name = name
来源：http://yan.zdbjq.cn

PHP:  public function __construct(public string $name) {}
来源：http://vxg.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://xvk.pycfn.com

TS:   constructor(public name: string) {}
来源：http://ted.sjlbkw.cn

Java: User(String name) { this.name = name; }
来源：http://aoo.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cci.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://cog.gotoacloud.top

C#:   public User(string name) { Name = name; }
来源：http://hlp.yangfankeji.com

[G03] 实例属性
来源：http://qxb.yj20258888.top

Py:   self.name = "x"
来源：http://kyr.fktsv.cn

PHP:  public string $name = "x";
来源：http://kac.gotoacloud.top

JS:   this.name = "x";
来源：http://was.yj20258.top

TS:   name: string = "x";
来源：http://zyt.jinqigfzy.top

Java: private String name;
来源：http://jor.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fhw.feifeiyinyue.top

Ruby: @name = "x"
来源：http://wku.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://jzg.jiagoushi.top

[G04] 定义方法
来源：http://ibe.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://tkz.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://gfn.jianghu66.top

JS:   greet() { return this.name; }
来源：http://cfa.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://njy.gzhubu.top

Java: String greet() { return name; }
来源：http://ecw.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dbx.epnwcf.com

Ruby: def greet; @name; end
来源：http://nmo.jianghu66.top

C#:   public string Greet() => Name;
来源：http://hde.shanyushiyangkeji.top

[G05] 继承
来源：http://gri.c1oappe.top

Py:   class Admin(User): pass
来源：http://zok.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://duv.haohaochexian.top

JS:   class Admin extends User {}
来源：http://gbb.shuidangran.top

TS:   class Admin extends User {}
来源：http://clg.shuidangran.top

Java: class Admin extends User {}
来源：http://ynh.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kgt.hywenlv.cn

Ruby: class Admin < User; end
来源：http://mvi.zdqjudy.top

C#:   class Admin : User {}
来源：http://vmb.tian-w.cn

[G06] 重写方法
来源：http://ggu.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://qxn.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nah.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://ehb.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://kfe.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://mhp.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ksa.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://dwc.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://gvw.pycfn.com

[G07] 调用父类方法
来源：http://ijl.havefunace.top

Py:   super().greet()
来源：http://lef.epnwcf.com

PHP:  parent::greet();
来源：http://lcs.tarul.cn

JS:   super.greet();
来源：http://hah.svipenyu.cn

TS:   super.greet();
来源：http://plw.hnxiangtu.top

Java: super.greet();
来源：http://bia.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lok.nanxinkj.top

Ruby: super
来源：http://ose.feifeiyinyue.top

C#:   base.Greet();
来源：http://jyr.fehbvm.com

[G08] 静态方法与属性
来源：http://qin.ctjpmb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mje.sjlbkw.cn

PHP:  public static function f() {}
来源：http://mhe.kuanghao11.cn

JS:   static f() {}
来源：http://jdi.jianghu66.top

TS:   static f(): void {}
来源：http://mus.wangshuangyany.cn

Java: static void f() {}
来源：http://qnc.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ebn.nanxinkj.top

Ruby: def self.f; end
来源：http://ljg.fktsv.cn

C#:   public static void F() {}
来源：http://ztz.cucudq.cn

[G09] 接口 / 抽象类
来源：http://vtz.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://eha.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://iaq.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fms.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://pff.hfpthk.cn

Java: interface Shape { double area(); }
来源：http://wcx.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://nje.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tqr.hnxiangtu.top

C#:   interface IShape { double Area(); }
来源：http://trv.xylfe.cn

[G10] 访问控制
来源：http://edu.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://gwr.hysaishi.cn

PHP:  public / protected / private
来源：http://qmf.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://cmo.andypj.xyz

TS:   public / protected / private
来源：http://tcc.jyoumei.cn

Java: public / protected / private / 默认包级
来源：http://lhj.ehwqpu.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://xbn.zhongyouzk.top

Ruby: public / protected / private
来源：http://aah.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://bey.ydjk.org.cn

[G11] getter / setter
来源：http://lzd.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://kyu.jinghuilouyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xpe.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://wlv.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://myh.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://lzg.haohaochexian.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vlu.zhoulong.xyz

Ruby: attr_accessor :name
来源：http://wut.hywenlv.cn

C#:   public string Name { get; set; }
来源：http://pkb.feifeiyinyue.top

[G12] 对象转字符串
来源：http://ebc.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://psp.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hmy.havefunace.top

JS:   toString() { return this.name; }
来源：http://rno.guowangkeji.top

TS:   toString(): string { return this.name; }
来源：http://oxj.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://toe.sjlbkw.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rri.xziqi.cn

Ruby: def to_s; @name; end
来源：http://zqb.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://axm.yueranfly.top

[G13] 判断对象类型
来源：http://dws.daxiang520.top

Py:   isinstance(u, User)
来源：http://yks.cqqwz.cn

PHP:  $u instanceof User
来源：http://gus.shuidangran.top

JS:   u instanceof User
来源：http://ajc.feifeiyinyue.top

TS:   u instanceof User
来源：http://fzx.yfazqb.com

Java: u instanceof User
来源：http://jvy.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ygw.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://luq.pycfn.com

C#:   u is User
来源：http://ncs.chenjidiqi.icu

[G14] 数据类 / record
来源：http://qnn.dianchejie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wtu.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://gvc.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://ubx.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://ofn.uphjek.com

Java: record User(String name, int age) {}
来源：http://eje.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://bwt.yongpay.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dqw.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://pwb.jinghuilouyu.cn

[G15] 枚举
来源：http://oah.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cye.dianchejie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ova.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xte.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tfz.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://mqj.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sti.yanxiufei.cn

Ruby: Color = %i[red green].freeze
来源：http://icd.gaohongyu789.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://efc.havefunace.top

[G16] 对象转数组 / 字典
来源：http://fin.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://soj.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://gra.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://nxn.jlsjyb.cn

TS:   Object.entries(obj)
来源：http://zcu.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jlt.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://kpr.snrcjt.cn

Ruby: obj.instance_variables
来源：http://rnv.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://ouw.nanxinkj.top

================================================================================
来源：http://wbw.hnqzz.top

H. 异常与错误处理
来源：http://yiw.ydzc1.top

================================================================================
来源：http://yjz.jinqigufen.top

[H01] try / catch 基础
来源：http://zss.andypj.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://spg.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zax.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jyt.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baa.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dif.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kmc.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jml.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vlp.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://gdu.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://puz.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jzs.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qwz.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rjm.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://unh.zhijiandao.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wqw.jianghu66.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ygn.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vfo.cqqwz.cn

[H03] 主动抛出异常
来源：http://rpd.sxryk.cn

Py:   raise ValueError("错误信息")
来源：http://ezh.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mqw.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://bvs.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://xfj.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wkq.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://msa.hfpthk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zcl.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://weh.zhengqikj.top

[H04] 自定义异常类型
来源：http://vdv.meibo888.top

Py:   class MyError(Exception): pass
来源：http://yog.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://btk.hysaishi.cn

JS:   class MyError extends Error {}
来源：http://jgt.tian-w.cn

TS:   class MyError extends Error {}
来源：http://zjg.zhengqikj.top

Java: class MyException extends RuntimeException {}
来源：http://fwz.cashguo.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bre.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://qoc.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://ykq.fktsv.cn

[H05] 捕获特定类型
来源：http://ymw.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://cdp.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://des.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://ecx.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://fko.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://ygk.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pzx.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://vpi.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ngf.cucudq.cn

[H06] 可选值 / 空值安全访问
来源：http://cyp.meibo888.top

Py:   value = d.get("k") or default
来源：http://brf.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://cyj.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://nib.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zjr.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sap.sjlbkw.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qag.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://vua.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://chz.xuetiantiany.cn

[H07] 断言
来源：http://xuk.haohaochexian.top

Py:   assert x > 0, "必须为正"
来源：http://vwv.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://atx.chenlongwang.top

JS:   console.assert(x > 0);
来源：http://pyp.gaohongyu789.top

TS:   console.assert(x > 0);
来源：http://kar.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://cre.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gfe.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://zfw.xingfuxueyuan.xyz

C#:   Debug.Assert(x > 0);
来源：http://aiq.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://gjk.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://tbb.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ffk.snrcjt.cn

JS:   e.message;  e.stack
来源：http://eac.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ftk.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wmm.svipenyu.cn

Go:   err.Error()
来源：http://ekh.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://vpl.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://nzt.chenzaomai.com

[H09] 带错误码的异常
来源：http://jlw.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://umq.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://vkq.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lzj.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://onu.zycfv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hal.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cxn.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://odw.bbcook.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://drj.smart0.xyz

[H10] 资源自动释放
来源：http://tah.c1oappe.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ybe.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sit.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xpi.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kwk.hnqzz.top


<!-- 参考信息 -->