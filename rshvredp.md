代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ads.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rkv.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xtb.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wqs.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://oov.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gpr.shuidangran.top

PHP:  file_exists("a.txt");
来源：http://aod.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://sbf.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://owh.cqqwz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nnz.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ify.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://qeg.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://tlz.hysaishi.cn

[F06] 删除文件
来源：http://xfi.daria6918.cn

Py:   os.remove("a.txt")
来源：http://zbr.sxryk.cn

PHP:  unlink("a.txt");
来源：http://zug.xziqi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ysr.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://lgf.hfpthk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dim.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://tuy.wangshuangyany.cn

Ruby: File.delete("a.txt")
来源：http://mgi.ivvv.top

C#:   File.Delete("a.txt");
来源：http://ezf.cdnleiting.top

[F07] 创建目录（含多级）
来源：http://dtt.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qhd.tian-w.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rql.hywenlv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://may.yueranfly.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vfr.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mci.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uuf.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kqz.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bux.redwolf501.top

[F08] 遍历目录
来源：http://tpk.daxiang520.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lxz.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hsc.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://gan.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://nig.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fxs.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lvd.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://bdx.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://pyk.cdnleiting.top

[F09] 获取文件大小
来源：http://nvd.yonumen.top

Py:   os.path.getsize("a.txt")
来源：http://cjt.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://qda.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://dul.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://bqh.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rkv.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ytm.yj20258.top

Ruby: File.size("a.txt")
来源：http://bbh.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://wxr.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://hsy.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wlo.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qha.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lyu.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://crq.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lrx.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fiq.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bcj.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lla.yj20258888.top

[F11] 复制与移动文件
来源：http://cnn.yvedp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rpn.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gno.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sik.xingfuxueyuan.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egi.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gro.shanyushiyangtech.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://obv.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dht.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://okj.cdnleiting.top

[F12] CSV 读写
来源：http://gyy.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yge.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eru.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tsb.yonumen.top

TS:   // 同上
来源：http://spf.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lsg.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cyo.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kid.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pyu.gotoacloud.top

================================================================================
来源：http://zje.jlsjyb.cn

G. 面向对象
来源：http://rqh.jianghu66.top

================================================================================
来源：http://xqf.fengsongda.top

[G01] 定义类
来源：http://jxc.epnwcf.com

Py:   class User: pass
来源：http://ysa.yvedp.cn

PHP:  class User {}
来源：http://whd.quarkkingdee.top

JS:   class User {}
来源：http://kyn.yj202588.top

TS:   class User { name: string = ""; }
来源：http://klq.yvedp.cn

Java: class User {}
来源：http://pdj.zycfv.cn

Go:   type User struct { Name string }
来源：http://zyn.ywan-chungtsiang.top

Ruby: class User; end
来源：http://efg.birdmap.top

C#:   class User {}
来源：http://ujj.gaohongyu789.top

[G02] 构造函数
来源：http://fgg.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://waj.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://btr.daria6918.cn

JS:   constructor(name) { this.name = name; }
来源：http://tyz.kuanghao11.cn

TS:   constructor(public name: string) {}
来源：http://kos.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://sib.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vky.yuxming.cn

Ruby: def initialize(name); @name = name; end
来源：http://pfb.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://dap.shuidangran.top

[G03] 实例属性
来源：http://bil.jqgfzy.top

Py:   self.name = "x"
来源：http://dra.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://zan.svipenyu.cn

JS:   this.name = "x";
来源：http://dry.chenlongwang.top

TS:   name: string = "x";
来源：http://ekt.ybcxt.top

Java: private String name;
来源：http://tmt.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rgt.xuetiantiany.cn

Ruby: @name = "x"
来源：http://kmd.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://rlw.yanxiufei.cn

[G04] 定义方法
来源：http://szq.redwolf501.top

Py:   def greet(self): return self.name
来源：http://ady.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qsb.yuxming.cn

JS:   greet() { return this.name; }
来源：http://zms.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://mpp.epnwcf.com

Java: String greet() { return name; }
来源：http://rfn.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vvi.0kj1m.cn

Ruby: def greet; @name; end
来源：http://pre.tanke756.top

C#:   public string Greet() => Name;
来源：http://cyb.fktsv.cn

[G05] 继承
来源：http://xhx.ybcxt.top

Py:   class Admin(User): pass
来源：http://tvd.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://dbc.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://icf.yfazqb.com

TS:   class Admin extends User {}
来源：http://xau.guowangkeji.top

Java: class Admin extends User {}
来源：http://jak.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zgm.xylfe.cn

Ruby: class Admin < User; end
来源：http://gur.zycfv.cn

C#:   class Admin : User {}
来源：http://hck.yvedp.cn

[G06] 重写方法
来源：http://rav.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://oga.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mld.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://wff.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://luv.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://xeb.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kvr.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://mrr.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://rtq.chenzaomai.com

[G07] 调用父类方法
来源：http://bsi.xuanzx.com

Py:   super().greet()
来源：http://gjj.yonumen.top

PHP:  parent::greet();
来源：http://gja.c1oappe.top

JS:   super.greet();
来源：http://shb.aizwys.cn

TS:   super.greet();
来源：http://cwg.52xcode.cn

Java: super.greet();
来源：http://tuj.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tne.andypj.xyz

Ruby: super
来源：http://lgb.tanke756.top

C#:   base.Greet();
来源：http://wom.tian-w.cn

[G08] 静态方法与属性
来源：http://ona.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nzm.yfazqb.com

PHP:  public static function f() {}
来源：http://xrz.smart0.xyz

JS:   static f() {}
来源：http://hui.shangyingyoupin.top

TS:   static f(): void {}
来源：http://tct.fanxiaobao.xyz

Java: static void f() {}
来源：http://gxz.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cva.ivvv.top

Ruby: def self.f; end
来源：http://ixw.sjlbkw.cn

C#:   public static void F() {}
来源：http://phd.hnqzz.top

[G09] 接口 / 抽象类
来源：http://mls.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://fjb.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://iqp.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dxe.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://xbb.dashuyun.cn

Java: interface Shape { double area(); }
来源：http://mqp.ydzc1.top

Go:   type Shape interface { Area() float64 }
来源：http://koy.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yde.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://dkv.iojbl.cn

[G10] 访问控制
来源：http://dgq.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://mgt.dashuyun.cn

PHP:  public / protected / private
来源：http://yxu.zhoulong.xyz

JS:   #private 字段；其余公开
来源：http://deb.sxryk.cn

TS:   public / protected / private
来源：http://onv.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://vvu.nwbrower.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rlp.ydzc1.top

Ruby: public / protected / private
来源：http://jcu.hfpthk.cn

C#:   public / protected / private / internal
来源：http://dlo.xziqi.cn

[G11] getter / setter
来源：http://hrr.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://wvs.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oex.cucudq.cn

JS:   get name() { return this._name; }
来源：http://jdc.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://qkc.aibaodan.cn

Java: public String getName() { return name; }
来源：http://ovb.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xbb.tian-w.cn

Ruby: attr_accessor :name
来源：http://iym.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://gbu.vqdsnc.cn

[G12] 对象转字符串
来源：http://jfd.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://pfl.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ftq.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://dsw.birdmap.top

TS:   toString(): string { return this.name; }
来源：http://nli.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://iov.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zgg.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://ryt.yj20258888.top

C#:   public override string ToString() => Name;
来源：http://kvd.ppjwa.cn

[G13] 判断对象类型
来源：http://qvo.ybcxt.top

Py:   isinstance(u, User)
来源：http://cjb.fehbvm.com

PHP:  $u instanceof User
来源：http://fwj.smart0.xyz

JS:   u instanceof User
来源：http://lzc.xziqi.cn

TS:   u instanceof User
来源：http://xnk.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://gwf.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tqg.316326.xyz

Ruby: u.is_a?(User)
来源：http://neh.yj20258888.top

C#:   u is User
来源：http://sax.ydzc1.top

[G14] 数据类 / record
来源：http://pjw.ehwqpu.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rui.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://qbg.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://peb.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://wwx.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://lkh.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://ird.yj20258.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ofl.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://sfe.wangshuangyany.cn

[G15] 枚举
来源：http://xjz.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://erb.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://abz.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xhh.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ofo.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://ech.sysykeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aja.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://csd.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zfk.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://byj.dashuyun.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nls.hammf.cn

PHP:  get_object_vars($obj);
来源：http://xkj.ppjwa.cn

JS:   Object.entries(obj)
来源：http://fkj.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://evn.zhixingplan.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eke.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mpf.bjfxy.top

Ruby: obj.instance_variables
来源：http://abk.havefunace.top

C#:   // 用反射或 System.Text.Json
来源：http://oht.guowangkeji.top

================================================================================
来源：http://nuk.jiagoushi.top

H. 异常与错误处理
来源：http://ojw.hywenlv.cn

================================================================================
来源：http://wbo.hcnkem.com

[H01] try / catch 基础
来源：http://vpx.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ysc.guowangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jui.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yap.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ivx.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tas.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dqj.xuanzx.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zxi.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rmy.9152youxi.cn

[H02] finally / ensure 收尾
来源：http://yil.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://kvq.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mjm.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fsz.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://usk.gogol.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pxq.tarul.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uoo.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://keo.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://kfj.xylfe.cn

[H03] 主动抛出异常
来源：http://wvs.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://fyr.xziqi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cec.shuidangran.top

JS:   throw new Error("错误信息");
来源：http://jqy.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://thj.guowangkeji.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yua.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nze.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kud.quarkkingdee.top

C#:   throw new ArgumentException("错误信息");
来源：http://jrb.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://vgg.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://cdz.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cxl.aizwys.cn

JS:   class MyError extends Error {}
来源：http://oqs.jinqigufen.top

TS:   class MyError extends Error {}
来源：http://vnq.havefunace.top

Java: class MyException extends RuntimeException {}
来源：http://raq.dianchejie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zhe.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://pqb.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://omb.tanke756.top

[H05] 捕获特定类型
来源：http://gbk.nanxuanxn.top

Py:   except ValueError as e:
来源：http://wug.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qte.ehwqpu.com

JS:   if (e instanceof TypeError) {}
来源：http://zvo.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://pes.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://gwx.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vgq.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://jhb.yongpay.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vyi.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://sqs.hongshengwenyu.top

Py:   value = d.get("k") or default
来源：http://uwv.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://qgy.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oid.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://kmj.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bbs.yanxiufei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kql.jqgufenzy.top

Ruby: d&.dig(:a, :b)
来源：http://dig.sweek.top

C#:   obj?.A?.B ?? default
来源：http://zmr.iojbl.cn

[H07] 断言
来源：http://his.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://lfm.cdnleiting.top

PHP:  assert($x > 0);
来源：http://cdj.316326.xyz

JS:   console.assert(x > 0);
来源：http://qop.tian-w.cn

TS:   console.assert(x > 0);
来源：http://tkt.sxryk.cn

Java: assert x > 0 : "必须为正";
来源：http://yws.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bwh.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://jdd.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://tpv.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://suc.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://feu.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gdq.cucudq.cn

JS:   e.message;  e.stack
来源：http://lbq.yangfankeji.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://boa.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cqd.epnwcf.com

Go:   err.Error()
来源：http://ree.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://lya.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://ckp.ybcxt.top

[H09] 带错误码的异常
来源：http://rdv.cucudq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sgq.guowangkeji.top


<!-- 参考信息 -->