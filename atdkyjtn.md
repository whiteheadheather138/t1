代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://xwd.shuidangran.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ssj.ehwqpu.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gvj.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hfd.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pnj.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://rjn.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cle.zycfv.cn

[F04] 追加写入文件
来源：http://ccv.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vmn.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ene.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfp.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gok.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kcj.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vbw.hnqzz.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dcv.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vuh.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://cvd.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blx.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://scm.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://gbg.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://gdf.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hwz.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://djk.jinghuilouyu.cn

Ruby: File.exist?("a.txt")
来源：http://zmt.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://haj.52xcode.cn

[F06] 删除文件
来源：http://ywe.smart0.xyz

Py:   os.remove("a.txt")
来源：http://yqx.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://ywl.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://rbc.aizwys.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yif.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://loj.wangdashe.top

Go:   os.Remove("a.txt")
来源：http://eod.yongpay.top

Ruby: File.delete("a.txt")
来源：http://dbu.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://ysm.guannengcc.top

[F07] 创建目录（含多级）
来源：http://dyb.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ist.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tmb.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rdf.dianchejie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://prk.wangdashe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lgs.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mja.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qfz.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://orr.jqgfzy.top

[F08] 遍历目录
来源：http://lxw.xuetiantiany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bxs.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ivu.dashuyun.cn

JS:   fs.readdirSync("dir")
来源：http://htx.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://xap.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cov.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ekk.hesvh.cn

Ruby: Dir.children("dir")
来源：http://ynz.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://sly.ydjk.org.cn

[F09] 获取文件大小
来源：http://ztt.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://bqx.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://xvd.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://nxs.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://pzl.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://uyi.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tkd.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://nrm.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://bwn.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://its.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rid.shuidangran.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwa.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ynb.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://une.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lbh.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xjd.pengpengdd.cyou

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ewb.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://spy.yuxming.cn

[F11] 复制与移动文件
来源：http://gpk.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zlk.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jxo.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wef.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lmz.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://luv.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://buu.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipc.yuxming.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dtl.yj20258.top

[F12] CSV 读写
来源：http://aoi.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wyl.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ajp.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hoy.yangfankeji.com

TS:   // 同上
来源：http://twe.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qjg.dashuyun.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jtb.wangshuangyany.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rvl.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lym.pengpengdd.cyou

================================================================================
来源：http://rgs.yongpay.top

G. 面向对象
来源：http://oub.wangshuangyany.cn

================================================================================
来源：http://hrd.shanyushiyangtech.top

[G01] 定义类
来源：http://nov.shangyingyoupin.top

Py:   class User: pass
来源：http://ywi.shzxlz.cn

PHP:  class User {}
来源：http://foj.uphjek.com

JS:   class User {}
来源：http://xvq.guannengcc.top

TS:   class User { name: string = ""; }
来源：http://kya.tian-w.cn

Java: class User {}
来源：http://bpg.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://srj.pycfn.com

Ruby: class User; end
来源：http://piu.havefunace.top

C#:   class User {}
来源：http://ttc.bbcook.cn

[G02] 构造函数
来源：http://dcc.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://flc.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://aeq.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://zov.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://xvy.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://xxn.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ebp.yj20258888.top

Ruby: def initialize(name); @name = name; end
来源：http://tyc.chenlongwang.top

C#:   public User(string name) { Name = name; }
来源：http://tmq.yanxiufei.cn

[G03] 实例属性
来源：http://ggt.haohaochexian.top

Py:   self.name = "x"
来源：http://etm.nwbrower.top

PHP:  public string $name = "x";
来源：http://hhl.sweek.top

JS:   this.name = "x";
来源：http://ejx.fehbvm.com

TS:   name: string = "x";
来源：http://kfj.yj202588.top

Java: private String name;
来源：http://rxw.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yqh.birdmap.top

Ruby: @name = "x"
来源：http://igl.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xgu.fehbvm.com

[G04] 定义方法
来源：http://ssz.hesvh.cn

Py:   def greet(self): return self.name
来源：http://kpj.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://oyw.sweek.top

JS:   greet() { return this.name; }
来源：http://fjd.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://bgn.aibaodan.cn

Java: String greet() { return name; }
来源：http://hfa.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kmc.nanxinkj.top

Ruby: def greet; @name; end
来源：http://xzl.ybcxt.top

C#:   public string Greet() => Name;
来源：http://ido.havefunace.top

[G05] 继承
来源：http://mvn.yfazqb.com

Py:   class Admin(User): pass
来源：http://sfa.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://lvj.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://djc.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://vbx.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://cms.hongshengwenyu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zny.sxryk.cn

Ruby: class Admin < User; end
来源：http://wrp.yfazqb.com

C#:   class Admin : User {}
来源：http://bcb.bjfxy.top

[G06] 重写方法
来源：http://pju.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://bky.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zol.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://jnl.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://hnn.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://ium.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yfg.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://lxs.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://yhl.vqdsnc.cn

[G07] 调用父类方法
来源：http://viq.havefunace.top

Py:   super().greet()
来源：http://hjs.zdqjudy.top

PHP:  parent::greet();
来源：http://bsz.sufxvd.cn

JS:   super.greet();
来源：http://jtd.sweek.top

TS:   super.greet();
来源：http://cyq.ehwqpu.com

Java: super.greet();
来源：http://qsy.aizwys.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://foa.zhaomingkeji.xyz

Ruby: super
来源：http://ciw.jinqigfzy.top

C#:   base.Greet();
来源：http://xwc.bjfxy.top

[G08] 静态方法与属性
来源：http://lck.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zuu.gaohongyu789.top

PHP:  public static function f() {}
来源：http://bok.yj20258.top

JS:   static f() {}
来源：http://vdw.vqdsnc.cn

TS:   static f(): void {}
来源：http://kcy.jinyuanbaomall.cn

Java: static void f() {}
来源：http://bxv.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://npb.svipenyu.cn

Ruby: def self.f; end
来源：http://zts.jqgufenzy.top

C#:   public static void F() {}
来源：http://jhc.fzhhl.top

[G09] 接口 / 抽象类
来源：http://hpu.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://ayc.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://nia.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oqa.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://gcj.yueranfly.top

Java: interface Shape { double area(); }
来源：http://lix.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://dgv.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ckb.gogol.net.cn

C#:   interface IShape { double Area(); }
来源：http://iag.c1oappe.top

[G10] 访问控制
来源：http://erq.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://dzn.zdbjq.cn

PHP:  public / protected / private
来源：http://oyz.birdmap.top

JS:   #private 字段；其余公开
来源：http://bev.daria6918.cn

TS:   public / protected / private
来源：http://out.pengpengdd.cyou

Java: public / protected / private / 默认包级
来源：http://xvy.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://psh.zhixingplan.top

Ruby: public / protected / private
来源：http://hni.guannengcc.top

C#:   public / protected / private / internal
来源：http://iac.bjfxy.top

[G11] getter / setter
来源：http://ikh.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://tpl.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dgn.ivvv.top

JS:   get name() { return this._name; }
来源：http://bcu.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://coa.ppjwa.cn

Java: public String getName() { return name; }
来源：http://xla.yj20258888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sbn.tian-w.cn

Ruby: attr_accessor :name
来源：http://coq.kuanghao11.cn

C#:   public string Name { get; set; }
来源：http://fcu.zhixingplan.top

[G12] 对象转字符串
来源：http://nti.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://qwz.nanxuanxn.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lmi.cqqwz.cn

JS:   toString() { return this.name; }
来源：http://axy.chenjidiqi.icu

TS:   toString(): string { return this.name; }
来源：http://efz.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://iat.zhiwuduotai.top

Go:   func (u User) String() string { return u.Name }
来源：http://ckc.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://qbt.tarul.cn

C#:   public override string ToString() => Name;
来源：http://grf.hnqzz.top

[G13] 判断对象类型
来源：http://gck.tianlin.xyz

Py:   isinstance(u, User)
来源：http://dcm.yongpay.top

PHP:  $u instanceof User
来源：http://wwm.shuidangran.top

JS:   u instanceof User
来源：http://xih.yanxiufei.cn

TS:   u instanceof User
来源：http://zgl.tian-w.cn

Java: u instanceof User
来源：http://hav.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://byi.zhengqikj.top

Ruby: u.is_a?(User)
来源：http://wft.bjfxy.top

C#:   u is User
来源：http://rmv.cheryme.top

[G14] 数据类 / record
来源：http://jyt.shanyushiyangtech.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://inj.shangyingyoupin.top

PHP:  // 用 readonly 属性模拟
来源：http://cve.zhoulong.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://zza.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://vxb.fzhhl.top

Java: record User(String name, int age) {}
来源：http://cgm.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://heu.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zdt.shanyushiyangkeji.top

C#:   record User(string Name, int Age);
来源：http://wps.jinghuilouyu.cn

[G15] 枚举
来源：http://wlf.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wkr.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://anr.bbcook.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ipl.jqgufenzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://noe.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://whh.dianchejie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fan.gotoacloud.top

Ruby: Color = %i[red green].freeze
来源：http://oov.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sdt.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://dtn.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cnk.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://xeo.zhixingplan.top

JS:   Object.entries(obj)
来源：http://umg.jinghuilouyu.cn

TS:   Object.entries(obj)
来源：http://voh.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cxk.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ofq.zhixingplan.top

Ruby: obj.instance_variables
来源：http://mdp.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://ryq.316326.xyz

================================================================================
来源：http://wsl.chenlongwang.top

H. 异常与错误处理
来源：http://bcw.svipenyu.cn

================================================================================
来源：http://wgp.guowangkeji.top

[H01] try / catch 基础
来源：http://snr.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sdp.smart0.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yxs.cashguo.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://akn.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://alk.gotoacloud.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mkc.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jtl.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mbq.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://itt.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://cdm.0kj1m.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lii.hammf.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://upq.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wsk.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eqg.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://oht.feifeiyinyue.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ihd.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mkf.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nhz.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://uvo.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://pto.yongpay.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqt.zdbjq.cn

JS:   throw new Error("错误信息");
来源：http://bnj.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://lmt.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://bqc.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oor.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://vaz.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://otg.havefunace.top

[H04] 自定义异常类型
来源：http://kzc.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://dsr.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wzo.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://pje.hywenlv.cn

TS:   class MyError extends Error {}
来源：http://kiu.hnxiangtu.top

Java: class MyException extends RuntimeException {}
来源：http://pub.chenzaomai.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kjl.xinyue.icu

Ruby: class MyError < StandardError; end
来源：http://eli.cashguo.top

C#:   class MyException : Exception {}
来源：http://uvf.hfpthk.cn

[H05] 捕获特定类型
来源：http://pxy.zhiwuduotai.top

Py:   except ValueError as e:
来源：http://jhj.ydjk.org.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lhj.ppjwa.cn

JS:   if (e instanceof TypeError) {}
来源：http://kfn.vehdjk.com

TS:   if (e instanceof TypeError) {}
来源：http://lpv.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://ddf.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ibi.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://jjh.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eji.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://cyr.vehdjk.com

Py:   value = d.get("k") or default
来源：http://ges.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://xbc.andypj.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://rli.wangdashe.top

TS:   obj?.a?.b;  d ?? default
来源：http://bxv.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nqc.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nig.cheryme.top

Ruby: d&.dig(:a, :b)
来源：http://qfv.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://zqv.hongshengwenyu.top

[H07] 断言
来源：http://rww.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://ksk.jinyuanbaomall.cn

PHP:  assert($x > 0);
来源：http://hor.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://qoe.xinyue.icu

TS:   console.assert(x > 0);
来源：http://arf.fzhhl.top

Java: assert x > 0 : "必须为正";
来源：http://ngk.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yud.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://fls.shanyushiyangtech.top


<!-- 参考信息 -->