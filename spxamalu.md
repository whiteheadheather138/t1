代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://put.xylfe.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yjv.yj202588.top

PHP:  file_exists("a.txt");
来源：http://ppx.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://dhu.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://qvb.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kzk.c1oappe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ocb.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://nhy.ctjpmb.com

C#:   File.Exists("a.txt")
来源：http://jnb.bjfxy.top

[F06] 删除文件
来源：http://nxx.xinyue.icu

Py:   os.remove("a.txt")
来源：http://bro.xziqi.cn

PHP:  unlink("a.txt");
来源：http://kby.mhx1999.top

JS:   fs.unlinkSync("a.txt")
来源：http://wyp.jqgufenzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://xxz.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://whr.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://rzn.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://gzi.guowangkeji.top

C#:   File.Delete("a.txt");
来源：http://rpy.sjlbkw.cn

[F07] 创建目录（含多级）
来源：http://gqy.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mng.sweek.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oma.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vzr.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://scv.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://laz.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ilb.xylfe.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ypu.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fht.fengsongda.top

[F08] 遍历目录
来源：http://efy.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://eoj.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lql.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://ica.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://fbo.zhoulong.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abc.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://eca.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://muy.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://oof.guannengcc.top

[F09] 获取文件大小
来源：http://ufq.c1oappe.top

Py:   os.path.getsize("a.txt")
来源：http://vnr.pengpengdd.cyou

PHP:  filesize("a.txt");
来源：http://hoo.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://rab.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://jiz.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vyo.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://neh.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://aui.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://wca.nwbrower.top

[F10] 取文件扩展名 / 文件名
来源：http://mcj.tanke756.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ulq.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mes.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dan.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://aho.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xhr.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wsd.yj20258888.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vlh.nanxuanxn.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sbu.daxiang520.top

[F11] 复制与移动文件
来源：http://hii.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pmy.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://huv.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://enq.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ttz.jiagoushi.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://phv.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pfo.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eto.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://psy.redwolf501.top

[F12] CSV 读写
来源：http://lne.iojbl.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://szt.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://eew.cucudq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tzm.tarul.cn

TS:   // 同上
来源：http://vcf.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lku.zhongyouzk.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ubu.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://frj.tianlin.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://flx.sweek.top

================================================================================
来源：http://ulz.andypj.xyz

G. 面向对象
来源：http://uar.hesvh.cn

================================================================================
来源：http://xwg.cucudq.cn

[G01] 定义类
来源：http://zky.shanyushiyangtech.top

Py:   class User: pass
来源：http://mua.jinqigufen.top

PHP:  class User {}
来源：http://ymp.daria6918.cn

JS:   class User {}
来源：http://yzm.havefunace.top

TS:   class User { name: string = ""; }
来源：http://dbm.dashuyun.cn

Java: class User {}
来源：http://tei.cqqwz.cn

Go:   type User struct { Name string }
来源：http://iac.chenzaomai.com

Ruby: class User; end
来源：http://ani.meibo888.top

C#:   class User {}
来源：http://rqj.havefunace.top

[G02] 构造函数
来源：http://wxh.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://vkr.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://tbi.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://efg.dianchejie.cn

TS:   constructor(public name: string) {}
来源：http://xep.yj20258888.top

Java: User(String name) { this.name = name; }
来源：http://yhg.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zay.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://bvk.epnwcf.com

C#:   public User(string name) { Name = name; }
来源：http://iea.epnwcf.com

[G03] 实例属性
来源：http://qji.hcnkem.com

Py:   self.name = "x"
来源：http://aqd.gzhubu.top

PHP:  public string $name = "x";
来源：http://lfk.jqgufenzy.top

JS:   this.name = "x";
来源：http://fbb.shangyingyoupin.top

TS:   name: string = "x";
来源：http://cay.zhaomingkeji.xyz

Java: private String name;
来源：http://uqk.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xuk.aibaodan.cn

Ruby: @name = "x"
来源：http://jeu.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://veb.yangfankeji.com

[G04] 定义方法
来源：http://ggz.fktsv.cn

Py:   def greet(self): return self.name
来源：http://rwc.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://rph.nwbrower.top

JS:   greet() { return this.name; }
来源：http://ztd.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://ero.ctjpmb.com

Java: String greet() { return name; }
来源：http://qcs.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://die.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://ecb.ybcxt.top

C#:   public string Greet() => Name;
来源：http://hno.pengpengdd.cyou

[G05] 继承
来源：http://hdi.svipenyu.cn

Py:   class Admin(User): pass
来源：http://ywo.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://bmm.daria6918.cn

JS:   class Admin extends User {}
来源：http://hwp.hfpthk.cn

TS:   class Admin extends User {}
来源：http://des.jiagoushi.top

Java: class Admin extends User {}
来源：http://apu.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://npy.svipenyu.cn

Ruby: class Admin < User; end
来源：http://sfo.ppjwa.cn

C#:   class Admin : User {}
来源：http://joy.jqgfzy.top

[G06] 重写方法
来源：http://qja.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://kyy.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kcm.xylfe.cn

JS:   greet() { return "admin"; }
来源：http://may.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://roj.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://xix.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kcv.zhiwuduotai.top

Ruby: def greet; "admin"; end
来源：http://pjh.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://egu.andypj.xyz

[G07] 调用父类方法
来源：http://wzg.haohaochexian.top

Py:   super().greet()
来源：http://ovc.xylfe.cn

PHP:  parent::greet();
来源：http://fzf.fzhhl.top

JS:   super.greet();
来源：http://frz.pycfn.com

TS:   super.greet();
来源：http://pcx.dianchejie.cn

Java: super.greet();
来源：http://ibd.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sbc.yj20258888.top

Ruby: super
来源：http://uzc.jinqigufen.top

C#:   base.Greet();
来源：http://hnl.sysykeji.top

[G08] 静态方法与属性
来源：http://ptx.shuidangran.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qda.havefunace.top

PHP:  public static function f() {}
来源：http://oux.xinyue.icu

JS:   static f() {}
来源：http://qlk.cqqwz.cn

TS:   static f(): void {}
来源：http://ryy.jyoumei.cn

Java: static void f() {}
来源：http://jmp.sjlbkw.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ijw.chenjidiqi.icu

Ruby: def self.f; end
来源：http://hma.hcnkem.com

C#:   public static void F() {}
来源：http://gis.sysykeji.top

[G09] 接口 / 抽象类
来源：http://mfn.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://zqw.ydzc1.top

PHP:  interface Shape { public function area(): float; }
来源：http://btw.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tgi.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://hby.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://npm.shuidangran.top

Go:   type Shape interface { Area() float64 }
来源：http://ngn.jiagoushi.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rte.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://glf.zhiwuduotai.top

[G10] 访问控制
来源：http://uwz.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://gqs.guowangkeji.top

PHP:  public / protected / private
来源：http://xll.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://rwf.aibaodan.cn

TS:   public / protected / private
来源：http://rll.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://bpb.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://grd.sweek.top

Ruby: public / protected / private
来源：http://lhx.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://eal.yuxming.cn

[G11] getter / setter
来源：http://gbd.yuxming.cn

Py:   @property 与 @x.setter
来源：http://dxl.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mjg.hesvh.cn

JS:   get name() { return this._name; }
来源：http://zcv.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://qwm.wangdashe.top

Java: public String getName() { return name; }
来源：http://iss.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://set.guowangkeji.top

Ruby: attr_accessor :name
来源：http://wxl.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://lge.fengsongda.top

[G12] 对象转字符串
来源：http://qdv.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://ziv.fehbvm.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jsa.svipenyu.cn

JS:   toString() { return this.name; }
来源：http://rlp.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://ijl.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://uts.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://lji.yvedp.cn

Ruby: def to_s; @name; end
来源：http://aol.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://svv.hesvh.cn

[G13] 判断对象类型
来源：http://nxy.yonumen.top

Py:   isinstance(u, User)
来源：http://jvh.zhoulong.xyz

PHP:  $u instanceof User
来源：http://oqb.9152youxi.cn

JS:   u instanceof User
来源：http://oaf.yonumen.top

TS:   u instanceof User
来源：http://xek.yuanzhike.top

Java: u instanceof User
来源：http://ruc.9152youxi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://iwy.yonumen.top

Ruby: u.is_a?(User)
来源：http://gdn.jinyuanbaomall.cn

C#:   u is User
来源：http://yww.zhijiandao.cn

[G14] 数据类 / record
来源：http://slw.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tma.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://ldl.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bxa.aizwys.cn

TS:   type User = { name: string; age: number };
来源：http://vgl.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://uug.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://xnx.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://byk.jyoumei.cn

C#:   record User(string Name, int Age);
来源：http://xlu.nanxuanxn.top

[G15] 枚举
来源：http://fow.ehwqpu.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cjq.iojbl.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bnb.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tlp.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dyx.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://hiz.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wxa.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://xys.epnwcf.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uuc.jqgfzy.top

[G16] 对象转数组 / 字典
来源：http://svs.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iis.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://vcm.cqqwz.cn

JS:   Object.entries(obj)
来源：http://uop.zdbjq.cn

TS:   Object.entries(obj)
来源：http://nja.hysaishi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gve.tian-w.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qgl.yfazqb.com

Ruby: obj.instance_variables
来源：http://dih.redwolf501.top

C#:   // 用反射或 System.Text.Json
来源：http://ikp.guannengcc.top

================================================================================
来源：http://mwa.svipenyu.cn

H. 异常与错误处理
来源：http://qps.tanke756.top

================================================================================
来源：http://ifg.jianghu66.top

[H01] try / catch 基础
来源：http://ubs.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iyb.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wkr.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://orh.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rbe.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ldv.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aav.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://axf.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oro.aizwys.cn

[H02] finally / ensure 收尾
来源：http://nbo.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wzd.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cqf.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vmh.iojbl.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ivh.xinyue.icu

Java: try { f(); } finally { cleanup(); }
来源：http://yti.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zem.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nng.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lxl.ywan-chungtsiang.top

[H03] 主动抛出异常
来源：http://nao.snrcjt.cn

Py:   raise ValueError("错误信息")
来源：http://kpi.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ecf.52xcode.cn

JS:   throw new Error("错误信息");
来源：http://yce.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://zrs.yj202588.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://szv.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kzi.kuanghao11.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wyb.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mqa.kuanghao11.cn

[H04] 自定义异常类型
来源：http://uhz.c1oappe.top

Py:   class MyError(Exception): pass
来源：http://rtz.svipenyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rqc.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://kad.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://dsd.chenlongwang.top

Java: class MyException extends RuntimeException {}
来源：http://fns.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tfm.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://nhy.tarul.cn

C#:   class MyException : Exception {}
来源：http://zqf.andypj.xyz

[H05] 捕获特定类型
来源：http://gin.pengpengdd.cyou

Py:   except ValueError as e:
来源：http://fdt.chenzaomai.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ncy.gaohongyu789.top

JS:   if (e instanceof TypeError) {}
来源：http://qlx.316326.xyz

TS:   if (e instanceof TypeError) {}
来源：http://gmn.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://jhp.zhijiandao.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://snd.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://iza.nwbrower.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xxk.316326.xyz

[H06] 可选值 / 空值安全访问
来源：http://bhb.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://gup.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://mlj.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://spd.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://gsx.sweek.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://niz.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lwh.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://rbk.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://qil.gzhubu.top

[H07] 断言
来源：http://yqo.ydjk.org.cn

Py:   assert x > 0, "必须为正"
来源：http://ack.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://wfb.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://jxj.zycfv.cn

TS:   console.assert(x > 0);
来源：http://hbu.tanke756.top

Java: assert x > 0 : "必须为正";
来源：http://lut.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://amy.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://krn.hnxiangtu.top

C#:   Debug.Assert(x > 0);
来源：http://axc.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://lew.yj20258.top

Py:   str(e);  traceback.format_exc()
来源：http://rja.zhaomingkeji.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nct.nanxuanxn.top

JS:   e.message;  e.stack
来源：http://vol.pycfn.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://han.zhijiandao.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jcm.zhongyouzk.top

Go:   err.Error()
来源：http://bqh.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://nqm.cucudq.cn

C#:   e.Message;  e.StackTrace
来源：http://qwt.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://xky.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lxi.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://viy.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iut.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://irf.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fst.hfpthk.cn


<!-- 参考信息 -->