代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：https://vi.zhonguo3118.cn

[F10] 取文件扩展名 / 文件名
来源：https://kl.zhonguo1118.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：https://qz.zhonguo1118.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：https://fx.zhonguo3118.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：https://jr.zhonguo2118.cn

TS:   path.extname("a.txt")
来源：https://py.zhonguo4118.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：https://fn.zhonguo3118.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：https://ap.zhonguo7118.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：https://xn.zhonguo5118.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：https://os.zhonguo1118.cn

[F11] 复制与移动文件
来源：https://so.zhonguo4118.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：https://ad.zhonguo5118.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：https://xs.zhonguo8118.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://cw.zhonguo4118.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：https://jv.zhonguo2118.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：https://ct.zhonguo3118.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：https://vq.zhonguo1118.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：https://oh.zhonguo5118.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：https://er.zhonguo6118.cn

[F12] CSV 读写
来源：https://mm.zhonguo4118.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://dx.zhonguo6118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://iz.zhonguo4118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://na.zhonguo5118.cn

TS:   // 同上
来源：https://xe.zhonguo7118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://mg.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://ck.zhonguo2118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://jg.zhonguo7118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://ro.zhonguo2118.cn

================================================================================
来源：https://gm.zhonguo7118.cn

G. 面向对象
来源：https://pf.zhonguo3118.cn

================================================================================
来源：https://an.zhonguo4118.cn

[G01] 定义类
来源：https://ca.zhonguo6118.cn

Py:   class User: pass
来源：https://ri.zhonguo3118.cn

PHP:  class User {}
来源：https://lm.zhonguo8118.cn

JS:   class User {}
来源：https://xs.zhonguo1118.cn

TS:   class User { name: string = ""; }
来源：https://us.zhonguo5118.cn

Java: class User {}
来源：https://ju.zhonguo4118.cn

Go:   type User struct { Name string }
来源：https://eo.zhonguo7118.cn

Ruby: class User; end
来源：https://wd.zhonguo3118.cn

C#:   class User {}
来源：https://td.zhonguo5118.cn

[G02] 构造函数
来源：https://bp.zhonguo5118.cn

Py:   def __init__(self, name): self.name = name
来源：https://by.zhonguo5118.cn

PHP:  public function __construct(public string $name) {}
来源：https://vw.zhonguo8118.cn

JS:   constructor(name) { this.name = name; }
来源：https://lf.zhonguo2118.cn

TS:   constructor(public name: string) {}
来源：https://do.zhonguo3118.cn

Java: User(String name) { this.name = name; }
来源：https://uf.zhonguo1118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://ni.zhonguo2118.cn

Ruby: def initialize(name); @name = name; end
来源：https://ex.zhonguo7118.cn

C#:   public User(string name) { Name = name; }
来源：https://zz.zhonguo2118.cn

[G03] 实例属性
来源：https://ry.zhonguo2118.cn

Py:   self.name = "x"
来源：https://qc.zhonguo3118.cn

PHP:  public string $name = "x";
来源：https://pk.zhonguo8118.cn

JS:   this.name = "x";
来源：https://kd.zhonguo1118.cn

TS:   name: string = "x";
来源：https://ww.zhonguo8118.cn

Java: private String name;
来源：https://nk.zhonguo6118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://rr.zhonguo3118.cn

Ruby: @name = "x"
来源：https://hd.zhonguo8118.cn

C#:   public string Name { get; set; } = "x";
来源：https://vd.zhonguo5118.cn

[G04] 定义方法
来源：https://kz.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://qp.zhonguo7118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://bv.zhonguo5118.cn

JS:   greet() { return this.name; }
来源：https://mp.zhonguo4118.cn

TS:   greet(): string { return this.name; }
来源：https://tq.zhonguo3118.cn

Java: String greet() { return name; }
来源：https://yn.zhonguo6118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://nf.zhonguo1118.cn

Ruby: def greet; @name; end
来源：https://ro.zhonguo2118.cn

C#:   public string Greet() => Name;
来源：https://zi.zhonguo4118.cn

[G05] 继承
来源：https://xg.zhonguo4118.cn

Py:   class Admin(User): pass
来源：https://az.zhonguo6118.cn

PHP:  class Admin extends User {}
来源：https://dl.zhonguo4118.cn

JS:   class Admin extends User {}
来源：https://dm.zhonguo4118.cn

TS:   class Admin extends User {}
来源：https://nu.zhonguo7118.cn

Java: class Admin extends User {}
来源：https://qi.zhonguo2118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://wa.zhonguo4118.cn

Ruby: class Admin < User; end
来源：https://cx.zhonguo3118.cn

C#:   class Admin : User {}
来源：https://pj.zhonguo3118.cn

[G06] 重写方法
来源：https://ru.zhonguo1118.cn

Py:   def greet(self): return "admin"
来源：https://ic.zhonguo7118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://wh.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://dc.zhonguo5118.cn

TS:   greet(): string { return "admin"; }
来源：https://wc.zhonguo6118.cn

Java: @Override String greet() { return "admin"; }
来源：https://gf.zhonguo6118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://gz.zhonguo7118.cn

Ruby: def greet; "admin"; end
来源：https://my.zhonguo1118.cn

C#:   public override string Greet() => "admin";
来源：https://qm.zhonguo1118.cn

[G07] 调用父类方法
来源：https://ob.zhonguo1118.cn

Py:   super().greet()
来源：https://hy.zhonguo6118.cn

PHP:  parent::greet();
来源：https://nn.zhonguo2118.cn

JS:   super.greet();
来源：https://tc.zhonguo6118.cn

TS:   super.greet();
来源：https://tk.zhonguo4118.cn

Java: super.greet();
来源：https://cd.zhonguo5118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ki.zhonguo6118.cn

Ruby: super
来源：https://hl.zhonguo2118.cn

C#:   base.Greet();
来源：https://uu.zhonguo5118.cn

[G08] 静态方法与属性
来源：https://kp.zhonguo3118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://ys.zhonguo2118.cn

PHP:  public static function f() {}
来源：https://xa.zhonguo5118.cn

JS:   static f() {}
来源：https://vu.zhonguo6118.cn

TS:   static f(): void {}
来源：https://mc.zhonguo3118.cn

Java: static void f() {}
来源：https://ue.zhonguo4118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://uz.zhonguo2118.cn

Ruby: def self.f; end
来源：https://dw.zhonguo8118.cn

C#:   public static void F() {}
来源：https://pg.zhonguo6118.cn

[G09] 接口 / 抽象类
来源：https://nn.zhonguo5118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ly.zhonguo5118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://ye.zhonguo5118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://un.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://lq.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://wh.zhonguo2118.cn

Go:   type Shape interface { Area() float64 }
来源：https://av.zhonguo8118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ic.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://sk.zhonguo4118.cn

[G10] 访问控制
来源：https://kx.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://xu.zhonguo1118.cn

PHP:  public / protected / private
来源：https://qs.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://ym.zhonguo3118.cn

TS:   public / protected / private
来源：https://ey.zhonguo2118.cn

Java: public / protected / private / 默认包级
来源：https://aj.zhonguo7118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://do.zhonguo5118.cn

Ruby: public / protected / private
来源：https://kb.zhonguo7118.cn

C#:   public / protected / private / internal
来源：https://su.zhonguo6118.cn

[G11] getter / setter
来源：https://yw.zhonguo7118.cn

Py:   @property 与 @x.setter
来源：https://uh.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://hz.zhonguo4118.cn

JS:   get name() { return this._name; }
来源：https://fq.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://dg.zhonguo8118.cn

Java: public String getName() { return name; }
来源：https://im.zhonguo2118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://xo.zhonguo3118.cn

Ruby: attr_accessor :name
来源：https://px.zhonguo7118.cn

C#:   public string Name { get; set; }
来源：https://ey.zhonguo4118.cn

[G12] 对象转字符串
来源：https://tu.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://tz.zhonguo2118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://rx.zhonguo7118.cn

JS:   toString() { return this.name; }
来源：https://zr.zhonguo5118.cn

TS:   toString(): string { return this.name; }
来源：https://yw.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://ea.zhonguo6118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://gc.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://pf.zhonguo4118.cn

C#:   public override string ToString() => Name;
来源：https://fx.zhonguo8118.cn

[G13] 判断对象类型
来源：https://yh.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://gb.zhonguo3118.cn

PHP:  $u instanceof User
来源：https://hp.zhonguo8118.cn

JS:   u instanceof User
来源：https://ax.zhonguo7118.cn

TS:   u instanceof User
来源：https://cf.zhonguo2118.cn

Java: u instanceof User
来源：https://bo.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://qe.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://on.zhonguo5118.cn

C#:   u is User
来源：https://du.zhonguo2118.cn

[G14] 数据类 / record
来源：https://xj.zhonguo1118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://kd.zhonguo3118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ge.zhonguo2118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://es.zhonguo5118.cn

TS:   type User = { name: string; age: number };
来源：https://fs.zhonguo3118.cn

Java: record User(String name, int age) {}
来源：https://up.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://gy.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://zy.zhonguo1118.cn

C#:   record User(string Name, int Age);
来源：https://zs.zhonguo2118.cn

[G15] 枚举
来源：https://cz.zhonguo5118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ma.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://oy.zhonguo3118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://zz.zhonguo5118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://mw.zhonguo4118.cn

Java: enum Color { RED, GREEN }
来源：https://ka.zhonguo6118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ns.zhonguo1118.cn

Ruby: Color = %i[red green].freeze
来源：https://yb.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://nj.zhonguo6118.cn

[G16] 对象转数组 / 字典
来源：https://kt.zhonguo8118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://cw.zhonguo5118.cn

PHP:  get_object_vars($obj);
来源：https://kn.zhonguo3118.cn

JS:   Object.entries(obj)
来源：https://tn.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://kw.zhonguo3118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://qr.zhonguo6118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://ui.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://ot.zhonguo3118.cn

C#:   // 用反射或 System.Text.Json
来源：https://zp.zhonguo6118.cn

================================================================================
来源：https://iy.zhonguo3118.cn

H. 异常与错误处理
来源：https://ng.zhonguo1118.cn

================================================================================
来源：https://cu.zhonguo7118.cn

[H01] try / catch 基础
来源：https://ut.zhonguo8118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://dm.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://si.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://wu.zhonguo6118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://pl.zhonguo7118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://pv.zhonguo1118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://iw.zhonguo4118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ln.zhonguo6118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ot.zhonguo5118.cn

[H02] finally / ensure 收尾
来源：https://fw.zhonguo3118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://em.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://wb.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://kq.zhonguo7118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://iq.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://em.zhonguo2118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://mx.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://et.zhonguo2118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://il.zhonguo7118.cn

[H03] 主动抛出异常
来源：https://zz.zhonguo1118.cn

Py:   raise ValueError("错误信息")
来源：https://dl.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ze.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://lx.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://jb.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://ec.zhonguo2118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://fq.zhonguo1118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://zl.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://wh.zhonguo6118.cn

[H04] 自定义异常类型
来源：https://mf.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://zf.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://rs.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://jg.zhonguo7118.cn

TS:   class MyError extends Error {}
来源：https://rn.zhonguo2118.cn

Java: class MyException extends RuntimeException {}
来源：https://qb.zhonguo4118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://jy.zhonguo8118.cn

Ruby: class MyError < StandardError; end
来源：https://ot.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://ki.zhonguo6118.cn

[H05] 捕获特定类型
来源：https://ab.zhonguo1118.cn

Py:   except ValueError as e:
来源：https://hy.zhonguo5118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://is.zhonguo3118.cn

JS:   if (e instanceof TypeError) {}
来源：https://pe.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://bm.zhonguo8118.cn

Java: catch (IOException | SQLException e) {}
来源：https://kr.zhonguo3118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://yl.zhonguo8118.cn

Ruby: rescue ArgumentError => e
来源：https://da.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://pn.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://ak.zhonguo8118.cn

Py:   value = d.get("k") or default
来源：https://xg.zhonguo8118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://py.zhonguo5118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vz.zhonguo7118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://vg.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://wv.zhonguo5118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ln.zhonguo2118.cn

Ruby: d&.dig(:a, :b)
来源：https://jn.zhonguo7118.cn

C#:   obj?.A?.B ?? default
来源：https://cv.zhonguo8118.cn

[H07] 断言
来源：https://se.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://ao.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://gb.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://dp.zhonguo6118.cn

TS:   console.assert(x > 0);
来源：https://jm.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://jf.zhonguo5118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://zf.zhonguo1118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ij.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://mt.zhonguo3118.cn

[H08] 获取错误信息与堆栈
来源：https://uj.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://ta.zhonguo7118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://tf.zhonguo8118.cn

JS:   e.message;  e.stack
来源：https://oj.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://rw.zhonguo7118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://aa.zhonguo2118.cn

Go:   err.Error()
来源：https://fd.zhonguo5118.cn

Ruby: e.message;  e.backtrace
来源：https://pm.zhonguo2118.cn

C#:   e.Message;  e.StackTrace
来源：https://qj.zhonguo4118.cn

[H09] 带错误码的异常
来源：https://az.zhonguo7118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://lu.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://cn.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://zd.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://ti.zhonguo3118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://tf.zhonguo2118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://am.zhonguo4118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ny.zhonguo4118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ff.zhonguo3118.cn

[H10] 资源自动释放
来源：https://ps.zhonguo3118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://yn.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ae.zhonguo1118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://xa.zhonguo2118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://su.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://hx.zhonguo2118.cn

Go:   defer f.Close()
来源：https://eo.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://zu.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://xo.zhonguo8118.cn

================================================================================
来源：https://rk.zhonguo3118.cn

I. 正则表达式
来源：https://gl.zhonguo5118.cn

================================================================================
来源：https://tv.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://th.zhonguo6118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://kl.zhonguo6118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://xs.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://jj.zhonguo1118.cn

TS:   /\d+/.test(s)
来源：https://lw.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://rg.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://vh.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://pz.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://jw.zhonguo2118.cn

[I02] 提取所有匹配
来源：https://as.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://wp.zhonguo2118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://eq.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://jz.zhonguo7118.cn

TS:   s.match(/\d+/g)
来源：https://fl.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://pu.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://de.zhonguo1118.cn

Ruby: s.scan(/\d+/)
来源：https://rr.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://rs.zhonguo2118.cn

[I03] 提取捕获分组
来源：https://kk.zhonguo7118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://qr.zhonguo4118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ne.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://st.zhonguo5118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://ac.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://uy.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://zr.zhonguo6118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://sf.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://av.zhonguo1118.cn

[I04] 正则替换
来源：https://vc.zhonguo8118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://aw.zhonguo8118.cn


<!-- 参考信息 -->