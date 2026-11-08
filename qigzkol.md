代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：https://uh.zhonguo4118.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：https://fi.zhonguo8118.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：https://ye.zhonguo8118.cn

TS:   // 同上
来源：https://yd.zhonguo1118.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：https://gq.zhonguo2118.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：https://lf.zhonguo3118.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：https://kq.zhonguo4118.cn

C#:   // 无内置：用 CsvHelper 库
来源：https://dw.zhonguo3118.cn

================================================================================
来源：https://gw.zhonguo4118.cn

G. 面向对象
来源：https://ut.zhonguo6118.cn

================================================================================
来源：https://uf.zhonguo7118.cn

[G01] 定义类
来源：https://ma.zhonguo3118.cn

Py:   class User: pass
来源：https://mg.zhonguo5118.cn

PHP:  class User {}
来源：https://np.zhonguo3118.cn

JS:   class User {}
来源：https://by.zhonguo3118.cn

TS:   class User { name: string = ""; }
来源：https://kd.zhonguo2118.cn

Java: class User {}
来源：https://cm.zhonguo7118.cn

Go:   type User struct { Name string }
来源：https://yx.zhonguo2118.cn

Ruby: class User; end
来源：https://sh.zhonguo1118.cn

C#:   class User {}
来源：https://zs.zhonguo5118.cn

[G02] 构造函数
来源：https://nu.zhonguo7118.cn

Py:   def __init__(self, name): self.name = name
来源：https://ne.zhonguo8118.cn

PHP:  public function __construct(public string $name) {}
来源：https://tc.zhonguo6118.cn

JS:   constructor(name) { this.name = name; }
来源：https://ta.zhonguo4118.cn

TS:   constructor(public name: string) {}
来源：https://cv.zhonguo3118.cn

Java: User(String name) { this.name = name; }
来源：https://rh.zhonguo6118.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：https://rj.zhonguo6118.cn

Ruby: def initialize(name); @name = name; end
来源：https://ei.zhonguo8118.cn

C#:   public User(string name) { Name = name; }
来源：https://xm.zhonguo3118.cn

[G03] 实例属性
来源：https://sb.zhonguo3118.cn

Py:   self.name = "x"
来源：https://mx.zhonguo8118.cn

PHP:  public string $name = "x";
来源：https://vr.zhonguo7118.cn

JS:   this.name = "x";
来源：https://fd.zhonguo7118.cn

TS:   name: string = "x";
来源：https://vx.zhonguo8118.cn

Java: private String name;
来源：https://qd.zhonguo3118.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：https://lm.zhonguo6118.cn

Ruby: @name = "x"
来源：https://xg.zhonguo6118.cn

C#:   public string Name { get; set; } = "x";
来源：https://kv.zhonguo2118.cn

[G04] 定义方法
来源：https://jm.zhonguo5118.cn

Py:   def greet(self): return self.name
来源：https://pp.zhonguo2118.cn

PHP:  public function greet(): string { return $this->name; }
来源：https://yf.zhonguo5118.cn

JS:   greet() { return this.name; }
来源：https://ro.zhonguo5118.cn

TS:   greet(): string { return this.name; }
来源：https://sz.zhonguo7118.cn

Java: String greet() { return name; }
来源：https://vz.zhonguo3118.cn

Go:   func (u User) Greet() string { return u.Name }
来源：https://hh.zhonguo7118.cn

Ruby: def greet; @name; end
来源：https://ux.zhonguo5118.cn

C#:   public string Greet() => Name;
来源：https://xo.zhonguo6118.cn

[G05] 继承
来源：https://hu.zhonguo8118.cn

Py:   class Admin(User): pass
来源：https://zx.zhonguo8118.cn

PHP:  class Admin extends User {}
来源：https://rv.zhonguo3118.cn

JS:   class Admin extends User {}
来源：https://jd.zhonguo6118.cn

TS:   class Admin extends User {}
来源：https://lq.zhonguo8118.cn

Java: class Admin extends User {}
来源：https://bv.zhonguo3118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://kk.zhonguo1118.cn

Ruby: class Admin < User; end
来源：https://df.zhonguo3118.cn

C#:   class Admin : User {}
来源：https://aa.zhonguo1118.cn

[G06] 重写方法
来源：https://wf.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://ia.zhonguo2118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://wr.zhonguo2118.cn

JS:   greet() { return "admin"; }
来源：https://gf.zhonguo8118.cn

TS:   greet(): string { return "admin"; }
来源：https://dv.zhonguo4118.cn

Java: @Override String greet() { return "admin"; }
来源：https://bs.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://la.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://cu.zhonguo6118.cn

C#:   public override string Greet() => "admin";
来源：https://zm.zhonguo8118.cn

[G07] 调用父类方法
来源：https://wj.zhonguo5118.cn

Py:   super().greet()
来源：https://eg.zhonguo4118.cn

PHP:  parent::greet();
来源：https://yj.zhonguo8118.cn

JS:   super.greet();
来源：https://bk.zhonguo6118.cn

TS:   super.greet();
来源：https://qi.zhonguo8118.cn

Java: super.greet();
来源：https://yy.zhonguo4118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://xe.zhonguo2118.cn

Ruby: super
来源：https://qh.zhonguo8118.cn

C#:   base.Greet();
来源：https://at.zhonguo3118.cn

[G08] 静态方法与属性
来源：https://yb.zhonguo5118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://jv.zhonguo7118.cn

PHP:  public static function f() {}
来源：https://hj.zhonguo4118.cn

JS:   static f() {}
来源：https://vf.zhonguo8118.cn

TS:   static f(): void {}
来源：https://xn.zhonguo3118.cn

Java: static void f() {}
来源：https://uk.zhonguo7118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://nv.zhonguo5118.cn

Ruby: def self.f; end
来源：https://tz.zhonguo1118.cn

C#:   public static void F() {}
来源：https://it.zhonguo2118.cn

[G09] 接口 / 抽象类
来源：https://qd.zhonguo8118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ve.zhonguo4118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://kf.zhonguo6118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://px.zhonguo5118.cn

TS:   interface Shape { area(): number; }
来源：https://gv.zhonguo7118.cn

Java: interface Shape { double area(); }
来源：https://em.zhonguo3118.cn

Go:   type Shape interface { Area() float64 }
来源：https://tv.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://np.zhonguo2118.cn

C#:   interface IShape { double Area(); }
来源：https://vg.zhonguo8118.cn

[G10] 访问控制
来源：https://iy.zhonguo4118.cn

Py:   约定 _protected / __private（不强制）
来源：https://la.zhonguo7118.cn

PHP:  public / protected / private
来源：https://jp.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://mq.zhonguo7118.cn

TS:   public / protected / private
来源：https://cs.zhonguo7118.cn

Java: public / protected / private / 默认包级
来源：https://up.zhonguo2118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://jk.zhonguo4118.cn

Ruby: public / protected / private
来源：https://le.zhonguo5118.cn

C#:   public / protected / private / internal
来源：https://ba.zhonguo7118.cn

[G11] getter / setter
来源：https://ia.zhonguo2118.cn

Py:   @property 与 @x.setter
来源：https://db.zhonguo3118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://bo.zhonguo2118.cn

JS:   get name() { return this._name; }
来源：https://tw.zhonguo6118.cn

TS:   get name(): string { return this._name; }
来源：https://cd.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://cx.zhonguo1118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://wk.zhonguo6118.cn

Ruby: attr_accessor :name
来源：https://tk.zhonguo8118.cn

C#:   public string Name { get; set; }
来源：https://gi.zhonguo3118.cn

[G12] 对象转字符串
来源：https://wf.zhonguo8118.cn

Py:   def __str__(self): return self.name
来源：https://ec.zhonguo2118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://wo.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://qn.zhonguo2118.cn

TS:   toString(): string { return this.name; }
来源：https://sp.zhonguo5118.cn

Java: @Override public String toString() { return name; }
来源：https://qt.zhonguo5118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://hb.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://xk.zhonguo7118.cn

C#:   public override string ToString() => Name;
来源：https://sl.zhonguo2118.cn

[G13] 判断对象类型
来源：https://kh.zhonguo4118.cn

Py:   isinstance(u, User)
来源：https://th.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://no.zhonguo2118.cn

JS:   u instanceof User
来源：https://kw.zhonguo3118.cn

TS:   u instanceof User
来源：https://qn.zhonguo6118.cn

Java: u instanceof User
来源：https://cm.zhonguo7118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://xn.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://wy.zhonguo6118.cn

C#:   u is User
来源：https://vb.zhonguo5118.cn

[G14] 数据类 / record
来源：https://uj.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://nk.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://qb.zhonguo5118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ms.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://ho.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://ui.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://lb.zhonguo6118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://zg.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://qj.zhonguo5118.cn

[G15] 枚举
来源：https://rx.zhonguo8118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://az.zhonguo3118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://gj.zhonguo6118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://jn.zhonguo1118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://iv.zhonguo6118.cn

Java: enum Color { RED, GREEN }
来源：https://ib.zhonguo6118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://zm.zhonguo5118.cn

Ruby: Color = %i[red green].freeze
来源：https://ki.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://qe.zhonguo7118.cn

[G16] 对象转数组 / 字典
来源：https://bn.zhonguo2118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://gq.zhonguo3118.cn

PHP:  get_object_vars($obj);
来源：https://nb.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://ja.zhonguo7118.cn

TS:   Object.entries(obj)
来源：https://yn.zhonguo5118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://sk.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://az.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://vz.zhonguo6118.cn

C#:   // 用反射或 System.Text.Json
来源：https://sp.zhonguo7118.cn

================================================================================
来源：https://pe.zhonguo7118.cn

H. 异常与错误处理
来源：https://jz.zhonguo7118.cn

================================================================================
来源：https://bf.zhonguo3118.cn

[H01] try / catch 基础
来源：https://jp.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://tv.zhonguo3118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://zy.zhonguo7118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://gk.zhonguo7118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sn.zhonguo2118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://io.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://ye.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://xg.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://oo.zhonguo2118.cn

[H02] finally / ensure 收尾
来源：https://rp.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://ls.zhonguo8118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://im.zhonguo8118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://zs.zhonguo3118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://jf.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://mf.zhonguo3118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://af.zhonguo1118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://xv.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://wg.zhonguo5118.cn

[H03] 主动抛出异常
来源：https://ua.zhonguo5118.cn

Py:   raise ValueError("错误信息")
来源：https://mp.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://wj.zhonguo2118.cn

JS:   throw new Error("错误信息");
来源：https://cu.zhonguo1118.cn

TS:   throw new Error("错误信息");
来源：https://av.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://cv.zhonguo7118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://gq.zhonguo6118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ce.zhonguo4118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://uu.zhonguo6118.cn

[H04] 自定义异常类型
来源：https://hs.zhonguo4118.cn

Py:   class MyError(Exception): pass
来源：https://wt.zhonguo6118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://xx.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://hm.zhonguo6118.cn

TS:   class MyError extends Error {}
来源：https://pe.zhonguo5118.cn

Java: class MyException extends RuntimeException {}
来源：https://es.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://ov.zhonguo4118.cn

Ruby: class MyError < StandardError; end
来源：https://hz.zhonguo3118.cn

C#:   class MyException : Exception {}
来源：https://vx.zhonguo3118.cn

[H05] 捕获特定类型
来源：https://qm.zhonguo7118.cn

Py:   except ValueError as e:
来源：https://pl.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://bs.zhonguo2118.cn

JS:   if (e instanceof TypeError) {}
来源：https://mb.zhonguo5118.cn

TS:   if (e instanceof TypeError) {}
来源：https://pv.zhonguo3118.cn

Java: catch (IOException | SQLException e) {}
来源：https://hv.zhonguo8118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://bc.zhonguo2118.cn

Ruby: rescue ArgumentError => e
来源：https://li.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://cm.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://vs.zhonguo4118.cn

Py:   value = d.get("k") or default
来源：https://mc.zhonguo4118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://mh.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://vq.zhonguo6118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://yf.zhonguo5118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ni.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://mi.zhonguo5118.cn

Ruby: d&.dig(:a, :b)
来源：https://oz.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://do.zhonguo7118.cn

[H07] 断言
来源：https://ae.zhonguo1118.cn

Py:   assert x > 0, "必须为正"
来源：https://fi.zhonguo8118.cn

PHP:  assert($x > 0);
来源：https://db.zhonguo8118.cn

JS:   console.assert(x > 0);
来源：https://tb.zhonguo6118.cn

TS:   console.assert(x > 0);
来源：https://iw.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://js.zhonguo3118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://uf.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://tk.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://gg.zhonguo2118.cn

[H08] 获取错误信息与堆栈
来源：https://wq.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://qb.zhonguo5118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://cj.zhonguo7118.cn

JS:   e.message;  e.stack
来源：https://xt.zhonguo2118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ab.zhonguo6118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://yw.zhonguo1118.cn

Go:   err.Error()
来源：https://xb.zhonguo4118.cn

Ruby: e.message;  e.backtrace
来源：https://xe.zhonguo6118.cn

C#:   e.Message;  e.StackTrace
来源：https://nc.zhonguo2118.cn

[H09] 带错误码的异常
来源：https://px.zhonguo4118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://iu.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://wq.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://yv.zhonguo1118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://dh.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://kj.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://ae.zhonguo5118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://kf.zhonguo8118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://el.zhonguo8118.cn

[H10] 资源自动释放
来源：https://nx.zhonguo6118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://mw.zhonguo7118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://bm.zhonguo2118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://ew.zhonguo5118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://qf.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://dv.zhonguo5118.cn

Go:   defer f.Close()
来源：https://ts.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://jc.zhonguo6118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://lv.zhonguo4118.cn

================================================================================
来源：https://lb.zhonguo7118.cn

I. 正则表达式
来源：https://nx.zhonguo4118.cn

================================================================================
来源：https://ig.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://hr.zhonguo4118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://za.zhonguo5118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://oi.zhonguo1118.cn

JS:   /\d+/.test(s)
来源：https://kp.zhonguo1118.cn

TS:   /\d+/.test(s)
来源：https://ij.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://ks.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://pn.zhonguo7118.cn

Ruby: s.match?(/\d+/)
来源：https://sn.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://my.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://vd.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://ap.zhonguo2118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://iq.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://bi.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://hq.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://bh.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://nk.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://hv.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ar.zhonguo2118.cn

[I03] 提取捕获分组
来源：https://my.zhonguo8118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://qz.zhonguo4118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://kl.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://up.zhonguo7118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://rv.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://ue.zhonguo7118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://pc.zhonguo8118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://kj.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://zf.zhonguo7118.cn

[I04] 正则替换
来源：https://pf.zhonguo3118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://dy.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://kd.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://hf.zhonguo7118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://hq.zhonguo4118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://os.zhonguo1118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://ht.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://dk.zhonguo2118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://hc.zhonguo4118.cn

[I05] 按正则拆分
来源：https://vk.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://ry.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://da.zhonguo4118.cn

JS:   s.split(/\s*,\s*/)
来源：https://xo.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://mq.zhonguo2118.cn

Java: s.split("\\s*,\\s*")
来源：https://th.zhonguo3118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://rt.zhonguo2118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://jp.zhonguo7118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://yk.zhonguo2118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://cg.zhonguo4118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://rv.zhonguo8118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://jl.zhonguo4118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://ag.zhonguo7118.cn


<!-- 参考信息 -->