代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://swc.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ubd.zhongyouzk.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lnx.jianghu66.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qpw.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tdo.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rmc.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rsw.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://may.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://lhd.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://naj.quarkkingdee.top

PHP:  file_exists("a.txt");
来源：http://cii.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://eaz.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://ljy.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pod.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ziq.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://qao.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://auh.sysykeji.top

[F06] 删除文件
来源：http://fag.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://tjc.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://vmb.zdbjq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nwe.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dmp.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqs.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://tcv.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://apx.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://yhn.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://zzn.cqqwz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pyf.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ify.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyj.xuetiantiany.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cac.tian-w.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://svx.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pxp.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://khw.fengsongda.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sjk.fktsv.cn

[F08] 遍历目录
来源：http://fzo.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://sot.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wzh.birdmap.top

JS:   fs.readdirSync("dir")
来源：http://rco.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://zle.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://spq.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kub.jianghu66.top

Ruby: Dir.children("dir")
来源：http://ryg.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://gkk.shzxlz.cn

[F09] 获取文件大小
来源：http://kvh.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://ndm.uphjek.com

PHP:  filesize("a.txt");
来源：http://ufy.zhijiandao.cn

JS:   fs.statSync("a.txt").size
来源：http://gan.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://ilj.yueranfly.top

Java: Files.size(Path.of("a.txt"))
来源：http://gke.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://huo.hnqzz.top

Ruby: File.size("a.txt")
来源：http://vei.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://uik.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://evq.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kxk.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xjg.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hjc.yangfankeji.com

TS:   path.extname("a.txt")
来源：http://gob.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wig.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jnk.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iuw.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kev.mhx1999.top

[F11] 复制与移动文件
来源：http://ana.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nyn.vqdsnc.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bfj.c1oappe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://poe.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wei.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mmo.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tuy.ywan-chungtsiang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vwu.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lom.0kj1m.cn

[F12] CSV 读写
来源：http://plw.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hzz.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iqi.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://chd.haohaochexian.top

TS:   // 同上
来源：http://tfb.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rks.cheryme.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mrj.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lrw.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://kfz.jiagoushi.top

================================================================================
来源：http://bnf.pengpengdd.cyou

G. 面向对象
来源：http://fli.hnxiangtu.top

================================================================================
来源：http://pus.9152youxi.cn

[G01] 定义类
来源：http://que.zhengqikj.top

Py:   class User: pass
来源：http://iuh.ppjwa.cn

PHP:  class User {}
来源：http://vcs.sysykeji.top

JS:   class User {}
来源：http://ymx.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://ffo.jinyuanbaomall.cn

Java: class User {}
来源：http://xfe.sufxvd.cn

Go:   type User struct { Name string }
来源：http://nak.ybcxt.top

Ruby: class User; end
来源：http://thv.zhaomingkeji.xyz

C#:   class User {}
来源：http://qeg.shuidangran.top

[G02] 构造函数
来源：http://ccf.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://tdb.meibo888.top

PHP:  public function __construct(public string $name) {}
来源：http://yqb.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://bhe.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://cmo.0kj1m.cn

Java: User(String name) { this.name = name; }
来源：http://cny.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lhn.tarul.cn

Ruby: def initialize(name); @name = name; end
来源：http://eyi.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://tcd.fengsongda.top

[G03] 实例属性
来源：http://nmo.dianchejie.cn

Py:   self.name = "x"
来源：http://orn.ybcxt.top

PHP:  public string $name = "x";
来源：http://usc.52xcode.cn

JS:   this.name = "x";
来源：http://iyo.ppjwa.cn

TS:   name: string = "x";
来源：http://xdz.hongshengwenyu.top

Java: private String name;
来源：http://pez.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ouv.yj20258.top

Ruby: @name = "x"
来源：http://giv.tian-w.cn

C#:   public string Name { get; set; } = "x";
来源：http://fud.yangfankeji.com

[G04] 定义方法
来源：http://ptj.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://qhk.ywan-chungtsiang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cms.ywan-chungtsiang.top

JS:   greet() { return this.name; }
来源：http://nym.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://cqa.sjlbkw.cn

Java: String greet() { return name; }
来源：http://jyg.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jvy.havefunace.top

Ruby: def greet; @name; end
来源：http://qjr.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://xel.yanxiufei.cn

[G05] 继承
来源：http://dbz.jyoumei.cn

Py:   class Admin(User): pass
来源：http://pfx.hcnkem.com

PHP:  class Admin extends User {}
来源：http://ldq.zhengqikj.top

JS:   class Admin extends User {}
来源：http://wxv.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://nwk.0kj1m.cn

Java: class Admin extends User {}
来源：http://doj.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isb.hfpthk.cn

Ruby: class Admin < User; end
来源：http://hxq.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://qcw.cqqwz.cn

[G06] 重写方法
来源：http://ifx.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://cng.jyoumei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wpz.pycfn.com

JS:   greet() { return "admin"; }
来源：http://uih.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://xlk.quarkkingdee.top

Java: @Override String greet() { return "admin"; }
来源：http://zrq.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gel.jyoumei.cn

Ruby: def greet; "admin"; end
来源：http://wgw.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://bxq.hywenlv.cn

[G07] 调用父类方法
来源：http://mmb.jqgfzy.top

Py:   super().greet()
来源：http://brw.epnwcf.com

PHP:  parent::greet();
来源：http://pdk.yfazqb.com

JS:   super.greet();
来源：http://pkt.gogol.net.cn

TS:   super.greet();
来源：http://jhu.shangyingyoupin.top

Java: super.greet();
来源：http://eup.ybcxt.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://npg.jlsjyb.cn

Ruby: super
来源：http://fpc.52xcode.cn

C#:   base.Greet();
来源：http://seh.cheryme.top

[G08] 静态方法与属性
来源：http://ecq.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rjm.tanke756.top

PHP:  public static function f() {}
来源：http://cks.jlsjyb.cn

JS:   static f() {}
来源：http://siq.shzxlz.cn

TS:   static f(): void {}
来源：http://xgr.gogol.net.cn

Java: static void f() {}
来源：http://bzq.hcnkem.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://flk.yj20258.top

Ruby: def self.f; end
来源：http://rmj.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://rah.bjfxy.top

[G09] 接口 / 抽象类
来源：http://vgm.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://czy.xylfe.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rzr.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://cta.c1oappe.top

TS:   interface Shape { area(): number; }
来源：http://eyr.fehbvm.com

Java: interface Shape { double area(); }
来源：http://lzs.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://bqq.pengpengdd.cyou

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ene.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://cjq.cashguo.top

[G10] 访问控制
来源：http://svu.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://lpo.iojbl.cn

PHP:  public / protected / private
来源：http://cyx.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://bgt.wangshuangyany.cn

TS:   public / protected / private
来源：http://avm.kuanghao11.cn

Java: public / protected / private / 默认包级
来源：http://wzp.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://iui.zdqjudy.top

Ruby: public / protected / private
来源：http://qvc.mhx1999.top

C#:   public / protected / private / internal
来源：http://tgi.sjlbkw.cn

[G11] getter / setter
来源：http://pqf.yj202588.top

Py:   @property 与 @x.setter
来源：http://xmr.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xuy.tarul.cn

JS:   get name() { return this._name; }
来源：http://vdz.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://xev.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://duj.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://poa.shanyushiyangkeji.top

Ruby: attr_accessor :name
来源：http://btq.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://dzz.ctjpmb.com

[G12] 对象转字符串
来源：http://ekg.andypj.xyz

Py:   def __str__(self): return self.name
来源：http://wzy.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jxa.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://qxu.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://qdf.daria6918.cn

Java: @Override public String toString() { return name; }
来源：http://oeh.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://edj.iojbl.cn

Ruby: def to_s; @name; end
来源：http://orj.9152youxi.cn

C#:   public override string ToString() => Name;
来源：http://ihc.aibaodan.cn

[G13] 判断对象类型
来源：http://tpq.chenzaomai.com

Py:   isinstance(u, User)
来源：http://mnn.52xcode.cn

PHP:  $u instanceof User
来源：http://zbm.andypj.xyz

JS:   u instanceof User
来源：http://hdg.hysaishi.cn

TS:   u instanceof User
来源：http://nqr.xuanzx.com

Java: u instanceof User
来源：http://ecx.uphjek.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://nth.andypj.xyz

Ruby: u.is_a?(User)
来源：http://mnb.52xcode.cn

C#:   u is User
来源：http://llm.aizwys.cn

[G14] 数据类 / record
来源：http://omm.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gti.hongshengwenyu.top

PHP:  // 用 readonly 属性模拟
来源：http://gzq.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://jrr.shangyingyoupin.top

TS:   type User = { name: string; age: number };
来源：http://mrm.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://sue.ywan-chungtsiang.top

Go:   type User struct { Name string; Age int }
来源：http://tpy.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zzz.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://lxy.xuanzx.com

[G15] 枚举
来源：http://yfk.jinqigfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cjn.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gny.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwm.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qpq.hcnkem.com

Java: enum Color { RED, GREEN }
来源：http://hod.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://utf.hnqzz.top

Ruby: Color = %i[red green].freeze
来源：http://zbv.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://crv.yj20258888.top

[G16] 对象转数组 / 字典
来源：http://pgs.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vrn.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://pki.vehdjk.com

JS:   Object.entries(obj)
来源：http://ugu.dashuyun.cn

TS:   Object.entries(obj)
来源：http://zis.hywenlv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://aru.shanyushiyangtech.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ksq.hnxiangtu.top

Ruby: obj.instance_variables
来源：http://vcd.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://fuh.yj20258.top

================================================================================
来源：http://ugg.snrcjt.cn

H. 异常与错误处理
来源：http://pyu.fanxiaobao.xyz

================================================================================
来源：http://qui.jinqigufen.top

[H01] try / catch 基础
来源：http://uzg.sysykeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fgh.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ato.iojbl.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ozu.ydzc1.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tcg.yfazqb.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uxr.yanxiufei.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yrm.fehbvm.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zej.sufxvd.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sfy.sxryk.cn

[H02] finally / ensure 收尾
来源：http://tow.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://plv.svipenyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://evk.xingfuxueyuan.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://hhx.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jpt.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://llk.cucudq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://plv.sjlbkw.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wfy.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wyl.jinghuilouyu.cn

[H03] 主动抛出异常
来源：http://ttr.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://ugp.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dsj.hnxiangtu.top

JS:   throw new Error("错误信息");
来源：http://iga.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://ghv.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jkr.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ykp.hesvh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://meu.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kli.zhijiandao.cn

[H04] 自定义异常类型
来源：http://yck.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://dzi.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cnw.tarul.cn

JS:   class MyError extends Error {}
来源：http://uni.0kj1m.cn

TS:   class MyError extends Error {}
来源：http://spi.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://sat.dashuyun.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bbf.shangyingyoupin.top

Ruby: class MyError < StandardError; end
来源：http://iwa.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://sve.jqgfzy.top

[H05] 捕获特定类型
来源：http://pxp.aizwys.cn

Py:   except ValueError as e:
来源：http://ezn.cdnleiting.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ieb.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://tkt.jqgufenzy.top

TS:   if (e instanceof TypeError) {}
来源：http://cbh.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://lqk.jianghu66.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bcy.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://kok.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gvl.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://ehd.redwolf501.top

Py:   value = d.get("k") or default
来源：http://tdj.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lca.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://lik.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://etf.sxryk.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nzj.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wzi.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://zhj.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://kio.quarkkingdee.top

[H07] 断言
来源：http://tik.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://rhp.ppjwa.cn

PHP:  assert($x > 0);
来源：http://kid.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://lxl.smart0.xyz

TS:   console.assert(x > 0);
来源：http://mqk.nwbrower.top

Java: assert x > 0 : "必须为正";
来源：http://cqb.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://owk.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fhj.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://hrp.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://pae.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://xyn.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ucb.wangdashe.top

JS:   e.message;  e.stack
来源：http://mhz.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ota.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ciy.jlsjyb.cn

Go:   err.Error()
来源：http://mdh.hfpthk.cn


<!-- 参考信息 -->