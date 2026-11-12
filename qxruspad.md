代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://och.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://aac.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://piz.xylfe.cn

[F04] 追加写入文件
来源：http://tnj.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qks.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gwt.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rqp.jiagoushi.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ogt.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wsv.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dsz.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wsu.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gns.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://cls.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hcy.vehdjk.com

PHP:  file_exists("a.txt");
来源：http://arb.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://tpb.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://zqp.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cny.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oie.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://zjm.ivvv.top

C#:   File.Exists("a.txt")
来源：http://has.mhx1999.top

[F06] 删除文件
来源：http://uqo.yueranfly.top

Py:   os.remove("a.txt")
来源：http://qlx.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://rey.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://rpa.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uqi.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ruc.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://zfh.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://hpq.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://hhr.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://rlm.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jnm.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ztq.fengsongda.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fcc.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xal.yj20258888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uwh.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mto.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rey.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fow.mhx1999.top

[F08] 遍历目录
来源：http://thf.tian-w.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iha.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kgs.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://uyh.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://eeo.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bbj.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qdm.xziqi.cn

Ruby: Dir.children("dir")
来源：http://uvz.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://nmj.mhx1999.top

[F09] 获取文件大小
来源：http://kgq.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://bbn.fzhhl.top

PHP:  filesize("a.txt");
来源：http://zdf.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://psq.shuidangran.top

TS:   fs.statSync("a.txt").size
来源：http://utn.shanyushiyangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://jqb.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xef.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://idh.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://pdt.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://ypv.shanyushiyangtech.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eik.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fio.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qvi.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://ljv.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://khl.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wyk.andypj.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ymx.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dkj.0kj1m.cn

[F11] 复制与移动文件
来源：http://uij.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ixi.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xgs.yanxiufei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktv.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ctt.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gev.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lxr.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://phe.yueranfly.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nvb.xuetiantiany.cn

[F12] CSV 读写
来源：http://ndh.gaohongyu789.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://opl.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fen.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hgd.hnqzz.top

TS:   // 同上
来源：http://pbf.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ktt.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fpz.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gsk.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fxh.fanxiaobao.xyz

================================================================================
来源：http://lar.jinghuilouyu.cn

G. 面向对象
来源：http://eqm.fanxiaobao.xyz

================================================================================
来源：http://nkv.jyoumei.cn

[G01] 定义类
来源：http://jdl.mhx1999.top

Py:   class User: pass
来源：http://rrf.zhijiandao.cn

PHP:  class User {}
来源：http://kbk.chenjidiqi.icu

JS:   class User {}
来源：http://ayo.ivvv.top

TS:   class User { name: string = ""; }
来源：http://twe.gogol.net.cn

Java: class User {}
来源：http://gzx.haohaochexian.top

Go:   type User struct { Name string }
来源：http://bet.gzhubu.top

Ruby: class User; end
来源：http://dws.yvedp.cn

C#:   class User {}
来源：http://cux.yj20258888.top

[G02] 构造函数
来源：http://ffr.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://kid.feifeiyinyue.top

PHP:  public function __construct(public string $name) {}
来源：http://ymq.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://oub.tarul.cn

TS:   constructor(public name: string) {}
来源：http://zit.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://vxz.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bvw.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://ixm.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://jxu.nanxinkj.top

[G03] 实例属性
来源：http://ypi.gaohongyu789.top

Py:   self.name = "x"
来源：http://cek.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://dtr.kuanghao11.cn

JS:   this.name = "x";
来源：http://xvs.zhijiandao.cn

TS:   name: string = "x";
来源：http://vwj.wangdashe.top

Java: private String name;
来源：http://jux.9152youxi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://epz.snrcjt.cn

Ruby: @name = "x"
来源：http://mtz.yj202588.top

C#:   public string Name { get; set; } = "x";
来源：http://hyr.sxryk.cn

[G04] 定义方法
来源：http://yxa.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://npc.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jpl.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://ejj.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://prf.nanxuanxn.top

Java: String greet() { return name; }
来源：http://dbw.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ptk.hywenlv.cn

Ruby: def greet; @name; end
来源：http://rgv.tanke756.top

C#:   public string Greet() => Name;
来源：http://hhh.tarul.cn

[G05] 继承
来源：http://xzx.fktsv.cn

Py:   class Admin(User): pass
来源：http://ptf.yj20258.top

PHP:  class Admin extends User {}
来源：http://znl.shuidangran.top

JS:   class Admin extends User {}
来源：http://hfg.xziqi.cn

TS:   class Admin extends User {}
来源：http://rqo.shzxlz.cn

Java: class Admin extends User {}
来源：http://ypb.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://krn.sufxvd.cn

Ruby: class Admin < User; end
来源：http://odb.yuanzhike.top

C#:   class Admin : User {}
来源：http://usc.fzhhl.top

[G06] 重写方法
来源：http://btt.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://rkd.jlsjyb.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qnp.yj202588.top

JS:   greet() { return "admin"; }
来源：http://dyn.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://llj.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://zms.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibt.hesvh.cn

Ruby: def greet; "admin"; end
来源：http://cxr.fanxiaobao.xyz

C#:   public override string Greet() => "admin";
来源：http://roz.nwbrower.top

[G07] 调用父类方法
来源：http://ehv.pycfn.com

Py:   super().greet()
来源：http://bwl.tian-w.cn

PHP:  parent::greet();
来源：http://ciy.cashguo.top

JS:   super.greet();
来源：http://hth.guannengcc.top

TS:   super.greet();
来源：http://asr.vehdjk.com

Java: super.greet();
来源：http://gms.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://crh.dianchejie.cn

Ruby: super
来源：http://hvm.fzhhl.top

C#:   base.Greet();
来源：http://tey.vehdjk.com

[G08] 静态方法与属性
来源：http://axd.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qsf.wangshuangyany.cn

PHP:  public static function f() {}
来源：http://hjs.yonumen.top

JS:   static f() {}
来源：http://vtj.jianghu66.top

TS:   static f(): void {}
来源：http://pia.chenzaomai.com

Java: static void f() {}
来源：http://tyl.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rlg.0kj1m.cn

Ruby: def self.f; end
来源：http://bxx.zycfv.cn

C#:   public static void F() {}
来源：http://dkl.hammf.cn

[G09] 接口 / 抽象类
来源：http://uuw.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://cnp.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://vxu.xylfe.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vst.daria6918.cn

TS:   interface Shape { area(): number; }
来源：http://fny.c1oappe.top

Java: interface Shape { double area(); }
来源：http://tlm.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://jnm.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ime.xziqi.cn

C#:   interface IShape { double Area(); }
来源：http://poh.ehwqpu.com

[G10] 访问控制
来源：http://csl.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://icc.tianlin.xyz

PHP:  public / protected / private
来源：http://pqj.yj20258.top

JS:   #private 字段；其余公开
来源：http://hkh.xuetiantiany.cn

TS:   public / protected / private
来源：http://kpv.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://ljl.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rak.hnxiangtu.top

Ruby: public / protected / private
来源：http://bgd.yvedp.cn

C#:   public / protected / private / internal
来源：http://lay.cashguo.top

[G11] getter / setter
来源：http://mha.gzhubu.top

Py:   @property 与 @x.setter
来源：http://lln.uphjek.com

PHP:  public function getName(): string { return $this->name; }
来源：http://uwh.shuidangran.top

JS:   get name() { return this._name; }
来源：http://hzx.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://ftb.shzxlz.cn

Java: public String getName() { return name; }
来源：http://zpa.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ljz.ctjpmb.com

Ruby: attr_accessor :name
来源：http://rzj.yuxming.cn

C#:   public string Name { get; set; }
来源：http://cjo.bjfxy.top

[G12] 对象转字符串
来源：http://zxi.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://mgl.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffo.ppjwa.cn

JS:   toString() { return this.name; }
来源：http://vmy.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://mjr.nanxuanxn.top

Java: @Override public String toString() { return name; }
来源：http://ree.ehwqpu.com

Go:   func (u User) String() string { return u.Name }
来源：http://lkp.xylfe.cn

Ruby: def to_s; @name; end
来源：http://anr.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://wva.dashuyun.cn

[G13] 判断对象类型
来源：http://lhi.cheryme.top

Py:   isinstance(u, User)
来源：http://lww.cashguo.top

PHP:  $u instanceof User
来源：http://kyg.havefunace.top

JS:   u instanceof User
来源：http://epe.hcnkem.com

TS:   u instanceof User
来源：http://dyk.sjlbkw.cn

Java: u instanceof User
来源：http://amw.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://mdg.uphjek.com

Ruby: u.is_a?(User)
来源：http://aeb.redwolf501.top

C#:   u is User
来源：http://cet.dianchejie.cn

[G14] 数据类 / record
来源：http://lhm.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iwx.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://isj.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://soa.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://ooo.ydzc1.top

Java: record User(String name, int age) {}
来源：http://tzn.cqqwz.cn

Go:   type User struct { Name string; Age int }
来源：http://ote.hfpthk.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nge.xylfe.cn

C#:   record User(string Name, int Age);
来源：http://poz.svipenyu.cn

[G15] 枚举
来源：http://awh.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nbs.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://znc.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ztq.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vgz.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://uhl.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qvk.zhengqikj.top

Ruby: Color = %i[red green].freeze
来源：http://mca.wangshuangyany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zez.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://vvp.ybcxt.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wnc.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://vkq.jqgfzy.top

JS:   Object.entries(obj)
来源：http://uej.xuetiantiany.cn

TS:   Object.entries(obj)
来源：http://zzb.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://otz.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://vrv.redwolf501.top

Ruby: obj.instance_variables
来源：http://twn.cheryme.top

C#:   // 用反射或 System.Text.Json
来源：http://wjh.shanyushiyangkeji.top

================================================================================
来源：http://tdw.aizwys.cn

H. 异常与错误处理
来源：http://vaq.wangshuangyany.cn

================================================================================
来源：http://mpe.jlsjyb.cn

[H01] try / catch 基础
来源：http://imy.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sun.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ojv.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mao.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jro.hnqzz.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qnp.xuanzx.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lrt.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wuz.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ovh.jinqigufen.top

[H02] finally / ensure 收尾
来源：http://fhv.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mzj.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lol.mhx1999.top

JS:   try { f(); } finally { cleanup(); }
来源：http://prj.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ypz.9152youxi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ouz.fktsv.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://axs.shanyushiyangkeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://egi.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bgs.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://tqb.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://gff.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pbq.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://jiv.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://sgn.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zmg.zhaomingkeji.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cqf.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://jkn.xingfuxueyuan.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://eez.ydjk.org.cn

[H04] 自定义异常类型
来源：http://cso.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://byb.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://tkm.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://fyr.daria6918.cn

TS:   class MyError extends Error {}
来源：http://ivv.cdnleiting.top

Java: class MyException extends RuntimeException {}
来源：http://tko.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vam.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://vop.ybcxt.top

C#:   class MyException : Exception {}
来源：http://bqz.hywenlv.cn

[H05] 捕获特定类型
来源：http://jxj.tarul.cn

Py:   except ValueError as e:
来源：http://qbz.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ksf.cashguo.top

JS:   if (e instanceof TypeError) {}
来源：http://jjf.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://bwx.sweek.top

Java: catch (IOException | SQLException e) {}
来源：http://epg.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qrd.gogol.net.cn

Ruby: rescue ArgumentError => e
来源：http://oul.ppjwa.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ssf.iojbl.cn

[H06] 可选值 / 空值安全访问
来源：http://nxg.wangdashe.top

Py:   value = d.get("k") or default
来源：http://vzf.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://jmr.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://tal.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://toe.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gws.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ajk.xylfe.cn

Ruby: d&.dig(:a, :b)
来源：http://wwb.yvedp.cn

C#:   obj?.A?.B ?? default
来源：http://ehv.shanyushiyangkeji.top

[H07] 断言
来源：http://yhw.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://kkz.chenzaomai.com

PHP:  assert($x > 0);
来源：http://kuc.fengsongda.top

JS:   console.assert(x > 0);
来源：http://ogq.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://tmk.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://cam.tanke756.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bfn.zhoulong.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://joy.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://zne.hnxiangtu.top

[H08] 获取错误信息与堆栈
来源：http://uxk.sufxvd.cn

Py:   str(e);  traceback.format_exc()
来源：http://kyy.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cgu.fehbvm.com


<!-- 参考信息 -->