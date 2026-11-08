代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://jq.zhonguo3118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://fc.zhonguo4118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://aq.zhonguo3118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://qm.zhonguo5118.cn

[F05] 判断文件或目录是否存在
来源：https://lp.zhonguo4118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://xz.zhonguo8118.cn

PHP:  file_exists("a.txt");
来源：https://cr.zhonguo6118.cn

JS:   fs.existsSync("a.txt")
来源：https://mq.zhonguo5118.cn

TS:   fs.existsSync("a.txt")
来源：https://yj.zhonguo5118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://ri.zhonguo1118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://ab.zhonguo2118.cn

Ruby: File.exist?("a.txt")
来源：https://ab.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://bi.zhonguo4118.cn

[F06] 删除文件
来源：https://px.zhonguo6118.cn

Py:   os.remove("a.txt")
来源：https://eo.zhonguo8118.cn

PHP:  unlink("a.txt");
来源：https://cc.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://pv.zhonguo7118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://yx.zhonguo1118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://cj.zhonguo3118.cn

Go:   os.Remove("a.txt")
来源：https://fm.zhonguo1118.cn

Ruby: File.delete("a.txt")
来源：https://wf.zhonguo2118.cn

C#:   File.Delete("a.txt");
来源：https://in.zhonguo3118.cn

[F07] 创建目录（含多级）
来源：https://ni.zhonguo3118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://jn.zhonguo1118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://hg.zhonguo3118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://gq.zhonguo7118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://bk.zhonguo4118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://ip.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://wd.zhonguo6118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://ti.zhonguo3118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://hb.zhonguo6118.cn

[F08] 遍历目录
来源：https://ay.zhonguo7118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://ow.zhonguo5118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://gj.zhonguo2118.cn

JS:   fs.readdirSync("dir")
来源：https://aq.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://ek.zhonguo6118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://rt.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://oa.zhonguo5118.cn

Ruby: Dir.children("dir")
来源：https://xt.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://ru.zhonguo5118.cn

[F09] 获取文件大小
来源：https://tu.zhonguo6118.cn

Py:   os.path.getsize("a.txt")
来源：https://wq.zhonguo1118.cn

PHP:  filesize("a.txt");
来源：https://lc.zhonguo6118.cn

JS:   fs.statSync("a.txt").size
来源：https://by.zhonguo3118.cn

TS:   fs.statSync("a.txt").size
来源：https://ig.zhonguo7118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://mk.zhonguo7118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://wn.zhonguo4118.cn

Ruby: File.size("a.txt")
来源：https://my.zhonguo8118.cn

C#:   new FileInfo("a.txt").Length
来源：https://gy.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://vw.zhonguo1118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://lh.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://rl.zhonguo7118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://el.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://jv.zhonguo3118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://is.zhonguo7118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://mr.zhonguo3118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://dr.zhonguo6118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://yy.zhonguo1118.cn

[F11] 复制与移动文件
来源：https://bz.zhonguo2118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ea.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://uk.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://cp.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ht.zhonguo3118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://cm.zhonguo4118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://df.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://nl.zhonguo5118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://rt.zhonguo1118.cn

[F12] CSV 读写
来源：https://tt.zhonguo4118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://je.zhonguo5118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://bw.zhonguo5118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://lt.zhonguo2118.cn

TS:   // 同上
来源：https://hf.zhonguo3118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://hz.zhonguo8118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://vj.zhonguo1118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://ze.zhonguo2118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://dh.zhonguo1118.cn

================================================================================
来源：https://sk.zhonguo6118.cn

G. 面向对象
来源：https://pd.zhonguo6118.cn

================================================================================
来源：https://at.zhonguo4118.cn

[G01] 定义类
来源：https://xj.zhonguo2118.cn

Py:   class User: pass
来源：https://er.zhonguo5118.cn

PHP:  class User {}
来源：https://qf.zhonguo2118.cn

JS:   class User {}
来源：https://qk.zhonguo7118.cn

TS:   class User { name: string = ""; }
来源：https://nt.zhonguo7118.cn

Java: class User {}
来源：https://de.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://ws.zhonguo7118.cn

Ruby: class User; end
来源：https://yf.zhonguo3118.cn

C#:   class User {}
来源：https://vw.zhonguo3118.cn

[G02] 构造函数
来源：https://wv.zhonguo3118.cn

Py:   def __init__(self, name): self.name = name
来源：https://vw.zhonguo8118.cn

PHP:  public function __construct(public string $name) {}
来源：https://jp.zhonguo8118.cn

JS:   constructor(name) { this.name = name; }
来源：https://xb.zhonguo1118.cn

TS:   constructor(public name: string) {}
来源：https://pi.zhonguo7118.cn

Java: User(String name) { this.name = name; }
来源：https://bd.zhonguo6118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://py.zhonguo3118.cn

Ruby: def initialize(name); @name = name; end
来源：https://xf.zhonguo3118.cn

C#:   public User(string name) { Name = name; }
来源：https://el.zhonguo3118.cn

[G03] 实例属性
来源：https://tb.zhonguo4118.cn

Py:   self.name = "x"
来源：https://vj.zhonguo2118.cn

PHP:  public string $name = "x";
来源：https://fd.zhonguo6118.cn

JS:   this.name = "x";
来源：https://pt.zhonguo2118.cn

TS:   name: string = "x";
来源：https://bh.zhonguo6118.cn

Java: private String name;
来源：https://kl.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://di.zhonguo4118.cn

Ruby: @name = "x"
来源：https://vp.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://hj.zhonguo3118.cn

[G04] 定义方法
来源：https://kh.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://fp.zhonguo4118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://ow.zhonguo8118.cn

JS:   greet() { return this.name; }
来源：https://jm.zhonguo5118.cn

TS:   greet(): string { return this.name; }
来源：https://lq.zhonguo3118.cn

Java: String greet() { return name; }
来源：https://ou.zhonguo7118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://pp.zhonguo3118.cn

Ruby: def greet; @name; end
来源：https://lh.zhonguo4118.cn

C#:   public string Greet() => Name;
来源：https://hr.zhonguo5118.cn

[G05] 继承
来源：https://kg.zhonguo5118.cn

Py:   class Admin(User): pass
来源：https://vh.zhonguo2118.cn

PHP:  class Admin extends User {}
来源：https://uj.zhonguo4118.cn

JS:   class Admin extends User {}
来源：https://ui.zhonguo2118.cn

TS:   class Admin extends User {}
来源：https://xc.zhonguo2118.cn

Java: class Admin extends User {}
来源：https://it.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://wh.zhonguo2118.cn

Ruby: class Admin < User; end
来源：https://ae.zhonguo8118.cn

C#:   class Admin : User {}
来源：https://zg.zhonguo5118.cn

[G06] 重写方法
来源：https://ox.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://qb.zhonguo6118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://zz.zhonguo4118.cn

JS:   greet() { return "admin"; }
来源：https://ev.zhonguo2118.cn

TS:   greet(): string { return "admin"; }
来源：https://zr.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://tz.zhonguo2118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://mv.zhonguo7118.cn

Ruby: def greet; "admin"; end
来源：https://pt.zhonguo3118.cn

C#:   public override string Greet() => "admin";
来源：https://wk.zhonguo7118.cn

[G07] 调用父类方法
来源：https://nk.zhonguo2118.cn

Py:   super().greet()
来源：https://ug.zhonguo8118.cn

PHP:  parent::greet();
来源：https://qg.zhonguo3118.cn

JS:   super.greet();
来源：https://ok.zhonguo6118.cn

TS:   super.greet();
来源：https://ei.zhonguo7118.cn

Java: super.greet();
来源：https://pr.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://hh.zhonguo4118.cn

Ruby: super
来源：https://em.zhonguo7118.cn

C#:   base.Greet();
来源：https://zj.zhonguo7118.cn

[G08] 静态方法与属性
来源：https://nw.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://rt.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://zk.zhonguo1118.cn

JS:   static f() {}
来源：https://wi.zhonguo1118.cn

TS:   static f(): void {}
来源：https://am.zhonguo8118.cn

Java: static void f() {}
来源：https://ey.zhonguo7118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://li.zhonguo6118.cn

Ruby: def self.f; end
来源：https://uw.zhonguo6118.cn

C#:   public static void F() {}
来源：https://ww.zhonguo3118.cn

[G09] 接口 / 抽象类
来源：https://yy.zhonguo6118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ki.zhonguo7118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ga.zhonguo6118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://el.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://ug.zhonguo2118.cn

Java: interface Shape { double area(); }
来源：https://hy.zhonguo7118.cn

Go:   type Shape interface { Area() float64 }
来源：https://su.zhonguo4118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://fk.zhonguo7118.cn

C#:   interface IShape { double Area(); }
来源：https://py.zhonguo2118.cn

[G10] 访问控制
来源：https://be.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ay.zhonguo7118.cn

PHP:  public / protected / private
来源：https://km.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://ct.zhonguo3118.cn

TS:   public / protected / private
来源：https://kt.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://zu.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://wb.zhonguo4118.cn

Ruby: public / protected / private
来源：https://vy.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://bg.zhonguo8118.cn

[G11] getter / setter
来源：https://aa.zhonguo2118.cn

Py:   @property 与 @x.setter
来源：https://it.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://kf.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://gq.zhonguo4118.cn

TS:   get name(): string { return this._name; }
来源：https://vt.zhonguo4118.cn

Java: public String getName() { return name; }
来源：https://bl.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://tn.zhonguo3118.cn

Ruby: attr_accessor :name
来源：https://ov.zhonguo2118.cn

C#:   public string Name { get; set; }
来源：https://lf.zhonguo1118.cn

[G12] 对象转字符串
来源：https://sx.zhonguo1118.cn

Py:   def __str__(self): return self.name
来源：https://dh.zhonguo7118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://zg.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://xs.zhonguo8118.cn

TS:   toString(): string { return this.name; }
来源：https://qw.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://fk.zhonguo8118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://my.zhonguo3118.cn

Ruby: def to_s; @name; end
来源：https://vj.zhonguo2118.cn

C#:   public override string ToString() => Name;
来源：https://xv.zhonguo3118.cn

[G13] 判断对象类型
来源：https://ox.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://ka.zhonguo8118.cn

PHP:  $u instanceof User
来源：https://qc.zhonguo6118.cn

JS:   u instanceof User
来源：https://eb.zhonguo1118.cn

TS:   u instanceof User
来源：https://qo.zhonguo8118.cn

Java: u instanceof User
来源：https://el.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://pt.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://ol.zhonguo2118.cn

C#:   u is User
来源：https://ws.zhonguo4118.cn

[G14] 数据类 / record
来源：https://mj.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://pj.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://fn.zhonguo3118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://xa.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://yt.zhonguo6118.cn

Java: record User(String name, int age) {}
来源：https://zy.zhonguo5118.cn

Go:   type User struct { Name string; Age int }
来源：https://mv.zhonguo2118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://db.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://lg.zhonguo7118.cn

[G15] 枚举
来源：https://jr.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://gk.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://we.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://kj.zhonguo3118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ee.zhonguo8118.cn

Java: enum Color { RED, GREEN }
来源：https://iv.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://si.zhonguo8118.cn

Ruby: Color = %i[red green].freeze
来源：https://zl.zhonguo1118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://qv.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://tj.zhonguo5118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ni.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://ti.zhonguo5118.cn

JS:   Object.entries(obj)
来源：https://hn.zhonguo1118.cn

TS:   Object.entries(obj)
来源：https://qp.zhonguo3118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://tt.zhonguo3118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://nv.zhonguo7118.cn

Ruby: obj.instance_variables
来源：https://xc.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://bj.zhonguo7118.cn

================================================================================
来源：https://ni.zhonguo1118.cn

H. 异常与错误处理
来源：https://hu.zhonguo2118.cn

================================================================================
来源：https://co.zhonguo7118.cn

[H01] try / catch 基础
来源：https://ol.zhonguo5118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://bm.zhonguo1118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://pt.zhonguo5118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://in.zhonguo3118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://gm.zhonguo6118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://hj.zhonguo6118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://hu.zhonguo5118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://jp.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://xq.zhonguo7118.cn

[H02] finally / ensure 收尾
来源：https://ck.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://dv.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://en.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://or.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://py.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://kj.zhonguo5118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://aw.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://yp.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://wo.zhonguo2118.cn

[H03] 主动抛出异常
来源：https://pp.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://jb.zhonguo7118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://wp.zhonguo7118.cn

JS:   throw new Error("错误信息");
来源：https://wz.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://wa.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://lx.zhonguo8118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ak.zhonguo3118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://pb.zhonguo5118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://rl.zhonguo5118.cn

[H04] 自定义异常类型
来源：https://sq.zhonguo7118.cn

Py:   class MyError(Exception): pass
来源：https://vc.zhonguo3118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ad.zhonguo7118.cn

JS:   class MyError extends Error {}
来源：https://kr.zhonguo6118.cn

TS:   class MyError extends Error {}
来源：https://pr.zhonguo3118.cn

Java: class MyException extends RuntimeException {}
来源：https://on.zhonguo4118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://ud.zhonguo3118.cn

Ruby: class MyError < StandardError; end
来源：https://xe.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://qa.zhonguo5118.cn

[H05] 捕获特定类型
来源：https://be.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://zl.zhonguo5118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://jf.zhonguo7118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ay.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://iu.zhonguo8118.cn

Java: catch (IOException | SQLException e) {}
来源：https://un.zhonguo7118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://vh.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://tl.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://en.zhonguo3118.cn

[H06] 可选值 / 空值安全访问
来源：https://cs.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://qn.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://oh.zhonguo3118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://mw.zhonguo2118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://iz.zhonguo6118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ci.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ke.zhonguo2118.cn

Ruby: d&.dig(:a, :b)
来源：https://tx.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://jb.zhonguo8118.cn

[H07] 断言
来源：https://qt.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://jz.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://rx.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://mm.zhonguo7118.cn

TS:   console.assert(x > 0);
来源：https://qm.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://hp.zhonguo5118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://vl.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://yr.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://gk.zhonguo3118.cn

[H08] 获取错误信息与堆栈
来源：https://yg.zhonguo1118.cn

Py:   str(e);  traceback.format_exc()
来源：https://vh.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://pk.zhonguo5118.cn

JS:   e.message;  e.stack
来源：https://et.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://lo.zhonguo7118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://pr.zhonguo2118.cn

Go:   err.Error()
来源：https://ds.zhonguo6118.cn

Ruby: e.message;  e.backtrace
来源：https://ri.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://qb.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://hm.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://ty.zhonguo6118.cn


<!-- 参考信息 -->