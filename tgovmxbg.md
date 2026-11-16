代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://nxm.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cit.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://wjz.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://ujn.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://oip.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rpd.fanxiaobao.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://scv.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://zls.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://eui.sjlbkw.cn

[F06] 删除文件
来源：http://jfi.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://qbt.yuanzhike.top

PHP:  unlink("a.txt");
来源：http://sli.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bgr.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://spj.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bmg.pycfn.com

Go:   os.Remove("a.txt")
来源：http://rxi.cashguo.top

Ruby: File.delete("a.txt")
来源：http://czv.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://avz.tarul.cn

[F07] 创建目录（含多级）
来源：http://xvc.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rea.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bku.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ncw.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ifs.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://brw.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mwa.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://krf.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://evh.zhixingplan.top

[F08] 遍历目录
来源：http://gze.fanxiaobao.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://vfp.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://goq.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://lki.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://sha.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fwh.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ivh.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://ypq.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://tum.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://moe.zhongyouzk.top

Py:   os.path.getsize("a.txt")
来源：http://oum.52xcode.cn

PHP:  filesize("a.txt");
来源：http://qts.jinghuilouyu.cn

JS:   fs.statSync("a.txt").size
来源：http://vlc.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://sgu.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://twq.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ala.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://jje.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://fzj.52xcode.cn

[F10] 取文件扩展名 / 文件名
来源：http://gtt.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lcm.wangdashe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rpe.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yjw.yj20258.top

TS:   path.extname("a.txt")
来源：http://nps.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bsp.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ioe.nanxuanxn.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://adk.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nji.tarul.cn

[F11] 复制与移动文件
来源：http://zzv.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://etp.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fgu.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jqf.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsv.feifeiyinyue.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pge.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tyt.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://emn.ehwqpu.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qnd.birdmap.top

[F12] CSV 读写
来源：http://gqu.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vuf.xuanzx.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pci.iojbl.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ywf.shzxlz.cn

TS:   // 同上
来源：http://phx.chenzaomai.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://phz.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ewi.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zjm.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iix.tanke756.top

================================================================================
来源：http://bsu.tanke756.top

G. 面向对象
来源：http://hix.yj202588.top

================================================================================
来源：http://huj.fehbvm.com

[G01] 定义类
来源：http://apr.fanxiaobao.xyz

Py:   class User: pass
来源：http://wnc.chenjidiqi.icu

PHP:  class User {}
来源：http://jnk.shzxlz.cn

JS:   class User {}
来源：http://pgc.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://peo.aizwys.cn

Java: class User {}
来源：http://fau.cashguo.top

Go:   type User struct { Name string }
来源：http://pox.epnwcf.com

Ruby: class User; end
来源：http://wfs.ydzc1.top

C#:   class User {}
来源：http://env.aizwys.cn

[G02] 构造函数
来源：http://vba.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://piv.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://txq.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://jlo.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://fiy.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://uii.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jsb.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://ysv.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://qrs.cqqwz.cn

[G03] 实例属性
来源：http://qpq.yangfankeji.com

Py:   self.name = "x"
来源：http://jmp.dashuyun.cn

PHP:  public string $name = "x";
来源：http://qpt.9152youxi.cn

JS:   this.name = "x";
来源：http://sqv.jinqigfzy.top

TS:   name: string = "x";
来源：http://uzw.cashguo.top

Java: private String name;
来源：http://fom.epnwcf.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wrd.vehdjk.com

Ruby: @name = "x"
来源：http://wqa.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://uxv.jiagoushi.top

[G04] 定义方法
来源：http://hon.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://gcq.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lcd.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://uqe.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://fmk.pycfn.com

Java: String greet() { return name; }
来源：http://nnt.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://qzf.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://wtw.bbcook.cn

C#:   public string Greet() => Name;
来源：http://xsi.yongpay.top

[G05] 继承
来源：http://suj.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://okt.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://zxd.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://wrb.guannengcc.top

TS:   class Admin extends User {}
来源：http://pav.pycfn.com

Java: class Admin extends User {}
来源：http://mpy.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nzj.gzhubu.top

Ruby: class Admin < User; end
来源：http://nlb.sufxvd.cn

C#:   class Admin : User {}
来源：http://jin.meibo888.top

[G06] 重写方法
来源：http://bms.yonumen.top

Py:   def greet(self): return "admin"
来源：http://nif.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bct.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://xrl.tarul.cn

TS:   greet(): string { return "admin"; }
来源：http://ada.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://oct.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hiw.ppjwa.cn

Ruby: def greet; "admin"; end
来源：http://zgl.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://exq.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://vqa.cqqwz.cn

Py:   super().greet()
来源：http://psx.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://xph.jianghu66.top

JS:   super.greet();
来源：http://tpp.kuanghao11.cn

TS:   super.greet();
来源：http://fer.tianlin.xyz

Java: super.greet();
来源：http://ydn.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pxj.ydjk.org.cn

Ruby: super
来源：http://wjg.0kj1m.cn

C#:   base.Greet();
来源：http://bgb.ydjk.org.cn

[G08] 静态方法与属性
来源：http://amp.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fuu.havefunace.top

PHP:  public static function f() {}
来源：http://hha.ppjwa.cn

JS:   static f() {}
来源：http://tqt.hnxiangtu.top

TS:   static f(): void {}
来源：http://inl.ybcxt.top

Java: static void f() {}
来源：http://lle.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfx.ybcxt.top

Ruby: def self.f; end
来源：http://tzv.jqgfzy.top

C#:   public static void F() {}
来源：http://ngl.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://kdr.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://wpw.meibo888.top

PHP:  interface Shape { public function area(): float; }
来源：http://xyp.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fll.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://yya.yj20258888.top

Java: interface Shape { double area(); }
来源：http://orj.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://jdf.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pnp.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://nhn.feifeiyinyue.top

[G10] 访问控制
来源：http://mav.316326.xyz

Py:   约定 _protected / __private（不强制）
来源：http://shj.chenlongwang.top

PHP:  public / protected / private
来源：http://itx.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://zvs.wangdashe.top

TS:   public / protected / private
来源：http://mkj.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://rpp.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ufn.jlsjyb.cn

Ruby: public / protected / private
来源：http://ohf.daria6918.cn

C#:   public / protected / private / internal
来源：http://yka.dashuyun.cn

[G11] getter / setter
来源：http://uzj.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://lrk.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tjy.gotoacloud.top

JS:   get name() { return this._name; }
来源：http://lwp.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://hex.yfazqb.com

Java: public String getName() { return name; }
来源：http://xbn.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mnw.fehbvm.com

Ruby: attr_accessor :name
来源：http://pef.tian-w.cn

C#:   public string Name { get; set; }
来源：http://msc.jyoumei.cn

[G12] 对象转字符串
来源：http://ezo.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://dly.shanyushiyangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mtj.ivvv.top

JS:   toString() { return this.name; }
来源：http://yby.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://vmq.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://afu.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iui.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://jej.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://moq.zycfv.cn

[G13] 判断对象类型
来源：http://whd.jiagoushi.top

Py:   isinstance(u, User)
来源：http://gcj.ctjpmb.com

PHP:  $u instanceof User
来源：http://kdd.fzhhl.top

JS:   u instanceof User
来源：http://sam.ppjwa.cn

TS:   u instanceof User
来源：http://nfz.shuidangran.top

Java: u instanceof User
来源：http://bzh.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nkn.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://opb.0kj1m.cn

C#:   u is User
来源：http://adu.svipenyu.cn

[G14] 数据类 / record
来源：http://paa.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zuj.cqqwz.cn

PHP:  // 用 readonly 属性模拟
来源：http://rum.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://ngi.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://wmv.sweek.top

Java: record User(String name, int age) {}
来源：http://dbb.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://cia.kuanghao11.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xyi.hfpthk.cn

C#:   record User(string Name, int Age);
来源：http://utg.xinyue.icu

[G15] 枚举
来源：http://ofg.dashuyun.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aoh.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jpc.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cop.yvedp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cae.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://cix.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rzs.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://dry.tanke756.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sii.yj20258.top

[G16] 对象转数组 / 字典
来源：http://snk.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bnk.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://bot.xuanzx.com

JS:   Object.entries(obj)
来源：http://cmu.havefunace.top

TS:   Object.entries(obj)
来源：http://mhv.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://llf.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uei.zhoulong.xyz

Ruby: obj.instance_variables
来源：http://jea.chenlongwang.top

C#:   // 用反射或 System.Text.Json
来源：http://pdg.bbcook.cn

================================================================================
来源：http://sue.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://kna.chenjidiqi.icu

================================================================================
来源：http://wiz.guowangkeji.top

[H01] try / catch 基础
来源：http://sqf.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ltp.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jiw.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oac.smart0.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://abt.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hyu.wangdashe.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ujr.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://awu.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fkr.hnqzz.top

[H02] finally / ensure 收尾
来源：http://fby.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://sxh.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://utb.zhaomingkeji.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://prj.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dca.jinqigfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://kym.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmy.fanxiaobao.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://hqn.shangyingyoupin.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tuw.fehbvm.com

[H03] 主动抛出异常
来源：http://mof.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://hgi.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oze.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://hhh.gogol.net.cn

TS:   throw new Error("错误信息");
来源：http://akb.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fgx.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pbz.ivvv.top

Ruby: raise ArgumentError, "错误信息"
来源：http://yrx.nanxinkj.top

C#:   throw new ArgumentException("错误信息");
来源：http://kro.sjlbkw.cn

[H04] 自定义异常类型
来源：http://avp.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://qdm.nwbrower.top

PHP:  class MyError extends RuntimeException {}
来源：http://hed.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://dck.52xcode.cn

TS:   class MyError extends Error {}
来源：http://vob.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://otk.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dtb.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://szw.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://tdj.ehwqpu.com

[H05] 捕获特定类型
来源：http://xmr.zhengqikj.top

Py:   except ValueError as e:
来源：http://rvk.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lwg.jiagoushi.top

JS:   if (e instanceof TypeError) {}
来源：http://jov.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://eqo.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://vqa.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kuq.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://azg.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ray.smart0.xyz

[H06] 可选值 / 空值安全访问
来源：http://mbq.nwbrower.top

Py:   value = d.get("k") or default
来源：http://quy.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://bhi.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://img.dashuyun.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kmk.wangdashe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mru.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lbg.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://ntm.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://oiw.dianchejie.cn

[H07] 断言
来源：http://iap.nanxuanxn.top

Py:   assert x > 0, "必须为正"
来源：http://git.nwbrower.top

PHP:  assert($x > 0);
来源：http://mxc.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://kzv.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://jhe.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://lre.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hlp.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://asf.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://vah.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://wcb.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://pnx.cashguo.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vuu.yj20258.top

JS:   e.message;  e.stack
来源：http://dmb.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://osw.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://stl.andypj.xyz

Go:   err.Error()
来源：http://bfo.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://yjb.shanyushiyangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://axf.sxryk.cn

[H09] 带错误码的异常
来源：http://aue.wangshuangyany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oeu.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://etq.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lnc.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nea.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fdy.yj202588.top


<!-- 参考信息 -->