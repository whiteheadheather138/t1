代发 wailian999

Java: class Admin extends User {}
来源：https://ls.zhonguo4118.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：https://gx.zhonguo3118.cn

Ruby: class Admin < User; end
来源：https://ik.zhonguo7118.cn

C#:   class Admin : User {}
来源：https://ep.zhonguo1118.cn

[G06] 重写方法
来源：https://fy.zhonguo1118.cn

Py:   def greet(self): return "admin"
来源：https://hf.zhonguo5118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://ur.zhonguo5118.cn

JS:   greet() { return "admin"; }
来源：https://cx.zhonguo1118.cn

TS:   greet(): string { return "admin"; }
来源：https://pe.zhonguo5118.cn

Java: @Override String greet() { return "admin"; }
来源：https://xy.zhonguo7118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://yo.zhonguo7118.cn

Ruby: def greet; "admin"; end
来源：https://xi.zhonguo4118.cn

C#:   public override string Greet() => "admin";
来源：https://pg.zhonguo5118.cn

[G07] 调用父类方法
来源：https://qw.zhonguo1118.cn

Py:   super().greet()
来源：https://ef.zhonguo7118.cn

PHP:  parent::greet();
来源：https://eu.zhonguo3118.cn

JS:   super.greet();
来源：https://st.zhonguo2118.cn

TS:   super.greet();
来源：https://px.zhonguo3118.cn

Java: super.greet();
来源：https://dk.zhonguo2118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://ln.zhonguo2118.cn

Ruby: super
来源：https://zi.zhonguo6118.cn

C#:   base.Greet();
来源：https://el.zhonguo3118.cn

[G08] 静态方法与属性
来源：https://hc.zhonguo6118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://rg.zhonguo5118.cn

PHP:  public static function f() {}
来源：https://xo.zhonguo8118.cn

JS:   static f() {}
来源：https://ek.zhonguo7118.cn

TS:   static f(): void {}
来源：https://fb.zhonguo5118.cn

Java: static void f() {}
来源：https://bl.zhonguo1118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://wh.zhonguo7118.cn

Ruby: def self.f; end
来源：https://cx.zhonguo4118.cn

C#:   public static void F() {}
来源：https://yi.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://vb.zhonguo5118.cn

Py:   from abc import ABC, abstractmethod
来源：https://ad.zhonguo8118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://rp.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://xh.zhonguo8118.cn

TS:   interface Shape { area(): number; }
来源：https://mb.zhonguo6118.cn

Java: interface Shape { double area(); }
来源：https://wc.zhonguo2118.cn

Go:   type Shape interface { Area() float64 }
来源：https://ux.zhonguo3118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ze.zhonguo1118.cn

C#:   interface IShape { double Area(); }
来源：https://xt.zhonguo2118.cn

[G10] 访问控制
来源：https://bu.zhonguo5118.cn

Py:   约定 _protected / __private（不强制）
来源：https://yl.zhonguo6118.cn

PHP:  public / protected / private
来源：https://bc.zhonguo1118.cn

JS:   #private 字段；其余公开
来源：https://eq.zhonguo2118.cn

TS:   public / protected / private
来源：https://fm.zhonguo1118.cn

Java: public / protected / private / 默认包级
来源：https://jt.zhonguo5118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://ua.zhonguo3118.cn

Ruby: public / protected / private
来源：https://bf.zhonguo7118.cn

C#:   public / protected / private / internal
来源：https://tn.zhonguo6118.cn

[G11] getter / setter
来源：https://wk.zhonguo8118.cn

Py:   @property 与 @x.setter
来源：https://hv.zhonguo1118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://ds.zhonguo8118.cn

JS:   get name() { return this._name; }
来源：https://ig.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://vx.zhonguo8118.cn

Java: public String getName() { return name; }
来源：https://qc.zhonguo5118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ng.zhonguo7118.cn

Ruby: attr_accessor :name
来源：https://xl.zhonguo4118.cn

C#:   public string Name { get; set; }
来源：https://bp.zhonguo7118.cn

[G12] 对象转字符串
来源：https://jv.zhonguo3118.cn

Py:   def __str__(self): return self.name
来源：https://nf.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://jf.zhonguo1118.cn

JS:   toString() { return this.name; }
来源：https://fs.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://ed.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://jv.zhonguo7118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://qi.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://uj.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://vr.zhonguo4118.cn

[G13] 判断对象类型
来源：https://il.zhonguo1118.cn

Py:   isinstance(u, User)
来源：https://ff.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://jt.zhonguo3118.cn

JS:   u instanceof User
来源：https://mj.zhonguo1118.cn

TS:   u instanceof User
来源：https://yt.zhonguo1118.cn

Java: u instanceof User
来源：https://jk.zhonguo1118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ne.zhonguo3118.cn

Ruby: u.is_a?(User)
来源：https://cf.zhonguo5118.cn

C#:   u is User
来源：https://ff.zhonguo5118.cn

[G14] 数据类 / record
来源：https://bx.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://bw.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://go.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://yd.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://in.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://ng.zhonguo2118.cn

Go:   type User struct { Name string; Age int }
来源：https://ed.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://kq.zhonguo8118.cn

C#:   record User(string Name, int Age);
来源：https://xc.zhonguo2118.cn

[G15] 枚举
来源：https://lu.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://az.zhonguo5118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://ut.zhonguo6118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://jg.zhonguo8118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://dq.zhonguo5118.cn

Java: enum Color { RED, GREEN }
来源：https://ix.zhonguo8118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://vo.zhonguo6118.cn

Ruby: Color = %i[red green].freeze
来源：https://od.zhonguo3118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://gi.zhonguo6118.cn

[G16] 对象转数组 / 字典
来源：https://vs.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ep.zhonguo8118.cn

PHP:  get_object_vars($obj);
来源：https://ah.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://pi.zhonguo6118.cn

TS:   Object.entries(obj)
来源：https://tt.zhonguo3118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://xr.zhonguo5118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://rt.zhonguo8118.cn

Ruby: obj.instance_variables
来源：https://zs.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://fp.zhonguo2118.cn

================================================================================
来源：https://dd.zhonguo8118.cn

H. 异常与错误处理
来源：https://di.zhonguo6118.cn

================================================================================
来源：https://hx.zhonguo5118.cn

[H01] try / catch 基础
来源：https://uz.zhonguo8118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://hk.zhonguo1118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://eb.zhonguo5118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://gk.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://yp.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://sl.zhonguo6118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://lt.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ol.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://qc.zhonguo1118.cn

[H02] finally / ensure 收尾
来源：https://nf.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://pk.zhonguo1118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://uq.zhonguo5118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://vj.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://tk.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://mf.zhonguo4118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://zl.zhonguo8118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://ys.zhonguo8118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://no.zhonguo4118.cn

[H03] 主动抛出异常
来源：https://cn.zhonguo2118.cn

Py:   raise ValueError("错误信息")
来源：https://io.zhonguo1118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://uf.zhonguo4118.cn

JS:   throw new Error("错误信息");
来源：https://iy.zhonguo5118.cn

TS:   throw new Error("错误信息");
来源：https://dv.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://er.zhonguo1118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ld.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ut.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://rf.zhonguo3118.cn

[H04] 自定义异常类型
来源：https://ue.zhonguo7118.cn

Py:   class MyError(Exception): pass
来源：https://fl.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://hw.zhonguo6118.cn

JS:   class MyError extends Error {}
来源：https://kj.zhonguo4118.cn

TS:   class MyError extends Error {}
来源：https://bg.zhonguo2118.cn

Java: class MyException extends RuntimeException {}
来源：https://kt.zhonguo8118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://cp.zhonguo2118.cn

Ruby: class MyError < StandardError; end
来源：https://xv.zhonguo8118.cn

C#:   class MyException : Exception {}
来源：https://ta.zhonguo8118.cn

[H05] 捕获特定类型
来源：https://av.zhonguo1118.cn

Py:   except ValueError as e:
来源：https://vq.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://ax.zhonguo7118.cn

JS:   if (e instanceof TypeError) {}
来源：https://yu.zhonguo6118.cn

TS:   if (e instanceof TypeError) {}
来源：https://nc.zhonguo1118.cn

Java: catch (IOException | SQLException e) {}
来源：https://de.zhonguo1118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://nu.zhonguo4118.cn

Ruby: rescue ArgumentError => e
来源：https://de.zhonguo8118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://zf.zhonguo3118.cn

[H06] 可选值 / 空值安全访问
来源：https://ua.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://fx.zhonguo6118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://ko.zhonguo7118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://ks.zhonguo1118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://lp.zhonguo1118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://bs.zhonguo6118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://pw.zhonguo1118.cn

Ruby: d&.dig(:a, :b)
来源：https://bt.zhonguo4118.cn

C#:   obj?.A?.B ?? default
来源：https://ra.zhonguo1118.cn

[H07] 断言
来源：https://xf.zhonguo1118.cn

Py:   assert x > 0, "必须为正"
来源：https://sa.zhonguo7118.cn

PHP:  assert($x > 0);
来源：https://pv.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://sq.zhonguo7118.cn

TS:   console.assert(x > 0);
来源：https://kt.zhonguo8118.cn

Java: assert x > 0 : "必须为正";
来源：https://gi.zhonguo5118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://vq.zhonguo3118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://bn.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://mx.zhonguo3118.cn

[H08] 获取错误信息与堆栈
来源：https://nk.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://zd.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://us.zhonguo2118.cn

JS:   e.message;  e.stack
来源：https://tb.zhonguo4118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://qq.zhonguo4118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://wz.zhonguo2118.cn

Go:   err.Error()
来源：https://ut.zhonguo2118.cn

Ruby: e.message;  e.backtrace
来源：https://oz.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://ls.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://oh.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://fz.zhonguo4118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://or.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ii.zhonguo6118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://ry.zhonguo4118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://pt.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://vv.zhonguo7118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://gt.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://qo.zhonguo3118.cn

[H10] 资源自动释放
来源：https://ag.zhonguo3118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://bc.zhonguo3118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://hk.zhonguo6118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://vu.zhonguo1118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://wi.zhonguo5118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://lb.zhonguo8118.cn

Go:   defer f.Close()
来源：https://ud.zhonguo1118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ud.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://qw.zhonguo7118.cn

================================================================================
来源：https://zk.zhonguo5118.cn

I. 正则表达式
来源：https://rr.zhonguo1118.cn

================================================================================
来源：https://gl.zhonguo8118.cn

[I01] 判断是否匹配
来源：https://rp.zhonguo7118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://yq.zhonguo8118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://qk.zhonguo2118.cn

JS:   /\d+/.test(s)
来源：https://hm.zhonguo5118.cn

TS:   /\d+/.test(s)
来源：https://ny.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://dq.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://dv.zhonguo2118.cn

Ruby: s.match?(/\d+/)
来源：https://la.zhonguo7118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://af.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://cg.zhonguo6118.cn

Py:   re.findall(r"\d+", s)
来源：https://ft.zhonguo5118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://nf.zhonguo3118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://tl.zhonguo5118.cn

TS:   s.match(/\d+/g)
来源：https://lr.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://mx.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://og.zhonguo6118.cn

Ruby: s.scan(/\d+/)
来源：https://es.zhonguo4118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ds.zhonguo6118.cn

[I03] 提取捕获分组
来源：https://sf.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://je.zhonguo1118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://qk.zhonguo3118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://zb.zhonguo1118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://hv.zhonguo5118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://bz.zhonguo3118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://dt.zhonguo6118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://yt.zhonguo7118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://qj.zhonguo7118.cn

[I04] 正则替换
来源：https://le.zhonguo1118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://yo.zhonguo6118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://hp.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://dg.zhonguo5118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://bn.zhonguo4118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://qj.zhonguo7118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://hb.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://yh.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ix.zhonguo1118.cn

[I05] 按正则拆分
来源：https://vg.zhonguo3118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://pe.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ew.zhonguo6118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ev.zhonguo8118.cn

TS:   s.split(/\s*,\s*/)
来源：https://oo.zhonguo3118.cn

Java: s.split("\\s*,\\s*")
来源：https://gk.zhonguo5118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://zh.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://qe.zhonguo8118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://hw.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://de.zhonguo8118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://iv.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://kd.zhonguo1118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://sn.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://um.zhonguo5118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://hz.zhonguo6118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://fl.zhonguo5118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://zr.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://jb.zhonguo2118.cn

[I07] 忽略大小写与多行模式
来源：https://yk.zhonguo8118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://zl.zhonguo5118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://fl.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://sc.zhonguo3118.cn

TS:   /error/gim
来源：https://zj.zhonguo6118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://gu.zhonguo1118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://be.zhonguo6118.cn

Ruby: s.scan(/error/i)
来源：https://nd.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://fa.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://fi.zhonguo1118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://lc.zhonguo8118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://zx.zhonguo6118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://kp.zhonguo8118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://ej.zhonguo2118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://vb.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://qm.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://lx.zhonguo1118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://np.zhonguo1118.cn

================================================================================
来源：https://px.zhonguo6118.cn

J. 日期与时间
来源：https://qd.zhonguo7118.cn

================================================================================
来源：https://xp.zhonguo4118.cn

[J01] 获取当前时间
来源：https://ai.zhonguo4118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://fq.zhonguo3118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ha.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://mg.zhonguo6118.cn

TS:   new Date();  Date.now()
来源：https://ub.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://cb.zhonguo4118.cn

Go:   time.Now()
来源：https://yz.zhonguo7118.cn

Ruby: Time.now
来源：https://qe.zhonguo4118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://io.zhonguo5118.cn

[J02] 格式化输出
来源：https://jn.zhonguo3118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ve.zhonguo3118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://vv.zhonguo8118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://vr.zhonguo8118.cn

TS:   d.toISOString()
来源：https://da.zhonguo5118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://rd.zhonguo3118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://ka.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://gs.zhonguo6118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://tv.zhonguo7118.cn

[J03] 字符串解析为日期
来源：https://sl.zhonguo1118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://oe.zhonguo7118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://hm.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://jw.zhonguo3118.cn

TS:   new Date("2024-01-02")
来源：https://dj.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://sx.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://hu.zhonguo5118.cn

Ruby: Date.parse("2024-01-02")
来源：https://wt.zhonguo2118.cn


<!-- 参考信息 -->