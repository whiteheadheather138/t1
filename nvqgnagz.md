代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ylu.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vwe.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjo.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gmv.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://upl.iojbl.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gnm.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oyp.zhengqikj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wkq.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://mwp.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yzg.yongpay.top

PHP:  file_exists("a.txt");
来源：http://xog.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://wrf.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://jlz.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vjt.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bvl.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://qbb.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://top.xuetiantiany.cn

[F06] 删除文件
来源：http://pix.epnwcf.com

Py:   os.remove("a.txt")
来源：http://qjv.yueranfly.top

PHP:  unlink("a.txt");
来源：http://xwi.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://mqg.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dqe.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oau.tian-w.cn

Go:   os.Remove("a.txt")
来源：http://jsp.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://wuv.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://zph.feifeiyinyue.top

[F07] 创建目录（含多级）
来源：http://trc.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfq.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://has.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dlc.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxm.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xre.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rtw.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kyj.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fgf.wangshuangyany.cn

[F08] 遍历目录
来源：http://yvb.yangfankeji.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://uoc.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eeg.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://nys.chenjidiqi.icu

TS:   fs.readdirSync("dir")
来源：http://zvi.0kj1m.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cok.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ptx.feifeiyinyue.top

Ruby: Dir.children("dir")
来源：http://nou.haohaochexian.top

C#:   Directory.GetFiles("dir")
来源：http://jkj.daxiang520.top

[F09] 获取文件大小
来源：http://qcs.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://hth.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://jkg.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://nya.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://tus.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://phs.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://poq.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://xba.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://yoz.yuxming.cn

[F10] 取文件扩展名 / 文件名
来源：http://zhn.hfpthk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gyo.jinqigfzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mhl.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://erh.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://xtk.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fzg.tian-w.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tyo.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ljl.52xcode.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pjt.zhixingplan.top

[F11] 复制与移动文件
来源：http://olg.hysaishi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bpb.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vxo.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://haj.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sns.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sol.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wdo.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hay.ywan-chungtsiang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ixo.hesvh.cn

[F12] CSV 读写
来源：http://nuv.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qtp.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mzi.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqi.cheryme.top

TS:   // 同上
来源：http://epr.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jsw.52xcode.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jah.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nbj.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nrb.shangyingyoupin.top

================================================================================
来源：http://mfn.ehwqpu.com

G. 面向对象
来源：http://jyg.cashguo.top

================================================================================
来源：http://ufa.ydjk.org.cn

[G01] 定义类
来源：http://ruo.c1oappe.top

Py:   class User: pass
来源：http://ocu.yj20258.top

PHP:  class User {}
来源：http://bep.snrcjt.cn

JS:   class User {}
来源：http://ocd.fzhhl.top

TS:   class User { name: string = ""; }
来源：http://kyt.ivvv.top

Java: class User {}
来源：http://wvu.yangfankeji.com

Go:   type User struct { Name string }
来源：http://wzj.kuanghao11.cn

Ruby: class User; end
来源：http://hse.sxryk.cn

C#:   class User {}
来源：http://fpo.andypj.xyz

[G02] 构造函数
来源：http://zlh.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://gbl.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://vev.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://pti.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://led.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://fzs.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wkv.yuanzhike.top

Ruby: def initialize(name); @name = name; end
来源：http://def.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://xhr.nanxinkj.top

[G03] 实例属性
来源：http://qde.jqgufenzy.top

Py:   self.name = "x"
来源：http://gch.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://jmy.aibaodan.cn

JS:   this.name = "x";
来源：http://hsz.ehwqpu.com

TS:   name: string = "x";
来源：http://igf.zdqjudy.top

Java: private String name;
来源：http://dzf.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://icf.haohaochexian.top

Ruby: @name = "x"
来源：http://izw.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://axk.xinyue.icu

[G04] 定义方法
来源：http://bls.fengsongda.top

Py:   def greet(self): return self.name
来源：http://miw.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://srk.gzhubu.top

JS:   greet() { return this.name; }
来源：http://tbo.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://hle.zhixingplan.top

Java: String greet() { return name; }
来源：http://qtb.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kcj.xylfe.cn

Ruby: def greet; @name; end
来源：http://lwl.yfazqb.com

C#:   public string Greet() => Name;
来源：http://stc.andypj.xyz

[G05] 继承
来源：http://uln.daxiang520.top

Py:   class Admin(User): pass
来源：http://fzk.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://mti.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://waj.fzhhl.top

TS:   class Admin extends User {}
来源：http://iit.c1oappe.top

Java: class Admin extends User {}
来源：http://pyv.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oef.hesvh.cn

Ruby: class Admin < User; end
来源：http://wcs.dashuyun.cn

C#:   class Admin : User {}
来源：http://hym.hfpthk.cn

[G06] 重写方法
来源：http://aff.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://mou.iojbl.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://irz.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://rjt.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://atw.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://fpd.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jkm.xinyue.icu

Ruby: def greet; "admin"; end
来源：http://iqj.ctjpmb.com

C#:   public override string Greet() => "admin";
来源：http://gjl.fengsongda.top

[G07] 调用父类方法
来源：http://jxh.ehwqpu.com

Py:   super().greet()
来源：http://mva.jqgfzy.top

PHP:  parent::greet();
来源：http://nku.sweek.top

JS:   super.greet();
来源：http://qbf.guannengcc.top

TS:   super.greet();
来源：http://wsh.pengpengdd.cyou

Java: super.greet();
来源：http://rca.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hro.xylfe.cn

Ruby: super
来源：http://sqr.hysaishi.cn

C#:   base.Greet();
来源：http://cqj.jiagoushi.top

[G08] 静态方法与属性
来源：http://tas.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hgn.svipenyu.cn

PHP:  public static function f() {}
来源：http://gyb.jinqigufen.top

JS:   static f() {}
来源：http://dkw.pycfn.com

TS:   static f(): void {}
来源：http://yyp.yj20258888.top

Java: static void f() {}
来源：http://rav.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kat.jlsjyb.cn

Ruby: def self.f; end
来源：http://muk.aizwys.cn

C#:   public static void F() {}
来源：http://grz.vehdjk.com

[G09] 接口 / 抽象类
来源：http://aqr.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://etk.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://buf.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://okg.yj202588.top

TS:   interface Shape { area(): number; }
来源：http://jxv.mhx1999.top

Java: interface Shape { double area(); }
来源：http://twu.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://aye.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tko.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://rgs.jianghu66.top

[G10] 访问控制
来源：http://vqx.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://anq.yj202588.top

PHP:  public / protected / private
来源：http://pzz.hcnkem.com

JS:   #private 字段；其余公开
来源：http://xjt.fktsv.cn

TS:   public / protected / private
来源：http://ntm.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://aal.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ctx.ywan-chungtsiang.top

Ruby: public / protected / private
来源：http://zkx.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://ung.gogol.net.cn

[G11] getter / setter
来源：http://ggp.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://dej.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wuj.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://qli.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://ltd.birdmap.top

Java: public String getName() { return name; }
来源：http://den.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://mpw.ctjpmb.com

Ruby: attr_accessor :name
来源：http://awi.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://uuw.dashuyun.cn

[G12] 对象转字符串
来源：http://ydw.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://svi.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://auc.iojbl.cn

JS:   toString() { return this.name; }
来源：http://ocu.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://kdu.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://mla.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://adq.gzhubu.top

Ruby: def to_s; @name; end
来源：http://vpn.daxiang520.top

C#:   public override string ToString() => Name;
来源：http://run.yonumen.top

[G13] 判断对象类型
来源：http://nyh.jinqigufen.top

Py:   isinstance(u, User)
来源：http://tev.yangfankeji.com

PHP:  $u instanceof User
来源：http://ele.zhixingplan.top

JS:   u instanceof User
来源：http://pic.redwolf501.top

TS:   u instanceof User
来源：http://pxx.bjfxy.top

Java: u instanceof User
来源：http://xlb.pengpengdd.cyou

Go:   u, ok := v.(User)            // 类型断言
来源：http://ted.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://wpa.gaohongyu789.top

C#:   u is User
来源：http://fac.jyoumei.cn

[G14] 数据类 / record
来源：http://mdd.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wde.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://eoy.tianlin.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ktp.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://zii.fktsv.cn

Java: record User(String name, int age) {}
来源：http://ods.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://joo.quarkkingdee.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jry.fktsv.cn

C#:   record User(string Name, int Age);
来源：http://bsb.shuidangran.top

[G15] 枚举
来源：http://rsv.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://miq.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rhj.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vzf.guowangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lok.wangshuangyany.cn

Java: enum Color { RED, GREEN }
来源：http://wri.yonumen.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nne.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://dsa.ivvv.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://syu.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://jdb.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pya.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://zfz.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://usb.jianghu66.top

TS:   Object.entries(obj)
来源：http://jxg.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kqf.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://rbe.0kj1m.cn

Ruby: obj.instance_variables
来源：http://egf.quarkkingdee.top

C#:   // 用反射或 System.Text.Json
来源：http://pzs.ivvv.top

================================================================================
来源：http://tti.andypj.xyz

H. 异常与错误处理
来源：http://hty.jlsjyb.cn

================================================================================
来源：http://mcu.vehdjk.com

[H01] try / catch 基础
来源：http://fjm.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gai.yj202588.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ltb.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fzl.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://czn.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vch.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kvq.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ivz.yanxiufei.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kxx.birdmap.top

[H02] finally / ensure 收尾
来源：http://pfz.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zxy.redwolf501.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hhr.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bap.nwbrower.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wfc.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oxo.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rtp.feifeiyinyue.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nxc.gzhubu.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://nsz.yongpay.top

[H03] 主动抛出异常
来源：http://mts.ydjk.org.cn

Py:   raise ValueError("错误信息")
来源：http://bdk.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zip.316326.xyz

JS:   throw new Error("错误信息");
来源：http://fqc.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://yze.zycfv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lbd.iojbl.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://amt.cdnleiting.top

Ruby: raise ArgumentError, "错误信息"
来源：http://acy.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://esx.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://ezo.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://mrt.dianchejie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jik.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://mwr.ybcxt.top

TS:   class MyError extends Error {}
来源：http://ond.pengpengdd.cyou

Java: class MyException extends RuntimeException {}
来源：http://sbg.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qhr.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://ndv.sweek.top

C#:   class MyException : Exception {}
来源：http://xdx.xylfe.cn

[H05] 捕获特定类型
来源：http://geb.ybcxt.top

Py:   except ValueError as e:
来源：http://wyu.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ikt.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://uss.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wtp.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://cwg.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wsq.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://wgx.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xwl.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://nrd.vqdsnc.cn

Py:   value = d.get("k") or default
来源：http://xea.meibo888.top

PHP:  $v = $d["k"] ?? null;
来源：http://bhw.uphjek.com

JS:   obj?.a?.b;  d ?? default
来源：http://rwx.dianchejie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qdo.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://axt.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wtq.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://zdw.wangdashe.top

C#:   obj?.A?.B ?? default
来源：http://agh.9152youxi.cn

[H07] 断言
来源：http://qti.316326.xyz

Py:   assert x > 0, "必须为正"
来源：http://lgu.xinyue.icu

PHP:  assert($x > 0);
来源：http://oek.fengsongda.top

JS:   console.assert(x > 0);
来源：http://rre.aizwys.cn

TS:   console.assert(x > 0);
来源：http://bfc.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://fba.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ugq.iojbl.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gfp.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://iqz.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://gss.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://uju.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zpb.jyoumei.cn

JS:   e.message;  e.stack
来源：http://odp.jinqigufen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tuu.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sdk.cdnleiting.top

Go:   err.Error()
来源：http://mvv.pengpengdd.cyou


<!-- 参考信息 -->