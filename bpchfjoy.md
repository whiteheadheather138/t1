代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hmu.xylfe.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vdr.zdbjq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jmz.daria6918.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wte.fengsongda.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gae.jianghu66.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gpy.quarkkingdee.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lhf.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xfs.birdmap.top

[F05] 判断文件或目录是否存在
来源：http://ghd.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rnl.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://dnn.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://ltx.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://jfx.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://skb.cheryme.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qop.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://mqe.hfpthk.cn

C#:   File.Exists("a.txt")
来源：http://zrl.cqqwz.cn

[F06] 删除文件
来源：http://pfw.yj20258.top

Py:   os.remove("a.txt")
来源：http://omk.feifeiyinyue.top

PHP:  unlink("a.txt");
来源：http://riu.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zwf.fktsv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rik.jinqigufen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://idi.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://tma.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://isk.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://joq.sxryk.cn

[F07] 创建目录（含多级）
来源：http://huo.jinqigfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uxt.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vob.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ljr.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gpr.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://csd.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gmo.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iup.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pqv.smart0.xyz

[F08] 遍历目录
来源：http://xkq.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xva.xuetiantiany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ckx.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://nik.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://fek.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fle.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lol.tianlin.xyz

Ruby: Dir.children("dir")
来源：http://vbi.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://rkz.jinqigufen.top

[F09] 获取文件大小
来源：http://pnj.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://ifb.yj20258888.top

PHP:  filesize("a.txt");
来源：http://fzs.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://kdw.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://pgw.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://prg.gotoacloud.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pix.guannengcc.top

Ruby: File.size("a.txt")
来源：http://ydu.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://sdb.0kj1m.cn

[F10] 取文件扩展名 / 文件名
来源：http://nba.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sza.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vyb.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://owo.tanke756.top

TS:   path.extname("a.txt")
来源：http://yte.316326.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cie.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dew.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hgr.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jwe.uphjek.com

[F11] 复制与移动文件
来源：http://ges.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ldb.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tnk.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gef.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sin.cucudq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fae.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mne.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gvu.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://agu.ctjpmb.com

[F12] CSV 读写
来源：http://kda.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zku.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uks.smart0.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bsh.yuanzhike.top

TS:   // 同上
来源：http://wxb.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://omj.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qil.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nuf.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yor.pengpengdd.cyou

================================================================================
来源：http://oap.jqgfzy.top

G. 面向对象
来源：http://pdt.meibo888.top

================================================================================
来源：http://upa.ybcxt.top

[G01] 定义类
来源：http://jbw.yuanzhike.top

Py:   class User: pass
来源：http://age.gzhubu.top

PHP:  class User {}
来源：http://ehp.xuetiantiany.cn

JS:   class User {}
来源：http://jrp.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://rpz.jianghu66.top

Java: class User {}
来源：http://art.jinyuanbaomall.cn

Go:   type User struct { Name string }
来源：http://brj.jlsjyb.cn

Ruby: class User; end
来源：http://ssp.yj20258888.top

C#:   class User {}
来源：http://vjq.aibaodan.cn

[G02] 构造函数
来源：http://rts.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://czs.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://nkp.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://jzb.316326.xyz

TS:   constructor(public name: string) {}
来源：http://qsv.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://cqz.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vhr.birdmap.top

Ruby: def initialize(name); @name = name; end
来源：http://dce.yonumen.top

C#:   public User(string name) { Name = name; }
来源：http://dst.hnqzz.top

[G03] 实例属性
来源：http://axm.0kj1m.cn

Py:   self.name = "x"
来源：http://beb.svipenyu.cn

PHP:  public string $name = "x";
来源：http://uka.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://ati.meibo888.top

TS:   name: string = "x";
来源：http://ige.redwolf501.top

Java: private String name;
来源：http://uqh.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fas.birdmap.top

Ruby: @name = "x"
来源：http://qne.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://mzc.jlsjyb.cn

[G04] 定义方法
来源：http://nbx.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://gui.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tqb.aizwys.cn

JS:   greet() { return this.name; }
来源：http://nik.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://dpq.ybcxt.top

Java: String greet() { return name; }
来源：http://aqw.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://bje.svipenyu.cn

Ruby: def greet; @name; end
来源：http://vma.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://zri.zhongyouzk.top

[G05] 继承
来源：http://mwt.daxiang520.top

Py:   class Admin(User): pass
来源：http://jln.c1oappe.top

PHP:  class Admin extends User {}
来源：http://fqw.gogol.net.cn

JS:   class Admin extends User {}
来源：http://raw.uphjek.com

TS:   class Admin extends User {}
来源：http://cxc.zdbjq.cn

Java: class Admin extends User {}
来源：http://vnz.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gun.chenzaomai.com

Ruby: class Admin < User; end
来源：http://rpn.hfpthk.cn

C#:   class Admin : User {}
来源：http://mmo.sufxvd.cn

[G06] 重写方法
来源：http://fsw.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://msl.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hkc.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://uwk.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://vgg.chenzaomai.com

Java: @Override String greet() { return "admin"; }
来源：http://ncv.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pqm.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://bua.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://jfh.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://nft.fzhhl.top

Py:   super().greet()
来源：http://oyf.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://dje.hesvh.cn

JS:   super.greet();
来源：http://msg.sxryk.cn

TS:   super.greet();
来源：http://oaa.pycfn.com

Java: super.greet();
来源：http://pve.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vas.yonumen.top

Ruby: super
来源：http://hvq.guannengcc.top

C#:   base.Greet();
来源：http://agq.kuanghao11.cn

[G08] 静态方法与属性
来源：http://tsa.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xhs.haohaochexian.top

PHP:  public static function f() {}
来源：http://wtc.hesvh.cn

JS:   static f() {}
来源：http://cqk.gogol.net.cn

TS:   static f(): void {}
来源：http://mfy.hnxiangtu.top

Java: static void f() {}
来源：http://mfu.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bkx.nanxuanxn.top

Ruby: def self.f; end
来源：http://lqc.smart0.xyz

C#:   public static void F() {}
来源：http://wdt.yj202588.top

[G09] 接口 / 抽象类
来源：http://htj.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://quu.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ake.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sse.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://tmr.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://bca.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://evk.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nls.hnqzz.top

C#:   interface IShape { double Area(); }
来源：http://uto.fehbvm.com

[G10] 访问控制
来源：http://svl.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://kyh.hysaishi.cn

PHP:  public / protected / private
来源：http://qys.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://bqu.haohaochexian.top

TS:   public / protected / private
来源：http://nma.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://bbe.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://psa.hesvh.cn

Ruby: public / protected / private
来源：http://fpo.yonumen.top

C#:   public / protected / private / internal
来源：http://xor.pycfn.com

[G11] getter / setter
来源：http://ggw.c1oappe.top

Py:   @property 与 @x.setter
来源：http://ixt.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rya.gzhubu.top

JS:   get name() { return this._name; }
来源：http://krd.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://wcs.xinyue.icu

Java: public String getName() { return name; }
来源：http://ejs.sufxvd.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zat.zhongyouzk.top

Ruby: attr_accessor :name
来源：http://shb.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://mhg.yuanzhike.top

[G12] 对象转字符串
来源：http://xjx.uphjek.com

Py:   def __str__(self): return self.name
来源：http://cjo.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://trs.aizwys.cn

JS:   toString() { return this.name; }
来源：http://qao.zhaomingkeji.xyz

TS:   toString(): string { return this.name; }
来源：http://zkl.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://rmk.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://jfx.sxryk.cn

Ruby: def to_s; @name; end
来源：http://bld.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://gph.zhoulong.xyz

[G13] 判断对象类型
来源：http://maw.uphjek.com

Py:   isinstance(u, User)
来源：http://yhf.yj202588.top

PHP:  $u instanceof User
来源：http://weg.sufxvd.cn

JS:   u instanceof User
来源：http://wbq.hongshengwenyu.top

TS:   u instanceof User
来源：http://tyz.xuetiantiany.cn

Java: u instanceof User
来源：http://jcm.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://hxs.yfazqb.com

Ruby: u.is_a?(User)
来源：http://wuo.zhaomingkeji.xyz

C#:   u is User
来源：http://kjl.aizwys.cn

[G14] 数据类 / record
来源：http://ile.xziqi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://csf.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://boa.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://izk.uphjek.com

TS:   type User = { name: string; age: number };
来源：http://nqs.yangfankeji.com

Java: record User(String name, int age) {}
来源：http://vsm.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://ull.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qkf.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://jmf.yj202588.top

[G15] 枚举
来源：http://hpp.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pft.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufd.epnwcf.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ukk.snrcjt.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://brk.hnqzz.top

Java: enum Color { RED, GREEN }
来源：http://upt.zhiwuduotai.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xyy.hongshengwenyu.top

Ruby: Color = %i[red green].freeze
来源：http://okf.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hvt.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://rmm.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wmj.zhaomingkeji.xyz

PHP:  get_object_vars($obj);
来源：http://uev.svipenyu.cn

JS:   Object.entries(obj)
来源：http://jae.yvedp.cn

TS:   Object.entries(obj)
来源：http://cqk.cqqwz.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rea.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vxg.sweek.top

Ruby: obj.instance_variables
来源：http://pwg.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://scd.uphjek.com

================================================================================
来源：http://sdj.hysaishi.cn

H. 异常与错误处理
来源：http://lmy.daria6918.cn

================================================================================
来源：http://end.sxryk.cn

[H01] try / catch 基础
来源：http://ksc.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ckw.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fiu.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hpj.shanyushiyangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mgr.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ihh.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hgp.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://foc.chenlongwang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://beq.smart0.xyz

[H02] finally / ensure 收尾
来源：http://qgu.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://sqn.jqgufenzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dly.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xaq.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://mkz.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://zgg.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://mvq.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://tiz.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://srl.sysykeji.top

[H03] 主动抛出异常
来源：http://yas.c1oappe.top

Py:   raise ValueError("错误信息")
来源：http://ocu.hammf.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xjr.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://nnr.xingfuxueyuan.xyz

TS:   throw new Error("错误信息");
来源：http://ocf.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gbd.jinqigfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bfj.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://koz.bbcook.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sbk.hnxiangtu.top

[H04] 自定义异常类型
来源：http://nzi.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://mkx.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vvs.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://mrh.ybcxt.top

TS:   class MyError extends Error {}
来源：http://mdv.aizwys.cn

Java: class MyException extends RuntimeException {}
来源：http://kah.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nen.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://dmw.xuanzx.com

C#:   class MyException : Exception {}
来源：http://nuw.tianlin.xyz

[H05] 捕获特定类型
来源：http://tzc.pycfn.com

Py:   except ValueError as e:
来源：http://nmz.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lfx.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://pwl.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://kje.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://dot.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bpv.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://nej.fengsongda.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kok.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://aap.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://chy.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://vvr.iojbl.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oim.yvedp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zqr.gogol.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nvm.xinyue.icu

Go:   if v, ok := m["k"]; ok { }
来源：http://apf.cqqwz.cn

Ruby: d&.dig(:a, :b)
来源：http://oje.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://lct.pycfn.com

[H07] 断言
来源：http://mfe.fktsv.cn

Py:   assert x > 0, "必须为正"
来源：http://cgj.zhoulong.xyz

PHP:  assert($x > 0);
来源：http://jvd.fzhhl.top

JS:   console.assert(x > 0);
来源：http://isu.ppjwa.cn

TS:   console.assert(x > 0);
来源：http://nqn.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://chi.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bjs.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://ezi.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://zcv.sysykeji.top

[H08] 获取错误信息与堆栈
来源：http://yxl.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://yts.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://htx.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://nzq.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uyr.yanxiufei.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ahs.yj20258888.top

Go:   err.Error()
来源：http://iwz.andypj.xyz


<!-- 参考信息 -->