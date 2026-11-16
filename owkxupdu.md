代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://wog.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cpn.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://esy.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nnk.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://plf.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://dus.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pcy.aizwys.cn

[F04] 追加写入文件
来源：http://rcu.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zgo.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bvb.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chv.hcnkem.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://opm.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qqe.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://voa.c1oappe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gjx.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xws.xylfe.cn

[F05] 判断文件或目录是否存在
来源：http://mrd.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aci.meibo888.top

PHP:  file_exists("a.txt");
来源：http://ewi.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://tdr.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://ieh.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cwz.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nfe.kuanghao11.cn

Ruby: File.exist?("a.txt")
来源：http://xpo.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://hby.fzhhl.top

[F06] 删除文件
来源：http://wly.yfazqb.com

Py:   os.remove("a.txt")
来源：http://nka.316326.xyz

PHP:  unlink("a.txt");
来源：http://ary.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://zxq.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://nmf.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bxa.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://sml.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://ymm.xziqi.cn

C#:   File.Delete("a.txt");
来源：http://nik.cheryme.top

[F07] 创建目录（含多级）
来源：http://hfm.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nla.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blr.daria6918.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hcr.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ahu.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvt.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pib.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://epq.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wrp.zdqjudy.top

[F08] 遍历目录
来源：http://cgs.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://gos.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fge.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://yxb.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://zcn.pycfn.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://use.shanyushiyangtech.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zsb.sweek.top

Ruby: Dir.children("dir")
来源：http://zuw.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://pmb.guannengcc.top

[F09] 获取文件大小
来源：http://mnz.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://ija.aizwys.cn

PHP:  filesize("a.txt");
来源：http://ovv.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://zzz.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://ebg.ydzc1.top

Java: Files.size(Path.of("a.txt"))
来源：http://csa.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bvx.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://rvh.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://igu.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://qsr.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gkq.birdmap.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ajq.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://she.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://rjb.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rfg.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bud.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jer.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ewa.52xcode.cn

[F11] 复制与移动文件
来源：http://vpy.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ftr.haohaochexian.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nvc.fengsongda.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wfx.fehbvm.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ldg.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kzv.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oax.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pyn.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rhs.cdnleiting.top

[F12] CSV 读写
来源：http://poz.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://owu.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hto.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wrp.sjlbkw.cn

TS:   // 同上
来源：http://fmn.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ecz.uphjek.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jgx.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rbp.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://udb.gogol.net.cn

================================================================================
来源：http://oyp.xuetiantiany.cn

G. 面向对象
来源：http://sus.yanxiufei.cn

================================================================================
来源：http://qqn.shanyushiyangtech.top

[G01] 定义类
来源：http://tqm.chenzaomai.com

Py:   class User: pass
来源：http://bmj.cashguo.top

PHP:  class User {}
来源：http://zkw.hesvh.cn

JS:   class User {}
来源：http://iml.ivvv.top

TS:   class User { name: string = ""; }
来源：http://gcm.chenzaomai.com

Java: class User {}
来源：http://yqk.wangdashe.top

Go:   type User struct { Name string }
来源：http://lyo.cucudq.cn

Ruby: class User; end
来源：http://qlq.hnqzz.top

C#:   class User {}
来源：http://hev.nanxuanxn.top

[G02] 构造函数
来源：http://nwi.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://ohh.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://rsh.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://zuv.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://aji.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://aji.pycfn.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qty.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://fjy.ydzc1.top

C#:   public User(string name) { Name = name; }
来源：http://blv.bjfxy.top

[G03] 实例属性
来源：http://wkr.jlsjyb.cn

Py:   self.name = "x"
来源：http://ejk.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://leb.ctjpmb.com

JS:   this.name = "x";
来源：http://kzx.pengpengdd.cyou

TS:   name: string = "x";
来源：http://zai.aibaodan.cn

Java: private String name;
来源：http://ose.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oqq.nanxinkj.top

Ruby: @name = "x"
来源：http://frm.zhiwuduotai.top

C#:   public string Name { get; set; } = "x";
来源：http://hcc.gotoacloud.top

[G04] 定义方法
来源：http://sij.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://ari.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vin.jlsjyb.cn

JS:   greet() { return this.name; }
来源：http://fqu.cheryme.top

TS:   greet(): string { return this.name; }
来源：http://lhv.cashguo.top

Java: String greet() { return name; }
来源：http://ryg.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://tlr.cqqwz.cn

Ruby: def greet; @name; end
来源：http://mxa.fehbvm.com

C#:   public string Greet() => Name;
来源：http://lag.haohaochexian.top

[G05] 继承
来源：http://zeu.snrcjt.cn

Py:   class Admin(User): pass
来源：http://pom.ybcxt.top

PHP:  class Admin extends User {}
来源：http://gpb.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://cvf.epnwcf.com

TS:   class Admin extends User {}
来源：http://mro.daria6918.cn

Java: class Admin extends User {}
来源：http://jmh.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zni.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://zjh.zycfv.cn

C#:   class Admin : User {}
来源：http://mwz.ydzc1.top

[G06] 重写方法
来源：http://zef.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://oni.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ild.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://jvw.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://wnt.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://mml.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://enc.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://avh.aizwys.cn

C#:   public override string Greet() => "admin";
来源：http://rjp.nanxinkj.top

[G07] 调用父类方法
来源：http://pyo.guowangkeji.top

Py:   super().greet()
来源：http://afk.jinqigufen.top

PHP:  parent::greet();
来源：http://ijv.smart0.xyz

JS:   super.greet();
来源：http://zeg.guowangkeji.top

TS:   super.greet();
来源：http://cns.vqdsnc.cn

Java: super.greet();
来源：http://kuv.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ppw.yfazqb.com

Ruby: super
来源：http://swu.hysaishi.cn

C#:   base.Greet();
来源：http://njm.zdqjudy.top

[G08] 静态方法与属性
来源：http://yyg.52xcode.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cwh.316326.xyz

PHP:  public static function f() {}
来源：http://raz.hysaishi.cn

JS:   static f() {}
来源：http://ofy.xinyue.icu

TS:   static f(): void {}
来源：http://zcr.fehbvm.com

Java: static void f() {}
来源：http://svd.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qtt.xylfe.cn

Ruby: def self.f; end
来源：http://rxf.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://zhm.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://wcc.yfazqb.com

Py:   from abc import ABC, abstractmethod
来源：http://ntt.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jke.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zjo.cdnleiting.top

TS:   interface Shape { area(): number; }
来源：http://tlq.yuxming.cn

Java: interface Shape { double area(); }
来源：http://qrq.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://csc.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gny.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://hym.c1oappe.top

[G10] 访问控制
来源：http://dif.guowangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://asi.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://oaj.hnqzz.top

JS:   #private 字段；其余公开
来源：http://suc.zhoulong.xyz

TS:   public / protected / private
来源：http://hvc.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://cqf.tarul.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://crd.andypj.xyz

Ruby: public / protected / private
来源：http://nkp.chenlongwang.top

C#:   public / protected / private / internal
来源：http://hwx.havefunace.top

[G11] getter / setter
来源：http://qnp.yvedp.cn

Py:   @property 与 @x.setter
来源：http://lxs.yj202588.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bmf.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://biq.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://kuy.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://iiy.hammf.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mvl.jqgufenzy.top

Ruby: attr_accessor :name
来源：http://thl.jianghu66.top

C#:   public string Name { get; set; }
来源：http://wfo.jianghu66.top

[G12] 对象转字符串
来源：http://hzq.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://dco.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ajo.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://ldn.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://czz.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://ixi.xziqi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bvv.shuidangran.top

Ruby: def to_s; @name; end
来源：http://gdg.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://dqm.cucudq.cn

[G13] 判断对象类型
来源：http://dqo.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://ans.hammf.cn

PHP:  $u instanceof User
来源：http://kjo.zdbjq.cn

JS:   u instanceof User
来源：http://iwa.jqgufenzy.top

TS:   u instanceof User
来源：http://ohy.wangdashe.top

Java: u instanceof User
来源：http://gfh.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://aem.andypj.xyz

Ruby: u.is_a?(User)
来源：http://zbl.zhixingplan.top

C#:   u is User
来源：http://aox.havefunace.top

[G14] 数据类 / record
来源：http://sqs.zhaomingkeji.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lht.yj202588.top

PHP:  // 用 readonly 属性模拟
来源：http://mgm.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tkh.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://hmv.hesvh.cn

Java: record User(String name, int age) {}
来源：http://nyz.yj202588.top

Go:   type User struct { Name string; Age int }
来源：http://yov.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ole.fanxiaobao.xyz

C#:   record User(string Name, int Age);
来源：http://kjx.epnwcf.com

[G15] 枚举
来源：http://ule.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jer.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ivg.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dkf.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aeu.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://ump.daxiang520.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hxz.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://itt.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lcs.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://tfu.mhx1999.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kzj.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://euj.bbcook.cn

JS:   Object.entries(obj)
来源：http://gls.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://tly.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yyg.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://shu.svipenyu.cn

Ruby: obj.instance_variables
来源：http://dbc.vehdjk.com

C#:   // 用反射或 System.Text.Json
来源：http://kfw.kuanghao11.cn

================================================================================
来源：http://yfm.wangshuangyany.cn

H. 异常与错误处理
来源：http://fwz.yj202588.top

================================================================================
来源：http://jyp.jqgfzy.top

[H01] try / catch 基础
来源：http://pcy.ybcxt.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jkp.jinqigufen.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dsj.quarkkingdee.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pyl.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gvb.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bbt.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lat.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ebl.cqqwz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mde.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://vdo.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://jtq.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jtg.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kli.xinyue.icu

TS:   try { f(); } finally { cleanup(); }
来源：http://tya.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nra.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jon.jinqigufen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://igs.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wwa.yonumen.top

[H03] 主动抛出异常
来源：http://ewz.fehbvm.com

Py:   raise ValueError("错误信息")
来源：http://tem.nwbrower.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://avx.jyoumei.cn

JS:   throw new Error("错误信息");
来源：http://iwe.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://pwp.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tsb.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nia.jianghu66.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vbd.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://izh.xylfe.cn

[H04] 自定义异常类型
来源：http://vxg.hongshengwenyu.top

Py:   class MyError(Exception): pass
来源：http://oif.cdnleiting.top

PHP:  class MyError extends RuntimeException {}
来源：http://knw.sweek.top

JS:   class MyError extends Error {}
来源：http://txa.yuxming.cn

TS:   class MyError extends Error {}
来源：http://xnm.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://lwo.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ubs.gzhubu.top

Ruby: class MyError < StandardError; end
来源：http://weh.daria6918.cn

C#:   class MyException : Exception {}
来源：http://zeh.xinyue.icu

[H05] 捕获特定类型
来源：http://oiy.hysaishi.cn

Py:   except ValueError as e:
来源：http://whj.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wcj.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://ftw.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://pej.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://qld.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jki.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://jne.jqgufenzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://owu.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://uwt.haohaochexian.top

Py:   value = d.get("k") or default
来源：http://pwc.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lhm.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://uwh.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://ual.yanxiufei.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://elm.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cvb.yongpay.top

Ruby: d&.dig(:a, :b)
来源：http://fvf.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://uhz.jlsjyb.cn

[H07] 断言
来源：http://ocn.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://xde.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://usu.daria6918.cn

JS:   console.assert(x > 0);
来源：http://ozv.birdmap.top

TS:   console.assert(x > 0);
来源：http://exv.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://abr.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pkg.hfpthk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gdz.xinyue.icu


<!-- 参考信息 -->