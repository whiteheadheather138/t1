代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://bqi.gogol.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rps.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wal.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://unz.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sbi.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://qch.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ott.xylfe.cn

[F04] 追加写入文件
来源：http://ksf.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ein.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lfa.9152youxi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lld.ctjpmb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://adp.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ytv.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vbo.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vqa.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uxi.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://nyv.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ksa.yonumen.top

PHP:  file_exists("a.txt");
来源：http://wta.chenlongwang.top

JS:   fs.existsSync("a.txt")
来源：http://hui.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://iij.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yfc.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://frr.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://iwb.pycfn.com

C#:   File.Exists("a.txt")
来源：http://wmh.hongshengwenyu.top

[F06] 删除文件
来源：http://qsk.cqqwz.cn

Py:   os.remove("a.txt")
来源：http://jmb.jqgufenzy.top

PHP:  unlink("a.txt");
来源：http://lvi.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lwk.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://ffp.jiagoushi.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://afj.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://gpb.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://gas.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://wlc.aizwys.cn

[F07] 创建目录（含多级）
来源：http://gmo.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rlg.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wxq.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjs.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ojr.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xxr.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rhn.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jos.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vaw.c1oappe.top

[F08] 遍历目录
来源：http://sjy.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bbw.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lsx.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://tbl.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://klf.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vwe.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wqd.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://vpv.ydzc1.top

C#:   Directory.GetFiles("dir")
来源：http://sfj.wangshuangyany.cn

[F09] 获取文件大小
来源：http://pli.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://isz.cashguo.top

PHP:  filesize("a.txt");
来源：http://iff.hcnkem.com

JS:   fs.statSync("a.txt").size
来源：http://uje.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://crd.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://een.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tve.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://bmb.iojbl.cn

C#:   new FileInfo("a.txt").Length
来源：http://icc.zhiwuduotai.top

[F10] 取文件扩展名 / 文件名
来源：http://sfr.hnqzz.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fee.hongshengwenyu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ihs.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rul.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://vby.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sxl.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wsb.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qrj.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://she.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://nzo.ctjpmb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rht.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://slp.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ljf.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynm.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nye.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fcq.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kix.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kkd.dashuyun.cn

[F12] CSV 读写
来源：http://yny.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://icg.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kwq.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://peb.shangyingyoupin.top

TS:   // 同上
来源：http://ctv.hongshengwenyu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://arc.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zbu.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ofg.chenjidiqi.icu

C#:   // 无内置：用 CsvHelper 库
来源：http://xnt.havefunace.top

================================================================================
来源：http://brz.pengpengdd.cyou

G. 面向对象
来源：http://dpi.sxryk.cn

================================================================================
来源：http://xyg.jqgfzy.top

[G01] 定义类
来源：http://fgu.yfazqb.com

Py:   class User: pass
来源：http://ovq.zhengqikj.top

PHP:  class User {}
来源：http://kdq.meibo888.top

JS:   class User {}
来源：http://rrt.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://iab.tian-w.cn

Java: class User {}
来源：http://wuv.birdmap.top

Go:   type User struct { Name string }
来源：http://pci.uphjek.com

Ruby: class User; end
来源：http://dgk.hammf.cn

C#:   class User {}
来源：http://src.fktsv.cn

[G02] 构造函数
来源：http://wwz.52xcode.cn

Py:   def __init__(self, name): self.name = name
来源：http://yqg.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://aez.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ccw.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://qut.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://zht.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zrb.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://rjy.zdqjudy.top

C#:   public User(string name) { Name = name; }
来源：http://wfn.epnwcf.com

[G03] 实例属性
来源：http://npe.hongshengwenyu.top

Py:   self.name = "x"
来源：http://ehj.yfazqb.com

PHP:  public string $name = "x";
来源：http://btt.nanxinkj.top

JS:   this.name = "x";
来源：http://ygz.sxryk.cn

TS:   name: string = "x";
来源：http://nat.hnqzz.top

Java: private String name;
来源：http://vzy.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cht.kuanghao11.cn

Ruby: @name = "x"
来源：http://bfl.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://qep.zhaomingkeji.xyz

[G04] 定义方法
来源：http://rqn.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://ays.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yum.cheryme.top

JS:   greet() { return this.name; }
来源：http://ize.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://wlr.jianghu66.top

Java: String greet() { return name; }
来源：http://aff.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hmd.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://dab.tian-w.cn

C#:   public string Greet() => Name;
来源：http://koh.fehbvm.com

[G05] 继承
来源：http://eep.yj20258888.top

Py:   class Admin(User): pass
来源：http://qml.fktsv.cn

PHP:  class Admin extends User {}
来源：http://fhe.aibaodan.cn

JS:   class Admin extends User {}
来源：http://vbv.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://ijt.epnwcf.com

Java: class Admin extends User {}
来源：http://opi.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vgf.yvedp.cn

Ruby: class Admin < User; end
来源：http://hby.zycfv.cn

C#:   class Admin : User {}
来源：http://edn.hfpthk.cn

[G06] 重写方法
来源：http://boj.cucudq.cn

Py:   def greet(self): return "admin"
来源：http://qsp.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jtf.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://xlg.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://asm.yangfankeji.com

Java: @Override String greet() { return "admin"; }
来源：http://blx.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bca.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://heu.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://iyw.shangyingyoupin.top

[G07] 调用父类方法
来源：http://sta.yongpay.top

Py:   super().greet()
来源：http://wwb.aizwys.cn

PHP:  parent::greet();
来源：http://lbn.guannengcc.top

JS:   super.greet();
来源：http://euo.fehbvm.com

TS:   super.greet();
来源：http://uhi.nanxuanxn.top

Java: super.greet();
来源：http://zpn.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hhx.jiagoushi.top

Ruby: super
来源：http://kft.pycfn.com

C#:   base.Greet();
来源：http://ubo.c1oappe.top

[G08] 静态方法与属性
来源：http://spe.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dpm.jqgfzy.top

PHP:  public static function f() {}
来源：http://izl.jqgfzy.top

JS:   static f() {}
来源：http://tbc.ybcxt.top

TS:   static f(): void {}
来源：http://zxo.hnxiangtu.top

Java: static void f() {}
来源：http://jwk.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bbb.mhx1999.top

Ruby: def self.f; end
来源：http://gtk.ctjpmb.com

C#:   public static void F() {}
来源：http://jhy.redwolf501.top

[G09] 接口 / 抽象类
来源：http://kue.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://dbx.jqgufenzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://rav.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://urb.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://csb.guannengcc.top

Java: interface Shape { double area(); }
来源：http://nrg.fengsongda.top

Go:   type Shape interface { Area() float64 }
来源：http://skt.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gfs.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://lmt.jqgfzy.top

[G10] 访问控制
来源：http://ggc.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://qak.bjfxy.top

PHP:  public / protected / private
来源：http://dwv.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://eiz.jyoumei.cn

TS:   public / protected / private
来源：http://zcp.nanxinkj.top

Java: public / protected / private / 默认包级
来源：http://bwk.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ihy.vehdjk.com

Ruby: public / protected / private
来源：http://uid.cqqwz.cn

C#:   public / protected / private / internal
来源：http://ocl.xylfe.cn

[G11] getter / setter
来源：http://ofb.yj20258.top

Py:   @property 与 @x.setter
来源：http://fyh.ydzc1.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nec.aizwys.cn

JS:   get name() { return this._name; }
来源：http://ncs.yj202588.top

TS:   get name(): string { return this._name; }
来源：http://qjs.yuxming.cn

Java: public String getName() { return name; }
来源：http://qgu.xingfuxueyuan.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://dyy.chenzaomai.com

Ruby: attr_accessor :name
来源：http://nwk.jinqigufen.top

C#:   public string Name { get; set; }
来源：http://cpv.fengsongda.top

[G12] 对象转字符串
来源：http://rid.hcnkem.com

Py:   def __str__(self): return self.name
来源：http://ncr.havefunace.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://drv.cashguo.top

JS:   toString() { return this.name; }
来源：http://nab.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://rxh.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://xsz.zhoulong.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://czt.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://awi.cheryme.top

C#:   public override string ToString() => Name;
来源：http://fng.hnqzz.top

[G13] 判断对象类型
来源：http://djq.yanxiufei.cn

Py:   isinstance(u, User)
来源：http://sub.andypj.xyz

PHP:  $u instanceof User
来源：http://coy.0kj1m.cn

JS:   u instanceof User
来源：http://xbi.yonumen.top

TS:   u instanceof User
来源：http://njj.andypj.xyz

Java: u instanceof User
来源：http://ets.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dpm.yueranfly.top

Ruby: u.is_a?(User)
来源：http://muk.hnqzz.top

C#:   u is User
来源：http://gkz.xingfuxueyuan.xyz

[G14] 数据类 / record
来源：http://vyh.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lif.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://sgo.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://bod.jinqigufen.top

TS:   type User = { name: string; age: number };
来源：http://jow.daxiang520.top

Java: record User(String name, int age) {}
来源：http://dpa.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://ycr.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ltn.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://nyj.xuanzx.com

[G15] 枚举
来源：http://fuy.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ggu.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lzm.zhaomingkeji.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ncg.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lwv.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://dtj.wangdashe.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vac.316326.xyz

Ruby: Color = %i[red green].freeze
来源：http://wic.ydzc1.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mdo.hcnkem.com

[G16] 对象转数组 / 字典
来源：http://cye.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zrf.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://juw.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://pgh.c1oappe.top

TS:   Object.entries(obj)
来源：http://vqe.birdmap.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sfq.dashuyun.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lyp.snrcjt.cn

Ruby: obj.instance_variables
来源：http://hhg.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://qme.aibaodan.cn

================================================================================
来源：http://ynl.jinghuilouyu.cn

H. 异常与错误处理
来源：http://sqs.jqgufenzy.top

================================================================================
来源：http://vhb.daria6918.cn

[H01] try / catch 基础
来源：http://ngf.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pmn.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qym.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://phr.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jcy.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://znr.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kck.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://okl.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ytb.yvedp.cn

[H02] finally / ensure 收尾
来源：http://csk.zdbjq.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xeb.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://ymh.shanyushiyangtech.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vqp.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ril.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ijr.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxx.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rwa.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://svm.ydjk.org.cn

[H03] 主动抛出异常
来源：http://bfg.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://itd.gaohongyu789.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lac.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://eol.andypj.xyz

TS:   throw new Error("错误信息");
来源：http://vyv.redwolf501.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aha.nanxuanxn.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ekj.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hgi.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://enc.hcnkem.com

[H04] 自定义异常类型
来源：http://veg.hammf.cn

Py:   class MyError(Exception): pass
来源：http://fcd.feifeiyinyue.top

PHP:  class MyError extends RuntimeException {}
来源：http://lje.andypj.xyz

JS:   class MyError extends Error {}
来源：http://rxe.c1oappe.top

TS:   class MyError extends Error {}
来源：http://zww.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://hdl.yonumen.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wyk.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://amh.svipenyu.cn

C#:   class MyException : Exception {}
来源：http://zcs.tian-w.cn

[H05] 捕获特定类型
来源：http://iqr.cucudq.cn

Py:   except ValueError as e:
来源：http://jpc.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dsx.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://rgr.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://axg.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://pzr.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pzj.epnwcf.com

Ruby: rescue ArgumentError => e
来源：http://hnl.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zgi.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://xfk.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://hpi.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://ded.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://kmv.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ywl.haohaochexian.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://phe.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vba.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://gye.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://edc.fehbvm.com

[H07] 断言
来源：http://aqd.yj20258.top

Py:   assert x > 0, "必须为正"
来源：http://eto.jyoumei.cn

PHP:  assert($x > 0);
来源：http://uls.pycfn.com

JS:   console.assert(x > 0);
来源：http://auv.52xcode.cn

TS:   console.assert(x > 0);
来源：http://jrm.ywan-chungtsiang.top

Java: assert x > 0 : "必须为正";
来源：http://vyx.smart0.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hca.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://abr.fktsv.cn


<!-- 参考信息 -->