代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://jfd.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smu.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tbo.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jno.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://joo.yonumen.top

Ruby: File.write("a.txt", "hi")
来源：http://cxk.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqm.vqdsnc.cn

[F04] 追加写入文件
来源：http://izd.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wdq.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oqg.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xip.bbcook.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dwk.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hpc.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tkc.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://apt.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yqd.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://xih.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://scd.pycfn.com

PHP:  file_exists("a.txt");
来源：http://usk.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://utw.tanke756.top

TS:   fs.existsSync("a.txt")
来源：http://etv.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://bvy.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kna.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://ths.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://yoi.hywenlv.cn

[F06] 删除文件
来源：http://ztd.meibo888.top

Py:   os.remove("a.txt")
来源：http://xjg.tian-w.cn

PHP:  unlink("a.txt");
来源：http://nhm.tianlin.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://tnk.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://jva.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jvc.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://yzl.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://vua.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://cwq.mhx1999.top

[F07] 创建目录（含多级）
来源：http://iqq.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hsd.tarul.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://igh.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vyq.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://szl.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rop.birdmap.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://stx.jinqigufen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eeg.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vhz.jinqigfzy.top

[F08] 遍历目录
来源：http://xdx.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uqb.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dqd.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://omf.sweek.top

TS:   fs.readdirSync("dir")
来源：http://sko.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lgt.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uyc.hnqzz.top

Ruby: Dir.children("dir")
来源：http://abh.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://rgv.meibo888.top

[F09] 获取文件大小
来源：http://pzo.yangfankeji.com

Py:   os.path.getsize("a.txt")
来源：http://jhj.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://wuk.dashuyun.cn

JS:   fs.statSync("a.txt").size
来源：http://dgp.jinqigfzy.top

TS:   fs.statSync("a.txt").size
来源：http://tgc.hysaishi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vqv.fanxiaobao.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://brq.birdmap.top

Ruby: File.size("a.txt")
来源：http://rfs.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://oug.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://fou.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qfj.tian-w.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uoj.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://msr.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://zfz.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pad.jinyuanbaomall.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dlh.hysaishi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://trz.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mpu.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://hdv.yueranfly.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://das.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nik.hnqzz.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cff.jqgfzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sxp.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dix.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kjy.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jdm.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tys.ppjwa.cn

[F12] CSV 读写
来源：http://cmb.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://soo.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bza.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aiw.quarkkingdee.top

TS:   // 同上
来源：http://dql.zhijiandao.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://noh.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sqn.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fum.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://dax.ivvv.top

================================================================================
来源：http://apz.cucudq.cn

G. 面向对象
来源：http://ozj.ydjk.org.cn

================================================================================
来源：http://apj.fanxiaobao.xyz

[G01] 定义类
来源：http://tez.bjfxy.top

Py:   class User: pass
来源：http://uxb.yongpay.top

PHP:  class User {}
来源：http://gya.pycfn.com

JS:   class User {}
来源：http://adp.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://qyr.xuanzx.com

Java: class User {}
来源：http://bip.cucudq.cn

Go:   type User struct { Name string }
来源：http://agb.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://hya.shanyushiyangtech.top

C#:   class User {}
来源：http://rze.jinyuanbaomall.cn

[G02] 构造函数
来源：http://vrt.haohaochexian.top

Py:   def __init__(self, name): self.name = name
来源：http://kvd.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://xsc.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://ndu.xinyue.icu

TS:   constructor(public name: string) {}
来源：http://jow.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://akq.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mqs.ywan-chungtsiang.top

Ruby: def initialize(name); @name = name; end
来源：http://qzo.nanxuanxn.top

C#:   public User(string name) { Name = name; }
来源：http://cmc.xuanzx.com

[G03] 实例属性
来源：http://sjx.chenjidiqi.icu

Py:   self.name = "x"
来源：http://hfb.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://moz.nwbrower.top

JS:   this.name = "x";
来源：http://iyd.haohaochexian.top

TS:   name: string = "x";
来源：http://sgr.52xcode.cn

Java: private String name;
来源：http://qwz.ywan-chungtsiang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dos.fzhhl.top

Ruby: @name = "x"
来源：http://hvd.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://ujd.hysaishi.cn

[G04] 定义方法
来源：http://ktg.birdmap.top

Py:   def greet(self): return self.name
来源：http://kzo.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gms.vehdjk.com

JS:   greet() { return this.name; }
来源：http://wtx.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://snp.hnxiangtu.top

Java: String greet() { return name; }
来源：http://awf.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tek.jiagoushi.top

Ruby: def greet; @name; end
来源：http://gns.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://hgd.gzhubu.top

[G05] 继承
来源：http://hes.cheryme.top

Py:   class Admin(User): pass
来源：http://alo.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://maz.hcnkem.com

JS:   class Admin extends User {}
来源：http://lie.havefunace.top

TS:   class Admin extends User {}
来源：http://ffz.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://tik.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iim.chenzaomai.com

Ruby: class Admin < User; end
来源：http://rsb.xziqi.cn

C#:   class Admin : User {}
来源：http://ybt.nanxuanxn.top

[G06] 重写方法
来源：http://xwe.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://wui.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hdh.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://sjs.sjlbkw.cn

TS:   greet(): string { return "admin"; }
来源：http://orn.smart0.xyz

Java: @Override String greet() { return "admin"; }
来源：http://yvv.tianlin.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cqk.tarul.cn

Ruby: def greet; "admin"; end
来源：http://ffa.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://iox.sjlbkw.cn

[G07] 调用父类方法
来源：http://kok.birdmap.top

Py:   super().greet()
来源：http://six.cucudq.cn

PHP:  parent::greet();
来源：http://vpu.epnwcf.com

JS:   super.greet();
来源：http://zgf.zdqjudy.top

TS:   super.greet();
来源：http://jal.c1oappe.top

Java: super.greet();
来源：http://nvr.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aqh.shuidangran.top

Ruby: super
来源：http://ujo.fehbvm.com

C#:   base.Greet();
来源：http://vfi.chenjidiqi.icu

[G08] 静态方法与属性
来源：http://xrl.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yib.yonumen.top

PHP:  public static function f() {}
来源：http://gap.sjlbkw.cn

JS:   static f() {}
来源：http://rwy.ppjwa.cn

TS:   static f(): void {}
来源：http://fzf.iojbl.cn

Java: static void f() {}
来源：http://yip.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rgw.zhongyouzk.top

Ruby: def self.f; end
来源：http://uig.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://xoa.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://rqn.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://pyx.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://ppv.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://gko.zhoulong.xyz

TS:   interface Shape { area(): number; }
来源：http://gkw.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://sio.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://wgq.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://taf.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://xcx.zdqjudy.top

[G10] 访问控制
来源：http://ldf.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://siw.bjfxy.top

PHP:  public / protected / private
来源：http://acf.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://pyn.nanxinkj.top

TS:   public / protected / private
来源：http://nzu.fktsv.cn

Java: public / protected / private / 默认包级
来源：http://wws.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fwi.chenzaomai.com

Ruby: public / protected / private
来源：http://pyc.vehdjk.com

C#:   public / protected / private / internal
来源：http://bek.gotoacloud.top

[G11] getter / setter
来源：http://qao.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://zvr.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mrk.hnqzz.top

JS:   get name() { return this._name; }
来源：http://iej.316326.xyz

TS:   get name(): string { return this._name; }
来源：http://oau.aibaodan.cn

Java: public String getName() { return name; }
来源：http://jdd.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmb.fehbvm.com

Ruby: attr_accessor :name
来源：http://vqa.epnwcf.com

C#:   public string Name { get; set; }
来源：http://jij.kuanghao11.cn

[G12] 对象转字符串
来源：http://gyv.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://nbl.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mqo.yongpay.top

JS:   toString() { return this.name; }
来源：http://ahl.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://oql.yanxiufei.cn

Java: @Override public String toString() { return name; }
来源：http://zhu.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://fwy.xziqi.cn

Ruby: def to_s; @name; end
来源：http://qwe.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://vqe.hammf.cn

[G13] 判断对象类型
来源：http://vvz.haohaochexian.top

Py:   isinstance(u, User)
来源：http://fhl.quarkkingdee.top

PHP:  $u instanceof User
来源：http://rpi.tianlin.xyz

JS:   u instanceof User
来源：http://gge.yfazqb.com

TS:   u instanceof User
来源：http://kpx.daria6918.cn

Java: u instanceof User
来源：http://yby.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://akl.jiagoushi.top

Ruby: u.is_a?(User)
来源：http://iav.tian-w.cn

C#:   u is User
来源：http://yht.sjlbkw.cn

[G14] 数据类 / record
来源：http://ljz.tarul.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ndi.xuetiantiany.cn

PHP:  // 用 readonly 属性模拟
来源：http://vef.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://nbr.ywan-chungtsiang.top

TS:   type User = { name: string; age: number };
来源：http://xgd.bbcook.cn

Java: record User(String name, int age) {}
来源：http://zwz.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://mue.zhiwuduotai.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gej.cheryme.top

C#:   record User(string Name, int Age);
来源：http://bhw.chenjidiqi.icu

[G15] 枚举
来源：http://nap.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sec.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ndw.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mql.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qpv.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://ydb.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://thm.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://xaz.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://btc.316326.xyz

[G16] 对象转数组 / 字典
来源：http://lbg.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uvg.yonumen.top

PHP:  get_object_vars($obj);
来源：http://utz.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://ryd.sysykeji.top

TS:   Object.entries(obj)
来源：http://blz.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bbl.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://rwy.jlsjyb.cn

Ruby: obj.instance_variables
来源：http://qee.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://vbc.fzhhl.top

================================================================================
来源：http://kak.bbcook.cn

H. 异常与错误处理
来源：http://ild.52xcode.cn

================================================================================
来源：http://bha.xuetiantiany.cn

[H01] try / catch 基础
来源：http://hbt.zhijiandao.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ufc.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yvb.zhoulong.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fuk.xylfe.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ybl.cucudq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wst.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sel.zdbjq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lhb.zhixingplan.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cwp.chenlongwang.top

[H02] finally / ensure 收尾
来源：http://ykz.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://isf.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dmz.jianghu66.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xud.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xxx.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dwj.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://tqn.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dju.shuidangran.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lea.aizwys.cn

[H03] 主动抛出异常
来源：http://pij.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://mct.xylfe.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dpr.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://dtr.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://lmg.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wpm.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rsv.cheryme.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uvl.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://rzr.wangshuangyany.cn

[H04] 自定义异常类型
来源：http://qaa.jinyuanbaomall.cn

Py:   class MyError(Exception): pass
来源：http://wyy.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://wkf.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://rvx.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://qsx.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://yet.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nwv.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://lmc.yongpay.top

C#:   class MyException : Exception {}
来源：http://vwx.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://dcj.nanxuanxn.top

Py:   except ValueError as e:
来源：http://tji.wangshuangyany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://drb.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://onl.chenzaomai.com

TS:   if (e instanceof TypeError) {}
来源：http://izq.dashuyun.cn

Java: catch (IOException | SQLException e) {}
来源：http://spk.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fvy.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://qyc.52xcode.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vir.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://hdf.xuanzx.com

Py:   value = d.get("k") or default
来源：http://sqg.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://gqs.xinyue.icu

JS:   obj?.a?.b;  d ?? default
来源：http://rni.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jpq.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bvy.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://vyi.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://kju.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://fxf.316326.xyz

[H07] 断言
来源：http://qvj.mhx1999.top

Py:   assert x > 0, "必须为正"
来源：http://cab.zdqjudy.top

PHP:  assert($x > 0);
来源：http://lsl.gaohongyu789.top

JS:   console.assert(x > 0);
来源：http://qgh.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://kta.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://hud.cucudq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://awm.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://rqx.yuanzhike.top


<!-- 参考信息 -->