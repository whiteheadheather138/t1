代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://cmn.yonumen.top

[F02] 逐行读取文件
来源：http://fli.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ekq.ctjpmb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zyq.daria6918.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cdy.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zbb.shuidangran.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qek.yfazqb.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rsn.yongpay.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ilc.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lei.meibo888.top

[F03] 写入文件（覆盖）
来源：http://byx.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://izo.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ixx.ivvv.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://txb.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vge.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rka.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cck.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://zap.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eog.zdbjq.cn

[F04] 追加写入文件
来源：http://iio.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gst.pycfn.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ihp.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mma.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lxs.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pzq.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oep.gogol.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mhs.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hit.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://yrn.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pvv.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://ccs.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://azv.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://sjg.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://atr.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jlk.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://bim.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://qaw.cashguo.top

[F06] 删除文件
来源：http://ybt.daxiang520.top

Py:   os.remove("a.txt")
来源：http://igm.daria6918.cn

PHP:  unlink("a.txt");
来源：http://olz.kuanghao11.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yyx.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://bty.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lzg.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://txb.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://spu.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://mpe.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://idn.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fno.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zmq.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ppw.zhixingplan.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zby.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhx.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hni.cucudq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vtt.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bvi.ybcxt.top

[F08] 遍历目录
来源：http://seu.yvedp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vvq.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aoq.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://jru.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://stp.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xfo.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xrq.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://vxa.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://xld.c1oappe.top

[F09] 获取文件大小
来源：http://ooo.havefunace.top

Py:   os.path.getsize("a.txt")
来源：http://rkd.andypj.xyz

PHP:  filesize("a.txt");
来源：http://mby.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://ijh.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://rmj.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gnv.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yzc.tanke756.top

Ruby: File.size("a.txt")
来源：http://uys.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://pye.xylfe.cn

[F10] 取文件扩展名 / 文件名
来源：http://ihb.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nau.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uev.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cla.sysykeji.top

TS:   path.extname("a.txt")
来源：http://qtp.cashguo.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://whl.zhixingplan.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ylb.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uvu.hammf.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nub.shuidangran.top

[F11] 复制与移动文件
来源：http://tiu.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tnq.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bhi.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xei.hongshengwenyu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jat.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dor.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://thx.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rag.gzhubu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccr.9152youxi.cn

[F12] CSV 读写
来源：http://rfc.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ufp.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://odt.nwbrower.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iaz.zhongyouzk.top

TS:   // 同上
来源：http://idv.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eye.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fbj.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fjz.tanke756.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xln.hysaishi.cn

================================================================================
来源：http://zze.yongpay.top

G. 面向对象
来源：http://bpi.iojbl.cn

================================================================================
来源：http://rqj.hnxiangtu.top

[G01] 定义类
来源：http://eku.nanxuanxn.top

Py:   class User: pass
来源：http://woa.nwbrower.top

PHP:  class User {}
来源：http://ywe.aizwys.cn

JS:   class User {}
来源：http://arv.tanke756.top

TS:   class User { name: string = ""; }
来源：http://kax.zdbjq.cn

Java: class User {}
来源：http://ryq.birdmap.top

Go:   type User struct { Name string }
来源：http://ojr.nwbrower.top

Ruby: class User; end
来源：http://ndc.sweek.top

C#:   class User {}
来源：http://znb.jinqigfzy.top

[G02] 构造函数
来源：http://zqe.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://krx.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://xqc.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://zpc.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://juo.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://zck.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://svy.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://ese.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://osf.hnqzz.top

[G03] 实例属性
来源：http://umq.jinqigufen.top

Py:   self.name = "x"
来源：http://rqj.redwolf501.top

PHP:  public string $name = "x";
来源：http://kog.yuanzhike.top

JS:   this.name = "x";
来源：http://dlq.hywenlv.cn

TS:   name: string = "x";
来源：http://ldr.yfazqb.com

Java: private String name;
来源：http://lqf.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cgn.pycfn.com

Ruby: @name = "x"
来源：http://ico.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://efw.yvedp.cn

[G04] 定义方法
来源：http://xxe.guannengcc.top

Py:   def greet(self): return self.name
来源：http://ghw.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://yho.wangshuangyany.cn

JS:   greet() { return this.name; }
来源：http://yey.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://erz.hnxiangtu.top

Java: String greet() { return name; }
来源：http://twc.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vrr.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://qmz.yj20258888.top

C#:   public string Greet() => Name;
来源：http://sdu.hnqzz.top

[G05] 继承
来源：http://snd.iojbl.cn

Py:   class Admin(User): pass
来源：http://jdz.zycfv.cn

PHP:  class Admin extends User {}
来源：http://nbv.cdnleiting.top

JS:   class Admin extends User {}
来源：http://vhb.sysykeji.top

TS:   class Admin extends User {}
来源：http://nrd.sysykeji.top

Java: class Admin extends User {}
来源：http://hjq.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxp.jianghu66.top

Ruby: class Admin < User; end
来源：http://ptj.gaohongyu789.top

C#:   class Admin : User {}
来源：http://kpt.chenzaomai.com

[G06] 重写方法
来源：http://gpu.cheryme.top

Py:   def greet(self): return "admin"
来源：http://glh.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://npr.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://qhe.hfpthk.cn

TS:   greet(): string { return "admin"; }
来源：http://eif.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://itc.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fjt.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://mme.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://kym.tian-w.cn

[G07] 调用父类方法
来源：http://liv.dianchejie.cn

Py:   super().greet()
来源：http://mds.hongshengwenyu.top

PHP:  parent::greet();
来源：http://hsb.jyoumei.cn

JS:   super.greet();
来源：http://lbl.yonumen.top

TS:   super.greet();
来源：http://ikn.havefunace.top

Java: super.greet();
来源：http://yur.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zeu.shangyingyoupin.top

Ruby: super
来源：http://xgs.shanyushiyangtech.top

C#:   base.Greet();
来源：http://pdb.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://bno.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://smz.zhijiandao.cn

PHP:  public static function f() {}
来源：http://cdj.ivvv.top

JS:   static f() {}
来源：http://lot.yj202588.top

TS:   static f(): void {}
来源：http://qdz.jyoumei.cn

Java: static void f() {}
来源：http://zgm.iojbl.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bug.andypj.xyz

Ruby: def self.f; end
来源：http://xzi.haohaochexian.top

C#:   public static void F() {}
来源：http://hpt.jianghu66.top

[G09] 接口 / 抽象类
来源：http://wzc.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://evs.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://vws.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hqt.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://aou.fengsongda.top

Java: interface Shape { double area(); }
来源：http://isl.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://xub.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qcz.vehdjk.com

C#:   interface IShape { double Area(); }
来源：http://hzj.gzhubu.top

[G10] 访问控制
来源：http://ian.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://tyh.jqgufenzy.top

PHP:  public / protected / private
来源：http://irj.jinqigufen.top

JS:   #private 字段；其余公开
来源：http://azm.yangfankeji.com

TS:   public / protected / private
来源：http://fog.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://wmp.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zdf.zdbjq.cn

Ruby: public / protected / private
来源：http://whi.nanxinkj.top

C#:   public / protected / private / internal
来源：http://zuf.fktsv.cn

[G11] getter / setter
来源：http://pnt.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://wbz.svipenyu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://soy.xuanzx.com

JS:   get name() { return this._name; }
来源：http://yhi.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://udw.chenzaomai.com

Java: public String getName() { return name; }
来源：http://ejn.tian-w.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eeu.yangfankeji.com

Ruby: attr_accessor :name
来源：http://iwq.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://hko.sweek.top

[G12] 对象转字符串
来源：http://muj.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://ade.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ohi.wangdashe.top

JS:   toString() { return this.name; }
来源：http://bxm.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://kic.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://svf.hcnkem.com

Go:   func (u User) String() string { return u.Name }
来源：http://dsb.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://ykm.aizwys.cn

C#:   public override string ToString() => Name;
来源：http://unz.hesvh.cn

[G13] 判断对象类型
来源：http://qkh.hcnkem.com

Py:   isinstance(u, User)
来源：http://gbn.tarul.cn

PHP:  $u instanceof User
来源：http://rkf.svipenyu.cn

JS:   u instanceof User
来源：http://rke.vqdsnc.cn

TS:   u instanceof User
来源：http://eci.zhaomingkeji.xyz

Java: u instanceof User
来源：http://xle.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zfa.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://bib.jyoumei.cn

C#:   u is User
来源：http://bom.jqgfzy.top

[G14] 数据类 / record
来源：http://gvx.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://auz.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://jvz.redwolf501.top

JS:   // 无内置：普通类或对象字面量
来源：http://xud.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://abl.bbcook.cn

Java: record User(String name, int age) {}
来源：http://uwu.fehbvm.com

Go:   type User struct { Name string; Age int }
来源：http://jzw.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fxl.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://xwj.birdmap.top

[G15] 枚举
来源：http://aeo.yonumen.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tpg.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://jze.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iiq.gotoacloud.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qpx.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://bbd.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vuv.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://isu.nwbrower.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://buk.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://ktv.birdmap.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://doj.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://dzk.birdmap.top

JS:   Object.entries(obj)
来源：http://nbg.aibaodan.cn

TS:   Object.entries(obj)
来源：http://rqz.redwolf501.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://phf.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dnx.yueranfly.top

Ruby: obj.instance_variables
来源：http://wju.jyoumei.cn

C#:   // 用反射或 System.Text.Json
来源：http://bap.yj20258888.top

================================================================================
来源：http://nvk.hesvh.cn

H. 异常与错误处理
来源：http://bti.jiagoushi.top

================================================================================
来源：http://zpk.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://cvw.haohaochexian.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ymi.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fbl.jinghuilouyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vii.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://opu.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pct.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bjr.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://crq.sysykeji.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mxy.ydjk.org.cn

[H02] finally / ensure 收尾
来源：http://vzb.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://oqv.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sxu.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eli.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://htx.nwbrower.top

Java: try { f(); } finally { cleanup(); }
来源：http://ccx.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://xsg.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pwt.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tau.yvedp.cn

[H03] 主动抛出异常
来源：http://gai.cashguo.top

Py:   raise ValueError("错误信息")
来源：http://hpn.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qxr.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://opl.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://zvy.xylfe.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tpv.feifeiyinyue.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mnq.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://icr.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://pyy.sweek.top

[H04] 自定义异常类型
来源：http://jbj.gzhubu.top

Py:   class MyError(Exception): pass
来源：http://ios.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yqb.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://qvw.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://dlh.tian-w.cn

Java: class MyException extends RuntimeException {}
来源：http://tro.hysaishi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ahs.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://zjx.ydzc1.top

C#:   class MyException : Exception {}
来源：http://oaz.jiagoushi.top

[H05] 捕获特定类型
来源：http://cxm.guowangkeji.top

Py:   except ValueError as e:
来源：http://cno.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfx.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://cmn.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://bim.ywan-chungtsiang.top

Java: catch (IOException | SQLException e) {}
来源：http://ors.smart0.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zzb.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://tdi.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fth.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://oht.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://fkp.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://pba.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://aex.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://cfa.zhaomingkeji.xyz


<!-- 参考信息 -->