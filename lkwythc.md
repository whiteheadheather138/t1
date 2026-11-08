代发 wailian999

Ruby: File.delete("a.txt")
来源：https://dh.zhonguo4118.cn

C#:   File.Delete("a.txt");
来源：https://dy.zhonguo1118.cn

[F07] 创建目录（含多级）
来源：https://jf.zhonguo1118.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：https://ha.zhonguo6118.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：https://cd.zhonguo7118.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://fz.zhonguo1118.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：https://cx.zhonguo2118.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：https://cz.zhonguo2118.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：https://dl.zhonguo7118.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：https://en.zhonguo1118.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：https://ov.zhonguo6118.cn

[F08] 遍历目录
来源：https://gv.zhonguo2118.cn

Py:   for name in os.listdir("dir"): print(name)
来源：https://zy.zhonguo5118.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：https://fo.zhonguo4118.cn

JS:   fs.readdirSync("dir")
来源：https://aj.zhonguo4118.cn

TS:   fs.readdirSync("dir")
来源：https://yb.zhonguo5118.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：https://cf.zhonguo2118.cn

Go:   entries, _ := os.ReadDir("dir")
来源：https://bg.zhonguo3118.cn

Ruby: Dir.children("dir")
来源：https://ww.zhonguo8118.cn

C#:   Directory.GetFiles("dir")
来源：https://jw.zhonguo3118.cn

[F09] 获取文件大小
来源：https://yd.zhonguo2118.cn

Py:   os.path.getsize("a.txt")
来源：https://fg.zhonguo3118.cn

PHP:  filesize("a.txt");
来源：https://bd.zhonguo5118.cn

JS:   fs.statSync("a.txt").size
来源：https://rz.zhonguo2118.cn

TS:   fs.statSync("a.txt").size
来源：https://fb.zhonguo8118.cn

Java: Files.size(Path.of("a.txt"))
来源：https://fl.zhonguo7118.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：https://tw.zhonguo5118.cn

Ruby: File.size("a.txt")
来源：https://ix.zhonguo7118.cn

C#:   new FileInfo("a.txt").Length
来源：https://br.zhonguo2118.cn

[F10] 取文件扩展名 / 文件名
来源：https://wq.zhonguo4118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://nm.zhonguo4118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://jq.zhonguo5118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://ld.zhonguo8118.cn

TS:   path.extname("a.txt")
来源：https://lv.zhonguo5118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://hm.zhonguo5118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://lp.zhonguo1118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://qw.zhonguo5118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://ps.zhonguo6118.cn

[F11] 复制与移动文件
来源：https://ba.zhonguo4118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://tv.zhonguo4118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://rk.zhonguo7118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://xm.zhonguo3118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://st.zhonguo6118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://gc.zhonguo5118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://gt.zhonguo2118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://mn.zhonguo1118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://jd.zhonguo5118.cn

[F12] CSV 读写
来源：https://wo.zhonguo4118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://ts.zhonguo1118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://nc.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://vl.zhonguo4118.cn

TS:   // 同上
来源：https://bm.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://ip.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://py.zhonguo2118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://oy.zhonguo3118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://qt.zhonguo2118.cn

================================================================================
来源：https://rg.zhonguo6118.cn

G. 面向对象
来源：https://sl.zhonguo1118.cn

================================================================================
来源：https://zl.zhonguo7118.cn

[G01] 定义类
来源：https://ye.zhonguo8118.cn

Py:   class User: pass
来源：https://kb.zhonguo2118.cn

PHP:  class User {}
来源：https://kz.zhonguo7118.cn

JS:   class User {}
来源：https://oo.zhonguo6118.cn

TS:   class User { name: string = ""; }
来源：https://gf.zhonguo8118.cn

Java: class User {}
来源：https://me.zhonguo2118.cn

Go:   type User struct { Name string }
来源：https://sg.zhonguo4118.cn

Ruby: class User; end
来源：https://tx.zhonguo5118.cn

C#:   class User {}
来源：https://ty.zhonguo3118.cn

[G02] 构造函数
来源：https://lb.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://wr.zhonguo2118.cn

PHP:  public function __construct(public string $name) {}
来源：https://dc.zhonguo6118.cn

JS:   constructor(name) { this.name = name; }
来源：https://dd.zhonguo3118.cn

TS:   constructor(public name: string) {}
来源：https://hx.zhonguo2118.cn

Java: User(String name) { this.name = name; }
来源：https://yd.zhonguo8118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://cx.zhonguo5118.cn

Ruby: def initialize(name); @name = name; end
来源：https://et.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://ek.zhonguo5118.cn

[G03] 实例属性
来源：https://cq.zhonguo5118.cn

Py:   self.name = "x"
来源：https://bc.zhonguo6118.cn

PHP:  public string $name = "x";
来源：https://ch.zhonguo4118.cn

JS:   this.name = "x";
来源：https://kx.zhonguo8118.cn

TS:   name: string = "x";
来源：https://wp.zhonguo7118.cn

Java: private String name;
来源：https://eo.zhonguo2118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://kf.zhonguo5118.cn

Ruby: @name = "x"
来源：https://re.zhonguo5118.cn

C#:   public string Name { get; set; } = "x";
来源：https://fe.zhonguo6118.cn

[G04] 定义方法
来源：https://lr.zhonguo8118.cn

Py:   def greet(self): return self.name
来源：https://wr.zhonguo8118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://jm.zhonguo3118.cn

JS:   greet() { return this.name; }
来源：https://an.zhonguo8118.cn

TS:   greet(): string { return this.name; }
来源：https://bo.zhonguo2118.cn

Java: String greet() { return name; }
来源：https://tj.zhonguo1118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://jm.zhonguo6118.cn

Ruby: def greet; @name; end
来源：https://ih.zhonguo5118.cn

C#:   public string Greet() => Name;
来源：https://km.zhonguo6118.cn

[G05] 继承
来源：https://gq.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://cj.zhonguo1118.cn

PHP:  class Admin extends User {}
来源：https://vk.zhonguo7118.cn

JS:   class Admin extends User {}
来源：https://xv.zhonguo8118.cn

TS:   class Admin extends User {}
来源：https://oe.zhonguo3118.cn

Java: class Admin extends User {}
来源：https://pu.zhonguo7118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://zk.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://jy.zhonguo4118.cn

C#:   class Admin : User {}
来源：https://fx.zhonguo7118.cn

[G06] 重写方法
来源：https://gf.zhonguo6118.cn

Py:   def greet(self): return "admin"
来源：https://xa.zhonguo6118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ur.zhonguo1118.cn

JS:   greet() { return "admin"; }
来源：https://ez.zhonguo7118.cn

TS:   greet(): string { return "admin"; }
来源：https://du.zhonguo1118.cn

Java: @Override String greet() { return "admin"; }
来源：https://sb.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://le.zhonguo2118.cn

Ruby: def greet; "admin"; end
来源：https://hv.zhonguo2118.cn

C#:   public override string Greet() => "admin";
来源：https://ub.zhonguo2118.cn

[G07] 调用父类方法
来源：https://fk.zhonguo7118.cn

Py:   super().greet()
来源：https://oo.zhonguo7118.cn

PHP:  parent::greet();
来源：https://lo.zhonguo7118.cn

JS:   super.greet();
来源：https://ox.zhonguo7118.cn

TS:   super.greet();
来源：https://wg.zhonguo6118.cn

Java: super.greet();
来源：https://rg.zhonguo3118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://do.zhonguo3118.cn

Ruby: super
来源：https://lf.zhonguo3118.cn

C#:   base.Greet();
来源：https://jg.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://gv.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://cj.zhonguo4118.cn

PHP:  public static function f() {}
来源：https://eb.zhonguo1118.cn

JS:   static f() {}
来源：https://cl.zhonguo2118.cn

TS:   static f(): void {}
来源：https://kl.zhonguo6118.cn

Java: static void f() {}
来源：https://bt.zhonguo2118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://qm.zhonguo7118.cn

Ruby: def self.f; end
来源：https://nd.zhonguo3118.cn

C#:   public static void F() {}
来源：https://yu.zhonguo5118.cn

[G09] 接口 / 抽象类
来源：https://fe.zhonguo5118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ym.zhonguo8118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://af.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://ai.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://jf.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://fc.zhonguo8118.cn

Go:   type Shape interface { Area() float64 }
来源：https://sm.zhonguo8118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ks.zhonguo5118.cn

C#:   interface IShape { double Area(); }
来源：https://rb.zhonguo8118.cn

[G10] 访问控制
来源：https://st.zhonguo1118.cn

Py:   约定 _protected / __private（不强制）
来源：https://wr.zhonguo1118.cn

PHP:  public / protected / private
来源：https://rn.zhonguo3118.cn

JS:   #private 字段；其余公开
来源：https://vf.zhonguo7118.cn

TS:   public / protected / private
来源：https://vd.zhonguo6118.cn

Java: public / protected / private / 默认包级
来源：https://oo.zhonguo3118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://zc.zhonguo1118.cn

Ruby: public / protected / private
来源：https://op.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://vh.zhonguo5118.cn

[G11] getter / setter
来源：https://ab.zhonguo4118.cn

Py:   @property 与 @x.setter
来源：https://ea.zhonguo4118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://um.zhonguo6118.cn

JS:   get name() { return this._name; }
来源：https://oa.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://yt.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://qq.zhonguo5118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://kg.zhonguo4118.cn

Ruby: attr_accessor :name
来源：https://oy.zhonguo2118.cn

C#:   public string Name { get; set; }
来源：https://pa.zhonguo7118.cn

[G12] 对象转字符串
来源：https://yq.zhonguo7118.cn

Py:   def __str__(self): return self.name
来源：https://ki.zhonguo4118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://xp.zhonguo8118.cn

JS:   toString() { return this.name; }
来源：https://wu.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://ad.zhonguo2118.cn

Java: @Override public String toString() { return name; }
来源：https://cd.zhonguo4118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://bo.zhonguo1118.cn

Ruby: def to_s; @name; end
来源：https://kd.zhonguo4118.cn

C#:   public override string ToString() => Name;
来源：https://wx.zhonguo3118.cn

[G13] 判断对象类型
来源：https://ff.zhonguo1118.cn

Py:   isinstance(u, User)
来源：https://hw.zhonguo1118.cn

PHP:  $u instanceof User
来源：https://qb.zhonguo1118.cn

JS:   u instanceof User
来源：https://ex.zhonguo2118.cn

TS:   u instanceof User
来源：https://tm.zhonguo3118.cn

Java: u instanceof User
来源：https://bk.zhonguo5118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ee.zhonguo6118.cn

Ruby: u.is_a?(User)
来源：https://ah.zhonguo1118.cn

C#:   u is User
来源：https://qk.zhonguo1118.cn

[G14] 数据类 / record
来源：https://gf.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://gz.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://np.zhonguo4118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://qn.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://sw.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://dx.zhonguo3118.cn

Go:   type User struct { Name string; Age int }
来源：https://bk.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://vz.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://qq.zhonguo2118.cn

[G15] 枚举
来源：https://xo.zhonguo1118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://wt.zhonguo1118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://xt.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://yv.zhonguo2118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ig.zhonguo7118.cn

Java: enum Color { RED, GREEN }
来源：https://ra.zhonguo1118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://wu.zhonguo6118.cn

Ruby: Color = %i[red green].freeze
来源：https://iu.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://no.zhonguo4118.cn

[G16] 对象转数组 / 字典
来源：https://dd.zhonguo8118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://qg.zhonguo7118.cn

PHP:  get_object_vars($obj);
来源：https://an.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://ef.zhonguo5118.cn

TS:   Object.entries(obj)
来源：https://ym.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://po.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://yv.zhonguo2118.cn

Ruby: obj.instance_variables
来源：https://dn.zhonguo6118.cn

C#:   // 用反射或 System.Text.Json
来源：https://eb.zhonguo1118.cn

================================================================================
来源：https://bw.zhonguo3118.cn

H. 异常与错误处理
来源：https://fj.zhonguo7118.cn

================================================================================
来源：https://yo.zhonguo4118.cn

[H01] try / catch 基础
来源：https://pz.zhonguo6118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://np.zhonguo6118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://cg.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://eq.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://yo.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://zt.zhonguo5118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://pv.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ew.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ho.zhonguo3118.cn

[H02] finally / ensure 收尾
来源：https://wb.zhonguo2118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://pw.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://kq.zhonguo4118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://sb.zhonguo4118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://bt.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://qi.zhonguo3118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://xl.zhonguo7118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://nt.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://qd.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://ae.zhonguo3118.cn

Py:   raise ValueError("错误信息")
来源：https://tt.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ki.zhonguo6118.cn

JS:   throw new Error("错误信息");
来源：https://ij.zhonguo5118.cn

TS:   throw new Error("错误信息");
来源：https://gf.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://gq.zhonguo3118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://jz.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://bu.zhonguo2118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://as.zhonguo4118.cn

[H04] 自定义异常类型
来源：https://pg.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://vg.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://eo.zhonguo1118.cn

JS:   class MyError extends Error {}
来源：https://ts.zhonguo4118.cn

TS:   class MyError extends Error {}
来源：https://ax.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://iy.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://co.zhonguo1118.cn

Ruby: class MyError < StandardError; end
来源：https://it.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://wl.zhonguo3118.cn

[H05] 捕获特定类型
来源：https://mv.zhonguo8118.cn

Py:   except ValueError as e:
来源：https://do.zhonguo1118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://or.zhonguo2118.cn

JS:   if (e instanceof TypeError) {}
来源：https://sb.zhonguo2118.cn

TS:   if (e instanceof TypeError) {}
来源：https://tb.zhonguo6118.cn

Java: catch (IOException | SQLException e) {}
来源：https://uo.zhonguo1118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://hj.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://pb.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://ax.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://pa.zhonguo4118.cn

Py:   value = d.get("k") or default
来源：https://pe.zhonguo7118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://wi.zhonguo8118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://lr.zhonguo8118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://be.zhonguo4118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://uh.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://hy.zhonguo5118.cn

Ruby: d&.dig(:a, :b)
来源：https://se.zhonguo1118.cn

C#:   obj?.A?.B ?? default
来源：https://no.zhonguo5118.cn

[H07] 断言
来源：https://vi.zhonguo7118.cn

Py:   assert x > 0, "必须为正"
来源：https://sb.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://sc.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://oi.zhonguo3118.cn

TS:   console.assert(x > 0);
来源：https://vt.zhonguo1118.cn

Java: assert x > 0 : "必须为正";
来源：https://ri.zhonguo8118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://uo.zhonguo6118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://em.zhonguo4118.cn

C#:   Debug.Assert(x > 0);
来源：https://ck.zhonguo4118.cn

[H08] 获取错误信息与堆栈
来源：https://wn.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://wb.zhonguo8118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://zp.zhonguo6118.cn

JS:   e.message;  e.stack
来源：https://cz.zhonguo4118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ut.zhonguo4118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://pm.zhonguo6118.cn

Go:   err.Error()
来源：https://fy.zhonguo5118.cn

Ruby: e.message;  e.backtrace
来源：https://yf.zhonguo6118.cn

C#:   e.Message;  e.StackTrace
来源：https://ea.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://fu.zhonguo3118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://yr.zhonguo4118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://zo.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://nh.zhonguo5118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://dc.zhonguo7118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ad.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://de.zhonguo1118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://jw.zhonguo7118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://dn.zhonguo4118.cn

[H10] 资源自动释放
来源：https://op.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://ut.zhonguo8118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://xf.zhonguo2118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://it.zhonguo2118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://db.zhonguo3118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://is.zhonguo5118.cn

Go:   defer f.Close()
来源：https://aj.zhonguo3118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://zp.zhonguo4118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://wk.zhonguo6118.cn

================================================================================
来源：https://xt.zhonguo7118.cn

I. 正则表达式
来源：https://zk.zhonguo3118.cn

================================================================================
来源：https://cv.zhonguo8118.cn

[I01] 判断是否匹配
来源：https://ag.zhonguo5118.cn


<!-- 参考信息 -->