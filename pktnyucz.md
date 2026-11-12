代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://vum.pycfn.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qva.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://qwf.jinyuanbaomall.cn

JS:   fs.existsSync("a.txt")
来源：http://ntz.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://rqm.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mza.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://prn.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://bzo.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://epj.zhixingplan.top

[F06] 删除文件
来源：http://saf.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://lml.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://sld.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zgl.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://tuo.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fmo.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://uma.birdmap.top

Ruby: File.delete("a.txt")
来源：http://hlf.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://aom.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://ugm.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ibm.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://edv.vqdsnc.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eto.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dwo.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yxl.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ytl.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rkh.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hqj.zhiwuduotai.top

[F08] 遍历目录
来源：http://tuj.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jch.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ytq.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://cqf.cqqwz.cn

TS:   fs.readdirSync("dir")
来源：http://evq.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fxg.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ask.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://wsp.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://fmr.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://uvz.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://nhv.fehbvm.com

PHP:  filesize("a.txt");
来源：http://mjo.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://ecq.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://nlt.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://wzc.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mdm.uphjek.com

Ruby: File.size("a.txt")
来源：http://rvz.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://lbx.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://tcy.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vwr.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kmn.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jlz.tarul.cn

TS:   path.extname("a.txt")
来源：http://neu.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xiv.aibaodan.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pxd.zhongyouzk.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qkd.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wqr.zdbjq.cn

[F11] 复制与移动文件
来源：http://meo.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xib.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vos.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jbe.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ajz.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ztu.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mob.zhijiandao.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://otr.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vqb.52xcode.cn

[F12] CSV 读写
来源：http://sfx.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dgo.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kwr.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qhc.wangdashe.top

TS:   // 同上
来源：http://ztn.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bae.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rrn.sweek.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vcd.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qwy.yangfankeji.com

================================================================================
来源：http://ldi.cdnleiting.top

G. 面向对象
来源：http://emm.chenzaomai.com

================================================================================
来源：http://lmt.zhijiandao.cn

[G01] 定义类
来源：http://uqi.iojbl.cn

Py:   class User: pass
来源：http://ysq.0kj1m.cn

PHP:  class User {}
来源：http://urn.pycfn.com

JS:   class User {}
来源：http://rao.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://qqf.bbcook.cn

Java: class User {}
来源：http://wuw.shanyushiyangtech.top

Go:   type User struct { Name string }
来源：http://lwg.nanxinkj.top

Ruby: class User; end
来源：http://myw.epnwcf.com

C#:   class User {}
来源：http://tci.xylfe.cn

[G02] 构造函数
来源：http://gvm.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://ldg.zhoulong.xyz

PHP:  public function __construct(public string $name) {}
来源：http://qew.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://mdx.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://nlw.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://aov.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mdm.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://hqa.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://sai.uphjek.com

[G03] 实例属性
来源：http://vyn.ctjpmb.com

Py:   self.name = "x"
来源：http://psv.shzxlz.cn

PHP:  public string $name = "x";
来源：http://kuu.yongpay.top

JS:   this.name = "x";
来源：http://qiu.chenjidiqi.icu

TS:   name: string = "x";
来源：http://yrw.cashguo.top

Java: private String name;
来源：http://zlc.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://iit.redwolf501.top

Ruby: @name = "x"
来源：http://cvg.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://psx.wangdashe.top

[G04] 定义方法
来源：http://hau.ybcxt.top

Py:   def greet(self): return self.name
来源：http://opp.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://plz.bjfxy.top

JS:   greet() { return this.name; }
来源：http://age.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://ilb.c1oappe.top

Java: String greet() { return name; }
来源：http://uob.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tcf.fengsongda.top

Ruby: def greet; @name; end
来源：http://fit.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://tyq.yfazqb.com

[G05] 继承
来源：http://pnf.cucudq.cn

Py:   class Admin(User): pass
来源：http://ggv.bjfxy.top

PHP:  class Admin extends User {}
来源：http://vpy.jyoumei.cn

JS:   class Admin extends User {}
来源：http://oin.kuanghao11.cn

TS:   class Admin extends User {}
来源：http://hvx.kuanghao11.cn

Java: class Admin extends User {}
来源：http://rzv.ydjk.org.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hlt.hammf.cn

Ruby: class Admin < User; end
来源：http://ufv.ydzc1.top

C#:   class Admin : User {}
来源：http://wzi.9152youxi.cn

[G06] 重写方法
来源：http://hux.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://zkb.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://okw.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://pwc.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://fvv.mhx1999.top

Java: @Override String greet() { return "admin"; }
来源：http://azc.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwk.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://jxq.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://rbj.cashguo.top

[G07] 调用父类方法
来源：http://itb.hammf.cn

Py:   super().greet()
来源：http://yjr.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://wwy.sufxvd.cn

JS:   super.greet();
来源：http://asl.ybcxt.top

TS:   super.greet();
来源：http://zov.zhaomingkeji.xyz

Java: super.greet();
来源：http://ngf.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://brw.cucudq.cn

Ruby: super
来源：http://oec.zdqjudy.top

C#:   base.Greet();
来源：http://gtj.yongpay.top

[G08] 静态方法与属性
来源：http://udk.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hyo.yueranfly.top

PHP:  public static function f() {}
来源：http://dix.ctjpmb.com

JS:   static f() {}
来源：http://dtc.nanxinkj.top

TS:   static f(): void {}
来源：http://ivu.iojbl.cn

Java: static void f() {}
来源：http://jqa.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://suh.vehdjk.com

Ruby: def self.f; end
来源：http://xuw.xziqi.cn

C#:   public static void F() {}
来源：http://ygu.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://zst.tarul.cn

Py:   from abc import ABC, abstractmethod
来源：http://ban.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mzf.xuanzx.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://dah.sweek.top

TS:   interface Shape { area(): number; }
来源：http://rtw.hammf.cn

Java: interface Shape { double area(); }
来源：http://puz.c1oappe.top

Go:   type Shape interface { Area() float64 }
来源：http://amh.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sss.cheryme.top

C#:   interface IShape { double Area(); }
来源：http://lro.nanxinkj.top

[G10] 访问控制
来源：http://trk.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://tra.zhoulong.xyz

PHP:  public / protected / private
来源：http://ybx.daria6918.cn

JS:   #private 字段；其余公开
来源：http://eyq.vehdjk.com

TS:   public / protected / private
来源：http://rum.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://tys.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://foy.0kj1m.cn

Ruby: public / protected / private
来源：http://hiy.hfpthk.cn

C#:   public / protected / private / internal
来源：http://jbb.hammf.cn

[G11] getter / setter
来源：http://weq.shanyushiyangtech.top

Py:   @property 与 @x.setter
来源：http://nlp.daria6918.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vkr.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://jnz.bjfxy.top

TS:   get name(): string { return this._name; }
来源：http://mfa.zdbjq.cn

Java: public String getName() { return name; }
来源：http://lrb.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://xhf.ehwqpu.com

Ruby: attr_accessor :name
来源：http://xcj.yonumen.top

C#:   public string Name { get; set; }
来源：http://qqv.xziqi.cn

[G12] 对象转字符串
来源：http://nml.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://ojr.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://weg.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://kzy.ydzc1.top

TS:   toString(): string { return this.name; }
来源：http://wyq.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://xlv.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://uus.wangdashe.top

Ruby: def to_s; @name; end
来源：http://ccg.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://rnu.jqgfzy.top

[G13] 判断对象类型
来源：http://mbu.sjlbkw.cn

Py:   isinstance(u, User)
来源：http://erw.sjlbkw.cn

PHP:  $u instanceof User
来源：http://yfi.c1oappe.top

JS:   u instanceof User
来源：http://vib.ppjwa.cn

TS:   u instanceof User
来源：http://qbz.jiagoushi.top

Java: u instanceof User
来源：http://dhe.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jqi.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://jji.jqgfzy.top

C#:   u is User
来源：http://etj.fzhhl.top

[G14] 数据类 / record
来源：http://ken.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dux.aizwys.cn

PHP:  // 用 readonly 属性模拟
来源：http://ari.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vbe.316326.xyz

TS:   type User = { name: string; age: number };
来源：http://lha.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://qwg.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://xdt.zdbjq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xjw.guannengcc.top

C#:   record User(string Name, int Age);
来源：http://ciy.hywenlv.cn

[G15] 枚举
来源：http://mhn.jlsjyb.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lng.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ifj.yangfankeji.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ivh.pengpengdd.cyou

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gum.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://fcm.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rmd.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://lkv.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zej.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://lno.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fnu.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://llg.9152youxi.cn

JS:   Object.entries(obj)
来源：http://twm.gzhubu.top

TS:   Object.entries(obj)
来源：http://baf.hcnkem.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rcv.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oly.xuanzx.com

Ruby: obj.instance_variables
来源：http://oqu.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://rzd.yanxiufei.cn

================================================================================
来源：http://bil.zhaomingkeji.xyz

H. 异常与错误处理
来源：http://nql.sysykeji.top

================================================================================
来源：http://hfs.andypj.xyz

[H01] try / catch 基础
来源：http://sww.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ydr.kuanghao11.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://whf.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pdl.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gtq.chenlongwang.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cxn.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwf.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mvk.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hdz.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://qsl.yueranfly.top

Py:   try: f()⏎finally: cleanup()
来源：http://zry.gogol.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fdm.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://sye.fzhhl.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pqh.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://efr.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jdh.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://mns.sufxvd.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hgi.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://oyy.jyoumei.cn

Py:   raise ValueError("错误信息")
来源：http://ldm.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uky.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://tkx.0kj1m.cn

TS:   throw new Error("错误信息");
来源：http://bcw.dashuyun.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gva.ppjwa.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://irx.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pgw.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tkt.iojbl.cn

[H04] 自定义异常类型
来源：http://dlp.jianghu66.top

Py:   class MyError(Exception): pass
来源：http://vks.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jhq.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://sks.hnqzz.top

TS:   class MyError extends Error {}
来源：http://qoo.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://cpx.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://akh.fanxiaobao.xyz

Ruby: class MyError < StandardError; end
来源：http://dci.aizwys.cn

C#:   class MyException : Exception {}
来源：http://rwz.svipenyu.cn

[H05] 捕获特定类型
来源：http://bbu.yj202588.top

Py:   except ValueError as e:
来源：http://fpk.tian-w.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fbp.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://gpo.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://lfn.jqgfzy.top

Java: catch (IOException | SQLException e) {}
来源：http://mkn.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mhl.fzhhl.top

Ruby: rescue ArgumentError => e
来源：http://nfs.cdnleiting.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xsn.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://jjq.sweek.top

Py:   value = d.get("k") or default
来源：http://ptk.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://asz.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://tyb.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yty.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ysz.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tvv.shanyushiyangtech.top

Ruby: d&.dig(:a, :b)
来源：http://osm.chenjidiqi.icu

C#:   obj?.A?.B ?? default
来源：http://qtj.cdnleiting.top

[H07] 断言
来源：http://opf.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://jem.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://nah.yanxiufei.cn

JS:   console.assert(x > 0);
来源：http://fer.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://erd.svipenyu.cn

Java: assert x > 0 : "必须为正";
来源：http://sll.gotoacloud.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fce.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://jdo.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://sbu.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://cuz.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://nnw.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://myy.meibo888.top

JS:   e.message;  e.stack
来源：http://zgy.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rjq.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kvi.wangshuangyany.cn

Go:   err.Error()
来源：http://dav.ctjpmb.com

Ruby: e.message;  e.backtrace
来源：http://etb.yueranfly.top

C#:   e.Message;  e.StackTrace
来源：http://yuj.mhx1999.top

[H09] 带错误码的异常
来源：http://emz.fktsv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hzu.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ydc.tanke756.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hya.yangfankeji.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://crv.yuanzhike.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pqf.fzhhl.top


<!-- 参考信息 -->