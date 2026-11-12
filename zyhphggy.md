代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://vbw.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sdd.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lxn.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mng.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vvq.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://mnp.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yvt.jqgufenzy.top

[F04] 追加写入文件
来源：http://dao.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yib.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://woc.zhiwuduotai.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xfr.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nad.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lmt.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ufo.fengsongda.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uuu.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tzb.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://pxt.xinyue.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iqx.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://qdn.uphjek.com

JS:   fs.existsSync("a.txt")
来源：http://qmu.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://guw.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ksz.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qxs.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://nsh.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://ubs.zhengqikj.top

[F06] 删除文件
来源：http://uoj.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://hne.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://jem.vqdsnc.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pqx.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://wun.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sih.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://ygs.jiagoushi.top

Ruby: File.delete("a.txt")
来源：http://ygo.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://zdd.havefunace.top

[F07] 创建目录（含多级）
来源：http://pfa.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vvi.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://auf.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mcs.hnqzz.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gxb.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zai.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gxy.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://abq.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://itm.gzhubu.top

[F08] 遍历目录
来源：http://zes.jianghu66.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iok.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tym.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://hqm.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://ohi.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://val.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iko.ydzc1.top

Ruby: Dir.children("dir")
来源：http://vtq.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://btj.zdqjudy.top

[F09] 获取文件大小
来源：http://auj.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://mal.fengsongda.top

PHP:  filesize("a.txt");
来源：http://tjw.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://dsz.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://muo.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://mfr.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oyd.ivvv.top

Ruby: File.size("a.txt")
来源：http://fce.jiagoushi.top

C#:   new FileInfo("a.txt").Length
来源：http://vci.dianchejie.cn

[F10] 取文件扩展名 / 文件名
来源：http://emn.jinqigufen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rcb.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fia.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ffp.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://vhg.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ihk.yueranfly.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kfq.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hvj.ydzc1.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mdi.xuanzx.com

[F11] 复制与移动文件
来源：http://upr.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yxi.hcnkem.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ixl.haohaochexian.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zqx.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xxw.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://edv.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fra.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fpg.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nuk.gotoacloud.top

[F12] CSV 读写
来源：http://rvm.yvedp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://anp.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uyk.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iwp.xinyue.icu

TS:   // 同上
来源：http://oyu.wangdashe.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uqr.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lng.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ppp.dianchejie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qoa.jqgfzy.top

================================================================================
来源：http://zac.fehbvm.com

G. 面向对象
来源：http://txf.birdmap.top

================================================================================
来源：http://lki.smart0.xyz

[G01] 定义类
来源：http://jpy.bjfxy.top

Py:   class User: pass
来源：http://gpx.nanxuanxn.top

PHP:  class User {}
来源：http://wfg.hnxiangtu.top

JS:   class User {}
来源：http://bit.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://lkd.svipenyu.cn

Java: class User {}
来源：http://cin.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://gpw.mhx1999.top

Ruby: class User; end
来源：http://mfd.svipenyu.cn

C#:   class User {}
来源：http://qmi.dianchejie.cn

[G02] 构造函数
来源：http://qxm.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://ojl.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://gje.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://sjo.0kj1m.cn

TS:   constructor(public name: string) {}
来源：http://ypo.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://cdq.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fds.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://ess.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://oqb.dianchejie.cn

[G03] 实例属性
来源：http://ckp.hcnkem.com

Py:   self.name = "x"
来源：http://zwk.zhongyouzk.top

PHP:  public string $name = "x";
来源：http://emm.zhixingplan.top

JS:   this.name = "x";
来源：http://icy.uphjek.com

TS:   name: string = "x";
来源：http://wqv.cdnleiting.top

Java: private String name;
来源：http://whu.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xaw.cdnleiting.top

Ruby: @name = "x"
来源：http://qbw.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://yex.yuxming.cn

[G04] 定义方法
来源：http://xmk.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://usd.vehdjk.com

PHP:  public function greet(): string { return $this->name; }
来源：http://gry.tian-w.cn

JS:   greet() { return this.name; }
来源：http://set.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://xxm.fktsv.cn

Java: String greet() { return name; }
来源：http://fch.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://odn.jinqigufen.top

Ruby: def greet; @name; end
来源：http://ljk.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://dxk.uphjek.com

[G05] 继承
来源：http://ovs.ydjk.org.cn

Py:   class Admin(User): pass
来源：http://ypf.wangdashe.top

PHP:  class Admin extends User {}
来源：http://otw.fengsongda.top

JS:   class Admin extends User {}
来源：http://xwk.yuxming.cn

TS:   class Admin extends User {}
来源：http://gvg.shzxlz.cn

Java: class Admin extends User {}
来源：http://ume.gaohongyu789.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://awb.nanxinkj.top

Ruby: class Admin < User; end
来源：http://yve.cdnleiting.top

C#:   class Admin : User {}
来源：http://kfo.jianghu66.top

[G06] 重写方法
来源：http://zxl.birdmap.top

Py:   def greet(self): return "admin"
来源：http://rlr.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://edo.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ett.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://dpv.cashguo.top

Java: @Override String greet() { return "admin"; }
来源：http://xsn.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iru.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://gyk.hammf.cn

C#:   public override string Greet() => "admin";
来源：http://fzw.jinqigfzy.top

[G07] 调用父类方法
来源：http://dmr.chenjidiqi.icu

Py:   super().greet()
来源：http://xiu.cashguo.top

PHP:  parent::greet();
来源：http://ylx.shanyushiyangkeji.top

JS:   super.greet();
来源：http://hjp.zhixingplan.top

TS:   super.greet();
来源：http://pgq.yueranfly.top

Java: super.greet();
来源：http://hkt.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oaq.cashguo.top

Ruby: super
来源：http://cnl.hnqzz.top

C#:   base.Greet();
来源：http://gzw.cqqwz.cn

[G08] 静态方法与属性
来源：http://hbu.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aog.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://cmu.guannengcc.top

JS:   static f() {}
来源：http://olv.feifeiyinyue.top

TS:   static f(): void {}
来源：http://xoc.ybcxt.top

Java: static void f() {}
来源：http://hgy.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://quv.zdqjudy.top

Ruby: def self.f; end
来源：http://xwy.gzhubu.top

C#:   public static void F() {}
来源：http://kps.sjlbkw.cn

[G09] 接口 / 抽象类
来源：http://fma.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://gmy.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://mcw.zhiwuduotai.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://atl.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://rza.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://rbt.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://rvj.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ugy.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://xfv.tianlin.xyz

[G10] 访问控制
来源：http://qix.shanyushiyangtech.top

Py:   约定 _protected / __private（不强制）
来源：http://yln.fengsongda.top

PHP:  public / protected / private
来源：http://ikl.hesvh.cn

JS:   #private 字段；其余公开
来源：http://gvp.hnqzz.top

TS:   public / protected / private
来源：http://bqs.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://pcp.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cpf.xinyue.icu

Ruby: public / protected / private
来源：http://alz.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://idd.yueranfly.top

[G11] getter / setter
来源：http://oem.yj20258.top

Py:   @property 与 @x.setter
来源：http://bbb.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://mrf.fzhhl.top

JS:   get name() { return this._name; }
来源：http://wpu.hysaishi.cn

TS:   get name(): string { return this._name; }
来源：http://awd.iojbl.cn

Java: public String getName() { return name; }
来源：http://cxs.shangyingyoupin.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lsj.guannengcc.top

Ruby: attr_accessor :name
来源：http://lyd.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://nyw.yuanzhike.top

[G12] 对象转字符串
来源：http://yhj.sweek.top

Py:   def __str__(self): return self.name
来源：http://inh.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://xuf.xingfuxueyuan.xyz

JS:   toString() { return this.name; }
来源：http://lvu.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://cju.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://aoo.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nvn.zhixingplan.top

Ruby: def to_s; @name; end
来源：http://pyq.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://mgi.smart0.xyz

[G13] 判断对象类型
来源：http://niu.c1oappe.top

Py:   isinstance(u, User)
来源：http://vbr.hammf.cn

PHP:  $u instanceof User
来源：http://oei.bbcook.cn

JS:   u instanceof User
来源：http://jum.vehdjk.com

TS:   u instanceof User
来源：http://fxs.zhengqikj.top

Java: u instanceof User
来源：http://dqx.aizwys.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://clm.uphjek.com

Ruby: u.is_a?(User)
来源：http://guc.hfpthk.cn

C#:   u is User
来源：http://qqj.c1oappe.top

[G14] 数据类 / record
来源：http://ctw.quarkkingdee.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cej.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://ppw.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://pwq.zhongyouzk.top

TS:   type User = { name: string; age: number };
来源：http://xde.hcnkem.com

Java: record User(String name, int age) {}
来源：http://hhq.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://skf.haohaochexian.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uuv.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://uve.quarkkingdee.top

[G15] 枚举
来源：http://zwz.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bma.kuanghao11.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mmu.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://avj.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ypa.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://cby.tianlin.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mdl.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://nqd.52xcode.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hqz.cqqwz.cn

[G16] 对象转数组 / 字典
来源：http://rvw.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sfg.shzxlz.cn

PHP:  get_object_vars($obj);
来源：http://nei.sweek.top

JS:   Object.entries(obj)
来源：http://mvo.316326.xyz

TS:   Object.entries(obj)
来源：http://kkl.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vbg.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://bfv.sysykeji.top

Ruby: obj.instance_variables
来源：http://iqb.0kj1m.cn

C#:   // 用反射或 System.Text.Json
来源：http://tph.mhx1999.top

================================================================================
来源：http://fmr.uphjek.com

H. 异常与错误处理
来源：http://onu.vehdjk.com

================================================================================
来源：http://bar.ppjwa.cn

[H01] try / catch 基础
来源：http://ynh.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://swe.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bfs.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yzt.vqdsnc.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zvl.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nrt.quarkkingdee.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://deg.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tux.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qym.dianchejie.cn

[H02] finally / ensure 收尾
来源：http://xdb.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://ytr.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hah.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nuq.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qdz.hesvh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jrb.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pik.fktsv.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ysh.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zvo.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://wsi.fengsongda.top

Py:   raise ValueError("错误信息")
来源：http://mku.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eos.chenjidiqi.icu

JS:   throw new Error("错误信息");
来源：http://cpm.yonumen.top

TS:   throw new Error("错误信息");
来源：http://rax.hongshengwenyu.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tvx.hnqzz.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wca.xziqi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cmg.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://tly.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://lra.cucudq.cn

Py:   class MyError(Exception): pass
来源：http://fwz.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://arl.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://rpr.fktsv.cn

TS:   class MyError extends Error {}
来源：http://qce.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://yll.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://crb.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://kow.tanke756.top

C#:   class MyException : Exception {}
来源：http://qqw.yj20258888.top

[H05] 捕获特定类型
来源：http://rvv.fktsv.cn

Py:   except ValueError as e:
来源：http://usv.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mbp.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://bmc.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://azg.jiagoushi.top

Java: catch (IOException | SQLException e) {}
来源：http://cfh.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://swm.ybcxt.top

Ruby: rescue ArgumentError => e
来源：http://igu.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pwl.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://zyn.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://pbw.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://dja.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://pkv.jinghuilouyu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kub.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hfw.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zpy.aizwys.cn

Ruby: d&.dig(:a, :b)
来源：http://czd.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://vpf.hysaishi.cn

[H07] 断言
来源：http://saz.cheryme.top

Py:   assert x > 0, "必须为正"
来源：http://esa.zdbjq.cn

PHP:  assert($x > 0);
来源：http://jfn.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://cne.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://xby.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://mvs.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aof.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://sgb.vehdjk.com


<!-- 参考信息 -->