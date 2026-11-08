代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：https://ff.zhonguo1118.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：https://cl.zhonguo3118.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：https://ct.zhonguo3118.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：https://wa.zhonguo7118.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：https://uc.zhonguo4118.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：https://lo.zhonguo1118.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：https://wh.zhonguo5118.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：https://ba.zhonguo7118.cn

[F05] 判断文件或目录是否存在
来源：https://hn.zhonguo8118.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：https://cs.zhonguo1118.cn

PHP:  file_exists("a.txt");
来源：https://ic.zhonguo3118.cn

JS:   fs.existsSync("a.txt")
来源：https://sb.zhonguo2118.cn

TS:   fs.existsSync("a.txt")
来源：https://hi.zhonguo1118.cn

Java: Files.exists(Path.of("a.txt"))
来源：https://yo.zhonguo5118.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：https://qc.zhonguo4118.cn

Ruby: File.exist?("a.txt")
来源：https://jr.zhonguo8118.cn

C#:   File.Exists("a.txt")
来源：https://op.zhonguo1118.cn

[F06] 删除文件
来源：https://wm.zhonguo1118.cn

Py:   os.remove("a.txt")
来源：https://ip.zhonguo7118.cn

PHP:  unlink("a.txt");
来源：https://am.zhonguo3118.cn

JS:   fs.unlinkSync("a.txt")
来源：https://hu.zhonguo3118.cn

TS:   fs.unlinkSync("a.txt")
来源：https://do.zhonguo4118.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：https://qn.zhonguo7118.cn

Go:   os.Remove("a.txt")
来源：https://gz.zhonguo8118.cn

Ruby: File.delete("a.txt")
来源：https://dt.zhonguo1118.cn

C#:   File.Delete("a.txt");
来源：https://ou.zhonguo2118.cn

[F07] 创建目录（含多级）
来源：https://ki.zhonguo5118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://sw.zhonguo8118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://dd.zhonguo6118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://mj.zhonguo5118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://mn.zhonguo4118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://mk.zhonguo3118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://po.zhonguo2118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://bj.zhonguo5118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://yl.zhonguo6118.cn

[F08] 遍历目录
来源：https://um.zhonguo4118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://le.zhonguo7118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://ho.zhonguo7118.cn

JS:   fs.readdirSync("dir")
来源：https://bz.zhonguo5118.cn

TS:   fs.readdirSync("dir")
来源：https://mj.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://jb.zhonguo3118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://jx.zhonguo8118.cn

Ruby: Dir.children("dir")
来源：https://ty.zhonguo3118.cn

C#:   Directory.GetFiles("dir")
来源：https://bo.zhonguo7118.cn

[F09] 获取文件大小
来源：https://xy.zhonguo4118.cn

Py:   os.path.getsize("a.txt")
来源：https://yq.zhonguo6118.cn

PHP:  filesize("a.txt");
来源：https://gd.zhonguo8118.cn

JS:   fs.statSync("a.txt").size
来源：https://hy.zhonguo8118.cn

TS:   fs.statSync("a.txt").size
来源：https://yb.zhonguo3118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://fb.zhonguo4118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://zy.zhonguo2118.cn

Ruby: File.size("a.txt")
来源：https://ce.zhonguo2118.cn

C#:   new FileInfo("a.txt").Length
来源：https://fw.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://yz.zhonguo5118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://vm.zhonguo5118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://tc.zhonguo8118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://yp.zhonguo3118.cn

TS:   path.extname("a.txt")
来源：https://bx.zhonguo6118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://qd.zhonguo1118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://mm.zhonguo5118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://dv.zhonguo8118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ma.zhonguo1118.cn

[F11] 复制与移动文件
来源：https://il.zhonguo1118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://jz.zhonguo3118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://tv.zhonguo4118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://xq.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://ud.zhonguo1118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://sw.zhonguo6118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://yy.zhonguo7118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://cv.zhonguo2118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://sr.zhonguo4118.cn

[F12] CSV 读写
来源：https://vb.zhonguo8118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://kl.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://az.zhonguo3118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://ra.zhonguo5118.cn

TS:   // 同上
来源：https://yk.zhonguo8118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://yy.zhonguo1118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://nd.zhonguo7118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://ek.zhonguo5118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://rq.zhonguo2118.cn

================================================================================
来源：https://co.zhonguo1118.cn

G. 面向对象
来源：https://dn.zhonguo3118.cn

================================================================================
来源：https://tq.zhonguo8118.cn

[G01] 定义类
来源：https://ip.zhonguo4118.cn

Py:   class User: pass
来源：https://jn.zhonguo1118.cn

PHP:  class User {}
来源：https://uh.zhonguo8118.cn

JS:   class User {}
来源：https://ml.zhonguo5118.cn

TS:   class User { name: string = ""; }
来源：https://lc.zhonguo1118.cn

Java: class User {}
来源：https://fy.zhonguo3118.cn

Go:   type User struct { Name string }
来源：https://xg.zhonguo6118.cn

Ruby: class User; end
来源：https://av.zhonguo2118.cn

C#:   class User {}
来源：https://hq.zhonguo3118.cn

[G02] 构造函数
来源：https://tx.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ny.zhonguo6118.cn

PHP:  public function __construct(public string $name) {}
来源：https://bj.zhonguo8118.cn

JS:   constructor(name) { this.name = name; }
来源：https://dk.zhonguo8118.cn

TS:   constructor(public name: string) {}
来源：https://mj.zhonguo8118.cn

Java: User(String name) { this.name = name; }
来源：https://va.zhonguo4118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://gy.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://cg.zhonguo2118.cn

C#:   public User(string name) { Name = name; }
来源：https://kn.zhonguo8118.cn

[G03] 实例属性
来源：https://ks.zhonguo7118.cn

Py:   self.name = "x"
来源：https://kr.zhonguo7118.cn

PHP:  public string $name = "x";
来源：https://mj.zhonguo2118.cn

JS:   this.name = "x";
来源：https://ds.zhonguo7118.cn

TS:   name: string = "x";
来源：https://bl.zhonguo3118.cn

Java: private String name;
来源：https://ca.zhonguo8118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://lj.zhonguo2118.cn

Ruby: @name = "x"
来源：https://dg.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://ti.zhonguo8118.cn

[G04] 定义方法
来源：https://fy.zhonguo1118.cn

Py:   def greet(self): return self.name
来源：https://dj.zhonguo5118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://zk.zhonguo7118.cn

JS:   greet() { return this.name; }
来源：https://tl.zhonguo3118.cn

TS:   greet(): string { return this.name; }
来源：https://cx.zhonguo1118.cn

Java: String greet() { return name; }
来源：https://ki.zhonguo1118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://lz.zhonguo3118.cn

Ruby: def greet; @name; end
来源：https://sd.zhonguo8118.cn

C#:   public string Greet() => Name;
来源：https://na.zhonguo4118.cn

[G05] 继承
来源：https://bf.zhonguo3118.cn

Py:   class Admin(User): pass
来源：https://al.zhonguo5118.cn

PHP:  class Admin extends User {}
来源：https://tx.zhonguo4118.cn

JS:   class Admin extends User {}
来源：https://xt.zhonguo7118.cn

TS:   class Admin extends User {}
来源：https://px.zhonguo3118.cn

Java: class Admin extends User {}
来源：https://vb.zhonguo5118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://po.zhonguo7118.cn

Ruby: class Admin < User; end
来源：https://of.zhonguo5118.cn

C#:   class Admin : User {}
来源：https://mj.zhonguo7118.cn

[G06] 重写方法
来源：https://if.zhonguo3118.cn

Py:   def greet(self): return "admin"
来源：https://ap.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://kr.zhonguo3118.cn

JS:   greet() { return "admin"; }
来源：https://yc.zhonguo6118.cn

TS:   greet(): string { return "admin"; }
来源：https://yv.zhonguo8118.cn

Java: @Override String greet() { return "admin"; }
来源：https://kg.zhonguo2118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://zy.zhonguo6118.cn

Ruby: def greet; "admin"; end
来源：https://am.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://bn.zhonguo8118.cn

[G07] 调用父类方法
来源：https://zz.zhonguo7118.cn

Py:   super().greet()
来源：https://ma.zhonguo2118.cn

PHP:  parent::greet();
来源：https://er.zhonguo6118.cn

JS:   super.greet();
来源：https://co.zhonguo1118.cn

TS:   super.greet();
来源：https://zy.zhonguo7118.cn

Java: super.greet();
来源：https://st.zhonguo1118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://pa.zhonguo2118.cn

Ruby: super
来源：https://up.zhonguo1118.cn

C#:   base.Greet();
来源：https://di.zhonguo8118.cn

[G08] 静态方法与属性
来源：https://gs.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://wy.zhonguo4118.cn

PHP:  public static function f() {}
来源：https://yu.zhonguo8118.cn

JS:   static f() {}
来源：https://jj.zhonguo2118.cn

TS:   static f(): void {}
来源：https://yv.zhonguo3118.cn

Java: static void f() {}
来源：https://hj.zhonguo2118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://fe.zhonguo2118.cn

Ruby: def self.f; end
来源：https://rd.zhonguo3118.cn

C#:   public static void F() {}
来源：https://uz.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://jz.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://pw.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://rb.zhonguo5118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://tf.zhonguo7118.cn

TS:   interface Shape { area(): number; }
来源：https://hs.zhonguo1118.cn

Java: interface Shape { double area(); }
来源：https://bz.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://xa.zhonguo7118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://yr.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://gd.zhonguo1118.cn

[G10] 访问控制
来源：https://jz.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://za.zhonguo5118.cn

PHP:  public / protected / private
来源：https://gx.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://jx.zhonguo4118.cn

TS:   public / protected / private
来源：https://yx.zhonguo7118.cn

Java: public / protected / private / 默认包级
来源：https://lc.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://mz.zhonguo1118.cn

Ruby: public / protected / private
来源：https://qy.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://xy.zhonguo3118.cn

[G11] getter / setter
来源：https://cq.zhonguo5118.cn

Py:   @property 与 @x.setter
来源：https://of.zhonguo5118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://xt.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://lg.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://iv.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://om.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://qh.zhonguo8118.cn

Ruby: attr_accessor :name
来源：https://hk.zhonguo6118.cn

C#:   public string Name { get; set; }
来源：https://bf.zhonguo3118.cn

[G12] 对象转字符串
来源：https://xp.zhonguo5118.cn

Py:   def __str__(self): return self.name
来源：https://ri.zhonguo6118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://tw.zhonguo1118.cn

JS:   toString() { return this.name; }
来源：https://xb.zhonguo4118.cn

TS:   toString(): string { return this.name; }
来源：https://xv.zhonguo1118.cn

Java: @Override public String toString() { return name; }
来源：https://nc.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://fx.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://oj.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://ay.zhonguo1118.cn

[G13] 判断对象类型
来源：https://km.zhonguo7118.cn

Py:   isinstance(u, User)
来源：https://yd.zhonguo3118.cn

PHP:  $u instanceof User
来源：https://es.zhonguo5118.cn

JS:   u instanceof User
来源：https://ka.zhonguo2118.cn

TS:   u instanceof User
来源：https://zp.zhonguo3118.cn

Java: u instanceof User
来源：https://ky.zhonguo2118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://bu.zhonguo4118.cn

Ruby: u.is_a?(User)
来源：https://rb.zhonguo8118.cn

C#:   u is User
来源：https://rz.zhonguo5118.cn

[G14] 数据类 / record
来源：https://ek.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://yv.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://tj.zhonguo5118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://oz.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://xm.zhonguo3118.cn

Java: record User(String name, int age) {}
来源：https://lt.zhonguo8118.cn

Go:   type User struct { Name string; Age int }
来源：https://hy.zhonguo3118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ut.zhonguo6118.cn

C#:   record User(string Name, int Age);
来源：https://ka.zhonguo6118.cn

[G15] 枚举
来源：https://cv.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://oi.zhonguo3118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ib.zhonguo4118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://hk.zhonguo3118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://zk.zhonguo7118.cn

Java: enum Color { RED, GREEN }
来源：https://bc.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://jd.zhonguo5118.cn

Ruby: Color = %i[red green].freeze
来源：https://np.zhonguo1118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ti.zhonguo1118.cn

[G16] 对象转数组 / 字典
来源：https://og.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://oc.zhonguo8118.cn

PHP:  get_object_vars($obj);
来源：https://sx.zhonguo7118.cn

JS:   Object.entries(obj)
来源：https://qt.zhonguo8118.cn

TS:   Object.entries(obj)
来源：https://tq.zhonguo5118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://tp.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://ug.zhonguo4118.cn

Ruby: obj.instance_variables
来源：https://ii.zhonguo4118.cn

C#:   // 用反射或 System.Text.Json
来源：https://ea.zhonguo5118.cn

================================================================================
来源：https://su.zhonguo3118.cn

H. 异常与错误处理
来源：https://fj.zhonguo2118.cn

================================================================================
来源：https://ll.zhonguo3118.cn

[H01] try / catch 基础
来源：https://it.zhonguo2118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://md.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://kr.zhonguo8118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://wr.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://yu.zhonguo1118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://pz.zhonguo8118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://nb.zhonguo4118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://wo.zhonguo8118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ug.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://xm.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://zb.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://sw.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://fj.zhonguo6118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://dm.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://gy.zhonguo6118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ia.zhonguo4118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://lq.zhonguo2118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ay.zhonguo4118.cn

[H03] 主动抛出异常
来源：https://ep.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://ca.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://jc.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://hw.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://tc.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://mh.zhonguo7118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://lw.zhonguo7118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://kd.zhonguo4118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://ux.zhonguo5118.cn

[H04] 自定义异常类型
来源：https://vr.zhonguo4118.cn

Py:   class MyError(Exception): pass
来源：https://bf.zhonguo2118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://bl.zhonguo8118.cn

JS:   class MyError extends Error {}
来源：https://vp.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://at.zhonguo6118.cn

Java: class MyException extends RuntimeException {}
来源：https://ue.zhonguo2118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://wl.zhonguo1118.cn

Ruby: class MyError < StandardError; end
来源：https://lt.zhonguo3118.cn

C#:   class MyException : Exception {}
来源：https://cf.zhonguo1118.cn

[H05] 捕获特定类型
来源：https://db.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://bw.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://cc.zhonguo7118.cn

JS:   if (e instanceof TypeError) {}
来源：https://vv.zhonguo6118.cn

TS:   if (e instanceof TypeError) {}
来源：https://fe.zhonguo5118.cn

Java: catch (IOException | SQLException e) {}
来源：https://rl.zhonguo8118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://wi.zhonguo7118.cn

Ruby: rescue ArgumentError => e
来源：https://ic.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://om.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://ak.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://dq.zhonguo7118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://sw.zhonguo1118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://xy.zhonguo3118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://qp.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://qv.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://za.zhonguo4118.cn

Ruby: d&.dig(:a, :b)
来源：https://nm.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://jh.zhonguo2118.cn

[H07] 断言
来源：https://ua.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://ai.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://xx.zhonguo2118.cn

JS:   console.assert(x > 0);
来源：https://mr.zhonguo5118.cn

TS:   console.assert(x > 0);
来源：https://kz.zhonguo4118.cn

Java: assert x > 0 : "必须为正";
来源：https://un.zhonguo3118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://dz.zhonguo2118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://wj.zhonguo1118.cn

C#:   Debug.Assert(x > 0);
来源：https://nm.zhonguo4118.cn

[H08] 获取错误信息与堆栈
来源：https://hj.zhonguo7118.cn

Py:   str(e);  traceback.format_exc()
来源：https://ap.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://qd.zhonguo7118.cn

JS:   e.message;  e.stack
来源：https://by.zhonguo8118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://sg.zhonguo8118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ux.zhonguo3118.cn

Go:   err.Error()
来源：https://ej.zhonguo7118.cn


<!-- 参考信息 -->