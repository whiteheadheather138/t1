代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uav.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ibr.zhoulong.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ioe.sjlbkw.cn

[F04] 追加写入文件
来源：http://onu.jinqigufen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://doy.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gmn.guowangkeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xgi.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbe.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mkj.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wta.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://way.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eng.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://xxe.redwolf501.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ekp.hesvh.cn

PHP:  file_exists("a.txt");
来源：http://ias.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://tnq.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://chh.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zku.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ipw.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://uqo.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://fqp.fktsv.cn

[F06] 删除文件
来源：http://krw.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://lji.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://ccm.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://rxk.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://afc.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xju.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://dsk.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://tqg.pycfn.com

C#:   File.Delete("a.txt");
来源：http://jky.yuxming.cn

[F07] 创建目录（含多级）
来源：http://xud.bjfxy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xyi.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qbr.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ryk.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stn.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nfb.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qob.cqqwz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pgv.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jmu.smart0.xyz

[F08] 遍历目录
来源：http://ung.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://rfv.shuidangran.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tvs.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://fjw.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://idy.chenzaomai.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kbx.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://znu.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://amy.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://nli.hnxiangtu.top

[F09] 获取文件大小
来源：http://kxc.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://buw.xinyue.icu

PHP:  filesize("a.txt");
来源：http://bac.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://cmy.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://dju.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://fgd.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wpp.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://sqf.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://rpo.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://lyx.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tis.nanxuanxn.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://adf.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zkt.fktsv.cn

TS:   path.extname("a.txt")
来源：http://ffe.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://edr.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pvm.jqgufenzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://til.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zka.ybcxt.top

[F11] 复制与移动文件
来源：http://goe.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wum.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rmx.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eny.pengpengdd.cyou

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oeg.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aow.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vfj.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sbv.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ton.ctjpmb.com

[F12] CSV 读写
来源：http://ity.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fow.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mzm.zhoulong.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://czg.9152youxi.cn

TS:   // 同上
来源：http://mxn.tarul.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rte.hnqzz.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sdf.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://awq.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nfs.zdbjq.cn

================================================================================
来源：http://fmd.yj202588.top

G. 面向对象
来源：http://vpr.aizwys.cn

================================================================================
来源：http://mtp.fanxiaobao.xyz

[G01] 定义类
来源：http://ozp.nanxuanxn.top

Py:   class User: pass
来源：http://sbc.jinyuanbaomall.cn

PHP:  class User {}
来源：http://uhx.xylfe.cn

JS:   class User {}
来源：http://evi.birdmap.top

TS:   class User { name: string = ""; }
来源：http://eae.hesvh.cn

Java: class User {}
来源：http://iah.guowangkeji.top

Go:   type User struct { Name string }
来源：http://tfq.zdbjq.cn

Ruby: class User; end
来源：http://irg.birdmap.top

C#:   class User {}
来源：http://ajg.chenzaomai.com

[G02] 构造函数
来源：http://gxu.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://gwe.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://qfb.ehwqpu.com

JS:   constructor(name) { this.name = name; }
来源：http://qox.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://vbb.cucudq.cn

Java: User(String name) { this.name = name; }
来源：http://btv.hywenlv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pjp.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://oxn.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://rxe.yonumen.top

[G03] 实例属性
来源：http://wip.zhengqikj.top

Py:   self.name = "x"
来源：http://znr.sysykeji.top

PHP:  public string $name = "x";
来源：http://sft.chenjidiqi.icu

JS:   this.name = "x";
来源：http://ler.gzhubu.top

TS:   name: string = "x";
来源：http://swr.yvedp.cn

Java: private String name;
来源：http://ykq.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dwp.nanxuanxn.top

Ruby: @name = "x"
来源：http://shx.zycfv.cn

C#:   public string Name { get; set; } = "x";
来源：http://mqf.hywenlv.cn

[G04] 定义方法
来源：http://wuu.ydzc1.top

Py:   def greet(self): return self.name
来源：http://ngv.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://kca.aizwys.cn

JS:   greet() { return this.name; }
来源：http://iii.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://gjj.ehwqpu.com

Java: String greet() { return name; }
来源：http://eyh.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://njp.redwolf501.top

Ruby: def greet; @name; end
来源：http://oxh.hcnkem.com

C#:   public string Greet() => Name;
来源：http://onx.hnxiangtu.top

[G05] 继承
来源：http://wgh.chenzaomai.com

Py:   class Admin(User): pass
来源：http://gug.tanke756.top

PHP:  class Admin extends User {}
来源：http://tzb.c1oappe.top

JS:   class Admin extends User {}
来源：http://rej.zdbjq.cn

TS:   class Admin extends User {}
来源：http://mii.iojbl.cn

Java: class Admin extends User {}
来源：http://edk.tanke756.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hcy.sxryk.cn

Ruby: class Admin < User; end
来源：http://dbw.yangfankeji.com

C#:   class Admin : User {}
来源：http://uni.hongshengwenyu.top

[G06] 重写方法
来源：http://uls.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://kls.sxryk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ues.yueranfly.top

JS:   greet() { return "admin"; }
来源：http://dob.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://boi.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://nye.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fqy.nanxinkj.top

Ruby: def greet; "admin"; end
来源：http://xmw.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://wcc.nanxinkj.top

[G07] 调用父类方法
来源：http://gnp.mhx1999.top

Py:   super().greet()
来源：http://kpz.wangdashe.top

PHP:  parent::greet();
来源：http://bcl.fzhhl.top

JS:   super.greet();
来源：http://loy.nanxinkj.top

TS:   super.greet();
来源：http://jwu.hysaishi.cn

Java: super.greet();
来源：http://vln.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mou.cucudq.cn

Ruby: super
来源：http://dgu.chenjidiqi.icu

C#:   base.Greet();
来源：http://uko.uphjek.com

[G08] 静态方法与属性
来源：http://rar.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lwo.haohaochexian.top

PHP:  public static function f() {}
来源：http://zoo.shuidangran.top

JS:   static f() {}
来源：http://rfk.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://uwt.ctjpmb.com

Java: static void f() {}
来源：http://dek.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://jmt.jyoumei.cn

Ruby: def self.f; end
来源：http://ygf.ywan-chungtsiang.top

C#:   public static void F() {}
来源：http://hnj.cucudq.cn

[G09] 接口 / 抽象类
来源：http://thr.hfpthk.cn

Py:   from abc import ABC, abstractmethod
来源：http://rpj.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zhp.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uou.tian-w.cn

TS:   interface Shape { area(): number; }
来源：http://aqp.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://ktd.sufxvd.cn

Go:   type Shape interface { Area() float64 }
来源：http://vcx.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://awz.sweek.top

C#:   interface IShape { double Area(); }
来源：http://nbu.0kj1m.cn

[G10] 访问控制
来源：http://acm.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://iwe.zhongyouzk.top

PHP:  public / protected / private
来源：http://pyu.yonumen.top

JS:   #private 字段；其余公开
来源：http://hlw.cashguo.top

TS:   public / protected / private
来源：http://sfh.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://wrx.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zwx.quarkkingdee.top

Ruby: public / protected / private
来源：http://oll.xingfuxueyuan.xyz

C#:   public / protected / private / internal
来源：http://lqr.yj20258.top

[G11] getter / setter
来源：http://cyc.sxryk.cn

Py:   @property 与 @x.setter
来源：http://iuv.vqdsnc.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bmb.pengpengdd.cyou

JS:   get name() { return this._name; }
来源：http://hyn.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://lfe.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://txq.fengsongda.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rym.iojbl.cn

Ruby: attr_accessor :name
来源：http://aty.ydzc1.top

C#:   public string Name { get; set; }
来源：http://bdq.shzxlz.cn

[G12] 对象转字符串
来源：http://txl.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://imi.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kgo.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://frz.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://ijg.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://bpg.tianlin.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://dpn.sufxvd.cn

Ruby: def to_s; @name; end
来源：http://lqh.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://nrr.52xcode.cn

[G13] 判断对象类型
来源：http://rdj.vehdjk.com

Py:   isinstance(u, User)
来源：http://pfr.nwbrower.top

PHP:  $u instanceof User
来源：http://tmq.hnxiangtu.top

JS:   u instanceof User
来源：http://sqx.tianlin.xyz

TS:   u instanceof User
来源：http://olh.yfazqb.com

Java: u instanceof User
来源：http://gjm.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nlt.fktsv.cn

Ruby: u.is_a?(User)
来源：http://zin.hammf.cn

C#:   u is User
来源：http://rzk.yanxiufei.cn

[G14] 数据类 / record
来源：http://reu.jinqigfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ktr.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://yly.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://zkp.c1oappe.top

TS:   type User = { name: string; age: number };
来源：http://tub.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://fwv.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://mpf.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xiw.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://wpe.xziqi.cn

[G15] 枚举
来源：http://egn.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rio.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yqn.jinqigufen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dov.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://imo.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://auh.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hpt.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://pad.daria6918.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suw.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://uxn.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hhn.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://prr.yuxming.cn

JS:   Object.entries(obj)
来源：http://vvx.fzhhl.top

TS:   Object.entries(obj)
来源：http://gjl.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wrf.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ars.zhengqikj.top

Ruby: obj.instance_variables
来源：http://tse.hesvh.cn

C#:   // 用反射或 System.Text.Json
来源：http://uwy.0kj1m.cn

================================================================================
来源：http://axk.pycfn.com

H. 异常与错误处理
来源：http://ppf.ydjk.org.cn

================================================================================
来源：http://ror.nwbrower.top

[H01] try / catch 基础
来源：http://psg.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gqo.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bxr.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tvg.uphjek.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eii.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nen.cheryme.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ofb.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lwc.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dsq.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://ewa.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://wju.jlsjyb.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://igr.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://jns.sweek.top

TS:   try { f(); } finally { cleanup(); }
来源：http://oiw.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://qut.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iqa.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://euo.ppjwa.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uso.jianghu66.top

[H03] 主动抛出异常
来源：http://nwb.yonumen.top

Py:   raise ValueError("错误信息")
来源：http://iyd.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ejj.cheryme.top

JS:   throw new Error("错误信息");
来源：http://dfv.xuanzx.com

TS:   throw new Error("错误信息");
来源：http://luo.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zzz.snrcjt.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oey.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ezz.havefunace.top

C#:   throw new ArgumentException("错误信息");
来源：http://xyy.gzhubu.top

[H04] 自定义异常类型
来源：http://dpy.zhoulong.xyz

Py:   class MyError(Exception): pass
来源：http://nto.pengpengdd.cyou

PHP:  class MyError extends RuntimeException {}
来源：http://cvv.nwbrower.top

JS:   class MyError extends Error {}
来源：http://thh.snrcjt.cn

TS:   class MyError extends Error {}
来源：http://pil.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://rxj.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vfx.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://nyo.ydzc1.top

C#:   class MyException : Exception {}
来源：http://oqh.gotoacloud.top

[H05] 捕获特定类型
来源：http://afh.bbcook.cn

Py:   except ValueError as e:
来源：http://bvm.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bjg.pengpengdd.cyou

JS:   if (e instanceof TypeError) {}
来源：http://xsl.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://tmr.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://qdc.yuxming.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mkj.guowangkeji.top

Ruby: rescue ArgumentError => e
来源：http://mjm.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rvx.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://rct.havefunace.top

Py:   value = d.get("k") or default
来源：http://awk.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kbg.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ejo.xuanzx.com

TS:   obj?.a?.b;  d ?? default
来源：http://szu.yj202588.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://asx.yueranfly.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fax.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://yue.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://mex.sufxvd.cn

[H07] 断言
来源：http://knb.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://flu.jianghu66.top

PHP:  assert($x > 0);
来源：http://grw.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://ycq.guannengcc.top

TS:   console.assert(x > 0);
来源：http://blx.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://uwo.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hqr.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://ojj.zhixingplan.top

C#:   Debug.Assert(x > 0);
来源：http://vbi.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://hnr.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://wjd.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vjy.zhiwuduotai.top


<!-- 参考信息 -->