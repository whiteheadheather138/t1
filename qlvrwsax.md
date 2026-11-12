代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rke.zhiwuduotai.top

Ruby: File.write("a.txt", "hi")
来源：http://obm.nanxuanxn.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pss.yj202588.top

[F04] 追加写入文件
来源：http://dgf.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyj.ivvv.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kqg.ybcxt.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://brn.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xiw.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://njw.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nlg.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kov.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vwf.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://moh.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pkb.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://cgr.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://ief.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://hzc.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://imv.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://chr.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://oxl.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://zxv.kuanghao11.cn

[F06] 删除文件
来源：http://brf.nwbrower.top

Py:   os.remove("a.txt")
来源：http://vxd.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://fwt.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aas.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://ehu.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qsn.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://zfx.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://dlw.hywenlv.cn

C#:   File.Delete("a.txt");
来源：http://azb.smart0.xyz

[F07] 创建目录（含多级）
来源：http://hsm.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vor.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hdl.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ewy.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shq.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dua.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://els.ydzc1.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cvz.gogol.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aob.dashuyun.cn

[F08] 遍历目录
来源：http://iop.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dod.hongshengwenyu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zsw.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://nnz.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://rbl.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hzr.hysaishi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://adj.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://dun.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://ipx.ydzc1.top

[F09] 获取文件大小
来源：http://cre.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://juw.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://now.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://jtr.sufxvd.cn

TS:   fs.statSync("a.txt").size
来源：http://qhi.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://snf.c1oappe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://erk.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://etk.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://rbu.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://noa.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://osl.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kvs.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sho.yvedp.cn

TS:   path.extname("a.txt")
来源：http://iuq.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oey.hnxiangtu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cod.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://srz.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xtr.xylfe.cn

[F11] 复制与移动文件
来源：http://mjw.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pin.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sdi.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zum.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xjp.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://seh.tarul.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://utp.redwolf501.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dlk.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zjj.jqgfzy.top

[F12] CSV 读写
来源：http://btq.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aqa.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tbt.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rfm.xylfe.cn

TS:   // 同上
来源：http://lqi.zdbjq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fym.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://klo.svipenyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eks.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dqp.ppjwa.cn

================================================================================
来源：http://hbe.xuetiantiany.cn

G. 面向对象
来源：http://dwm.0kj1m.cn

================================================================================
来源：http://lvn.gogol.net.cn

[G01] 定义类
来源：http://yvm.meibo888.top

Py:   class User: pass
来源：http://pqp.hcnkem.com

PHP:  class User {}
来源：http://xbk.mhx1999.top

JS:   class User {}
来源：http://dra.meibo888.top

TS:   class User { name: string = ""; }
来源：http://udl.zdbjq.cn

Java: class User {}
来源：http://jro.zdqjudy.top

Go:   type User struct { Name string }
来源：http://krs.gzhubu.top

Ruby: class User; end
来源：http://ohk.jqgufenzy.top

C#:   class User {}
来源：http://obm.daria6918.cn

[G02] 构造函数
来源：http://zko.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://jqs.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://euf.bjfxy.top

JS:   constructor(name) { this.name = name; }
来源：http://qat.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://sxy.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://gex.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gxl.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://xwq.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://fzk.yuxming.cn

[G03] 实例属性
来源：http://ffr.smart0.xyz

Py:   self.name = "x"
来源：http://xji.cucudq.cn

PHP:  public string $name = "x";
来源：http://mru.kuanghao11.cn

JS:   this.name = "x";
来源：http://tgl.c1oappe.top

TS:   name: string = "x";
来源：http://hfj.bjfxy.top

Java: private String name;
来源：http://zbl.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dbw.52xcode.cn

Ruby: @name = "x"
来源：http://byd.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://bae.tianlin.xyz

[G04] 定义方法
来源：http://aga.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://rhp.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xsa.shuidangran.top

JS:   greet() { return this.name; }
来源：http://kfx.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://dgp.bbcook.cn

Java: String greet() { return name; }
来源：http://zxh.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aol.ydjk.org.cn

Ruby: def greet; @name; end
来源：http://wov.bjfxy.top

C#:   public string Greet() => Name;
来源：http://rpw.dashuyun.cn

[G05] 继承
来源：http://hha.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://jab.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://mol.daria6918.cn

JS:   class Admin extends User {}
来源：http://klu.dashuyun.cn

TS:   class Admin extends User {}
来源：http://sbq.sufxvd.cn

Java: class Admin extends User {}
来源：http://jkw.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xjg.fengsongda.top

Ruby: class Admin < User; end
来源：http://biz.bjfxy.top

C#:   class Admin : User {}
来源：http://mnl.yfazqb.com

[G06] 重写方法
来源：http://gwn.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://vqk.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pab.dianchejie.cn

JS:   greet() { return "admin"; }
来源：http://yxv.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://esd.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://mno.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ybu.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://aqt.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://fzd.gaohongyu789.top

[G07] 调用父类方法
来源：http://xfa.pycfn.com

Py:   super().greet()
来源：http://qqa.vehdjk.com

PHP:  parent::greet();
来源：http://kqx.pengpengdd.cyou

JS:   super.greet();
来源：http://bux.fzhhl.top

TS:   super.greet();
来源：http://vgs.jqgfzy.top

Java: super.greet();
来源：http://xlj.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xfy.hammf.cn

Ruby: super
来源：http://cnm.yj202588.top

C#:   base.Greet();
来源：http://swy.yuxming.cn

[G08] 静态方法与属性
来源：http://koo.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fxe.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://jdo.iojbl.cn

JS:   static f() {}
来源：http://dxs.9152youxi.cn

TS:   static f(): void {}
来源：http://sbs.yj20258.top

Java: static void f() {}
来源：http://dqt.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gua.jinqigfzy.top

Ruby: def self.f; end
来源：http://qvd.shangyingyoupin.top

C#:   public static void F() {}
来源：http://bxu.zycfv.cn

[G09] 接口 / 抽象类
来源：http://jir.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://bbh.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://wmu.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bcd.hesvh.cn

TS:   interface Shape { area(): number; }
来源：http://fyf.xylfe.cn

Java: interface Shape { double area(); }
来源：http://zju.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://jym.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bgf.zhijiandao.cn

C#:   interface IShape { double Area(); }
来源：http://oyz.nanxinkj.top

[G10] 访问控制
来源：http://ktc.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://omm.hysaishi.cn

PHP:  public / protected / private
来源：http://tkh.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://epe.yanxiufei.cn

TS:   public / protected / private
来源：http://fdp.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://oag.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wlx.0kj1m.cn

Ruby: public / protected / private
来源：http://pfh.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://hos.epnwcf.com

[G11] getter / setter
来源：http://ltu.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://llk.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jfu.aibaodan.cn

JS:   get name() { return this._name; }
来源：http://upb.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://thq.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://kvf.redwolf501.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ulu.hesvh.cn

Ruby: attr_accessor :name
来源：http://jyn.yueranfly.top

C#:   public string Name { get; set; }
来源：http://lpg.fktsv.cn

[G12] 对象转字符串
来源：http://ikt.hnxiangtu.top

Py:   def __str__(self): return self.name
来源：http://zri.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ere.yongpay.top

JS:   toString() { return this.name; }
来源：http://das.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://agr.sysykeji.top

Java: @Override public String toString() { return name; }
来源：http://end.fzhhl.top

Go:   func (u User) String() string { return u.Name }
来源：http://gnj.fehbvm.com

Ruby: def to_s; @name; end
来源：http://pse.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://hlq.zhixingplan.top

[G13] 判断对象类型
来源：http://nof.sxryk.cn

Py:   isinstance(u, User)
来源：http://qoq.tanke756.top

PHP:  $u instanceof User
来源：http://tmn.havefunace.top

JS:   u instanceof User
来源：http://lak.fanxiaobao.xyz

TS:   u instanceof User
来源：http://urc.hfpthk.cn

Java: u instanceof User
来源：http://jzx.hysaishi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://slq.snrcjt.cn

Ruby: u.is_a?(User)
来源：http://euz.c1oappe.top

C#:   u is User
来源：http://fiq.cdnleiting.top

[G14] 数据类 / record
来源：http://pil.xuetiantiany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://luw.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://rel.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://gra.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://ked.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://oii.vqdsnc.cn

Go:   type User struct { Name string; Age int }
来源：http://hwm.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://erd.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://boz.daxiang520.top

[G15] 枚举
来源：http://pdf.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kue.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://iel.pycfn.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lui.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rhq.andypj.xyz

Java: enum Color { RED, GREEN }
来源：http://dzz.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tjv.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://gby.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://egy.xylfe.cn

[G16] 对象转数组 / 字典
来源：http://een.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rrl.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://ivt.jyoumei.cn

JS:   Object.entries(obj)
来源：http://jgx.yvedp.cn

TS:   Object.entries(obj)
来源：http://utg.jinqigufen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jll.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://uop.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://jje.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://ppz.zycfv.cn

================================================================================
来源：http://cww.cheryme.top

H. 异常与错误处理
来源：http://axy.0kj1m.cn

================================================================================
来源：http://wyb.snrcjt.cn

[H01] try / catch 基础
来源：http://tfc.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://thh.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vbe.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hce.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zzz.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://znt.jinqigufen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nvm.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ood.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mhx.tian-w.cn

[H02] finally / ensure 收尾
来源：http://qft.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://qyh.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gsv.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://rsx.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fqz.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cdg.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://min.yj202588.top

Ruby: begin; f; ensure; cleanup; end
来源：http://aph.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://tns.cashguo.top

[H03] 主动抛出异常
来源：http://akh.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://hfo.sxryk.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cfe.daria6918.cn

JS:   throw new Error("错误信息");
来源：http://oxi.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://mvk.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fdp.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rfk.zhoulong.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://hyy.xylfe.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mxg.gotoacloud.top

[H04] 自定义异常类型
来源：http://ltd.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://msu.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://urd.havefunace.top

JS:   class MyError extends Error {}
来源：http://icy.hesvh.cn

TS:   class MyError extends Error {}
来源：http://pgc.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://bij.sufxvd.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sbz.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://kpo.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://oro.cqqwz.cn

[H05] 捕获特定类型
来源：http://wcf.fehbvm.com

Py:   except ValueError as e:
来源：http://mee.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ypw.xziqi.cn

JS:   if (e instanceof TypeError) {}
来源：http://qji.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://iug.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://qjg.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ppb.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://pvz.jinqigfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cir.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://kan.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://lpl.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://fgm.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://uod.svipenyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sga.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mha.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oef.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://gyv.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://mfx.xingfuxueyuan.xyz

[H07] 断言
来源：http://ndj.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://yhe.gzhubu.top

PHP:  assert($x > 0);
来源：http://ovp.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://fsu.havefunace.top

TS:   console.assert(x > 0);
来源：http://vyy.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://mpv.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yoj.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://klg.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://scx.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://bdw.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://bmn.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nhm.0kj1m.cn


<!-- 参考信息 -->