代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tun.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ywz.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wlp.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhy.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hgg.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wuc.zhoulong.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://adr.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ord.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://aec.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dhm.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://vmw.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://inw.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://cpa.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eie.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ico.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://mex.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://wcl.9152youxi.cn

[F06] 删除文件
来源：http://ieb.meibo888.top

Py:   os.remove("a.txt")
来源：http://phm.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://zvt.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://wjh.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://zmv.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dsp.tanke756.top

Go:   os.Remove("a.txt")
来源：http://gwv.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://abn.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://kws.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://gbd.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mlf.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ymq.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jbp.52xcode.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vde.shzxlz.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vrx.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ozx.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xss.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://otn.smart0.xyz

[F08] 遍历目录
来源：http://vsz.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ufh.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tty.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://eju.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://jcb.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://san.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ele.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://qof.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://aeq.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://jfq.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://eob.epnwcf.com

PHP:  filesize("a.txt");
来源：http://kno.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://dcu.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://cmd.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dsh.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jrz.fzhhl.top

Ruby: File.size("a.txt")
来源：http://xcl.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://hhl.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://vrm.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mdi.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uyp.hongshengwenyu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gxh.jianghu66.top

TS:   path.extname("a.txt")
来源：http://ovd.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xog.gotoacloud.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uoz.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vev.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cyx.zdbjq.cn

[F11] 复制与移动文件
来源：http://pfe.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldn.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bqc.cdnleiting.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qky.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zem.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wgt.yonumen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dwp.aibaodan.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hvg.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uij.cashguo.top

[F12] CSV 读写
来源：http://eag.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jiv.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gon.zhixingplan.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qtq.zhoulong.xyz

TS:   // 同上
来源：http://tkj.ywan-chungtsiang.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vpa.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nao.zhongyouzk.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wxe.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zjq.cqqwz.cn

================================================================================
来源：http://lkg.cashguo.top

G. 面向对象
来源：http://aqj.cdnleiting.top

================================================================================
来源：http://hod.zhiwuduotai.top

[G01] 定义类
来源：http://mxd.hongshengwenyu.top

Py:   class User: pass
来源：http://whf.yangfankeji.com

PHP:  class User {}
来源：http://trp.sysykeji.top

JS:   class User {}
来源：http://vxp.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://qnk.zycfv.cn

Java: class User {}
来源：http://qqe.cashguo.top

Go:   type User struct { Name string }
来源：http://hih.jqgufenzy.top

Ruby: class User; end
来源：http://knx.havefunace.top

C#:   class User {}
来源：http://cqy.zhixingplan.top

[G02] 构造函数
来源：http://gyz.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://igv.yj20258.top

PHP:  public function __construct(public string $name) {}
来源：http://idy.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://ohe.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://vxn.shuidangran.top

Java: User(String name) { this.name = name; }
来源：http://wat.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bvg.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://hrk.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://nci.uphjek.com

[G03] 实例属性
来源：http://hld.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://odo.zhaomingkeji.xyz

PHP:  public string $name = "x";
来源：http://pyw.yueranfly.top

JS:   this.name = "x";
来源：http://znt.birdmap.top

TS:   name: string = "x";
来源：http://yjh.yfazqb.com

Java: private String name;
来源：http://gfb.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://epy.yvedp.cn

Ruby: @name = "x"
来源：http://vmn.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://ttm.jlsjyb.cn

[G04] 定义方法
来源：http://rmx.zhoulong.xyz

Py:   def greet(self): return self.name
来源：http://zpn.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://knb.guannengcc.top

JS:   greet() { return this.name; }
来源：http://brq.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://hhu.aibaodan.cn

Java: String greet() { return name; }
来源：http://xkn.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qex.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://yyw.316326.xyz

C#:   public string Greet() => Name;
来源：http://mvd.hongshengwenyu.top

[G05] 继承
来源：http://hhz.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://tef.daxiang520.top

PHP:  class Admin extends User {}
来源：http://hsf.zhixingplan.top

JS:   class Admin extends User {}
来源：http://qam.xziqi.cn

TS:   class Admin extends User {}
来源：http://hvm.hcnkem.com

Java: class Admin extends User {}
来源：http://tcj.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rov.zhixingplan.top

Ruby: class Admin < User; end
来源：http://zbp.xylfe.cn

C#:   class Admin : User {}
来源：http://sqd.wangshuangyany.cn

[G06] 重写方法
来源：http://bte.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://yuu.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ydq.yonumen.top

JS:   greet() { return "admin"; }
来源：http://uke.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://svd.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://ucr.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bwh.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://ckx.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://iwz.zhijiandao.cn

[G07] 调用父类方法
来源：http://poo.hnqzz.top

Py:   super().greet()
来源：http://kyi.pengpengdd.cyou

PHP:  parent::greet();
来源：http://kil.nwbrower.top

JS:   super.greet();
来源：http://ftm.yuanzhike.top

TS:   super.greet();
来源：http://fhx.nanxinkj.top

Java: super.greet();
来源：http://jnp.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yhe.nanxinkj.top

Ruby: super
来源：http://koz.sxryk.cn

C#:   base.Greet();
来源：http://utp.bbcook.cn

[G08] 静态方法与属性
来源：http://cqk.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vkh.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://zhz.wangshuangyany.cn

JS:   static f() {}
来源：http://vil.guowangkeji.top

TS:   static f(): void {}
来源：http://lgh.jinghuilouyu.cn

Java: static void f() {}
来源：http://zou.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ril.vehdjk.com

Ruby: def self.f; end
来源：http://hzp.fzhhl.top

C#:   public static void F() {}
来源：http://qlp.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://euq.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pfi.sysykeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://khc.zhoulong.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpd.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://uya.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://qzk.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://bct.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://djp.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://dlq.c1oappe.top

[G10] 访问控制
来源：http://ntj.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://rxz.nanxuanxn.top

PHP:  public / protected / private
来源：http://vsp.zycfv.cn

JS:   #private 字段；其余公开
来源：http://dlg.aizwys.cn

TS:   public / protected / private
来源：http://ulj.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://szw.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tuh.meibo888.top

Ruby: public / protected / private
来源：http://kun.cqqwz.cn

C#:   public / protected / private / internal
来源：http://mcb.xziqi.cn

[G11] getter / setter
来源：http://fpx.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://xpw.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bor.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://szp.chenzaomai.com

TS:   get name(): string { return this._name; }
来源：http://nkp.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://ovi.yfazqb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://uew.cucudq.cn

Ruby: attr_accessor :name
来源：http://mwy.daria6918.cn

C#:   public string Name { get; set; }
来源：http://fxo.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://fuu.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://vpu.sysykeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://isi.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://drd.hnqzz.top

TS:   toString(): string { return this.name; }
来源：http://fht.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://sme.haohaochexian.top

Go:   func (u User) String() string { return u.Name }
来源：http://wgn.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://chj.wangdashe.top

C#:   public override string ToString() => Name;
来源：http://fpz.epnwcf.com

[G13] 判断对象类型
来源：http://yoq.gzhubu.top

Py:   isinstance(u, User)
来源：http://vso.yanxiufei.cn

PHP:  $u instanceof User
来源：http://ulu.yonumen.top

JS:   u instanceof User
来源：http://xsa.jinqigfzy.top

TS:   u instanceof User
来源：http://qyk.fzhhl.top

Java: u instanceof User
来源：http://jah.dashuyun.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ogl.mhx1999.top

Ruby: u.is_a?(User)
来源：http://vpy.fzhhl.top

C#:   u is User
来源：http://tby.daria6918.cn

[G14] 数据类 / record
来源：http://ngo.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wgk.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://quf.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://hfy.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://zyd.guowangkeji.top

Java: record User(String name, int age) {}
来源：http://itl.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://evm.gaohongyu789.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xkf.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://jtn.shangyingyoupin.top

[G15] 枚举
来源：http://dwo.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kik.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qpz.nanxinkj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqd.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uwj.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://fzs.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xor.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://fph.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://thz.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://irq.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://imm.chenlongwang.top

PHP:  get_object_vars($obj);
来源：http://ecd.ydzc1.top

JS:   Object.entries(obj)
来源：http://epc.sjlbkw.cn

TS:   Object.entries(obj)
来源：http://lok.vqdsnc.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zci.cheryme.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://aqu.meibo888.top

Ruby: obj.instance_variables
来源：http://bpx.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://isp.wangshuangyany.cn

================================================================================
来源：http://giq.tarul.cn

H. 异常与错误处理
来源：http://hxo.ydjk.org.cn

================================================================================
来源：http://lxv.shanyushiyangtech.top

[H01] try / catch 基础
来源：http://vyq.feifeiyinyue.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pyn.quarkkingdee.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cqw.pengpengdd.cyou

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://awq.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://svx.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gts.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://alh.epnwcf.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://byn.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://now.daria6918.cn

[H02] finally / ensure 收尾
来源：http://ski.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aoh.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ebq.zycfv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gtf.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rou.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ozx.vehdjk.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://wyj.yfazqb.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ndz.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wau.havefunace.top

[H03] 主动抛出异常
来源：http://zjf.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://ext.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qxb.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://jjs.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://gve.cqqwz.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mgq.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wot.gaohongyu789.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bvq.birdmap.top

C#:   throw new ArgumentException("错误信息");
来源：http://hja.iojbl.cn

[H04] 自定义异常类型
来源：http://zzz.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://jqb.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eks.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://apf.fehbvm.com

TS:   class MyError extends Error {}
来源：http://ztn.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://pab.xingfuxueyuan.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qys.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://bqp.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://yas.xinyue.icu

[H05] 捕获特定类型
来源：http://bdy.zhijiandao.cn

Py:   except ValueError as e:
来源：http://ywp.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gig.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://cxa.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://few.vehdjk.com

Java: catch (IOException | SQLException e) {}
来源：http://lyc.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vni.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://joj.xuetiantiany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://buu.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://oyd.gzhubu.top

Py:   value = d.get("k") or default
来源：http://adt.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://lra.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rws.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://msr.meibo888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dns.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jpm.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://nkv.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://kon.hammf.cn

[H07] 断言
来源：http://deg.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://hrl.ybcxt.top

PHP:  assert($x > 0);
来源：http://ffy.cashguo.top

JS:   console.assert(x > 0);
来源：http://doq.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://tpt.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://xyd.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fuk.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pxi.yuxming.cn

C#:   Debug.Assert(x > 0);
来源：http://gom.zhijiandao.cn

[H08] 获取错误信息与堆栈
来源：http://vpl.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://ava.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dsc.haohaochexian.top

JS:   e.message;  e.stack
来源：http://row.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xsv.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://akq.yuxming.cn

Go:   err.Error()
来源：http://lcf.hfpthk.cn


<!-- 参考信息 -->