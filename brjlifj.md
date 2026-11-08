代发 wailian999

[G06] 重写方法
来源：https://rd.zhonguo8118.cn

Py:   def greet(self): return "admin"
来源：https://tc.zhonguo2118.cn

PHP:  public function greet(): string { return "admin"; }
来源：https://xj.zhonguo8118.cn

JS:   greet() { return "admin"; }
来源：https://tk.zhonguo4118.cn

TS:   greet(): string { return "admin"; }
来源：https://zz.zhonguo1118.cn

Java: @Override String greet() { return "admin"; }
来源：https://is.zhonguo1118.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：https://ek.zhonguo4118.cn

Ruby: def greet; "admin"; end
来源：https://qn.zhonguo1118.cn

C#:   public override string Greet() => "admin";
来源：https://qn.zhonguo4118.cn

[G07] 调用父类方法
来源：https://uz.zhonguo1118.cn

Py:   super().greet()
来源：https://id.zhonguo6118.cn

PHP:  parent::greet();
来源：https://jm.zhonguo7118.cn

JS:   super.greet();
来源：https://sg.zhonguo7118.cn

TS:   super.greet();
来源：https://ks.zhonguo5118.cn

Java: super.greet();
来源：https://lz.zhonguo3118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://kx.zhonguo2118.cn

Ruby: super
来源：https://fj.zhonguo3118.cn

C#:   base.Greet();
来源：https://iq.zhonguo8118.cn

[G08] 静态方法与属性
来源：https://hz.zhonguo7118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://aq.zhonguo6118.cn

PHP:  public static function f() {}
来源：https://rz.zhonguo2118.cn

JS:   static f() {}
来源：https://rz.zhonguo2118.cn

TS:   static f(): void {}
来源：https://tn.zhonguo5118.cn

Java: static void f() {}
来源：https://fc.zhonguo7118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://xd.zhonguo5118.cn

Ruby: def self.f; end
来源：https://dz.zhonguo8118.cn

C#:   public static void F() {}
来源：https://wx.zhonguo3118.cn

[G09] 接口 / 抽象类
来源：https://ss.zhonguo5118.cn

Py:   from abc import ABC, abstractmethod
来源：https://kd.zhonguo1118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://da.zhonguo6118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://bz.zhonguo6118.cn

TS:   interface Shape { area(): number; }
来源：https://ys.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://tk.zhonguo6118.cn

Go:   type Shape interface { Area() float64 }
来源：https://jz.zhonguo4118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://pv.zhonguo8118.cn

C#:   interface IShape { double Area(); }
来源：https://ch.zhonguo2118.cn

[G10] 访问控制
来源：https://tk.zhonguo7118.cn

Py:   约定 _protected / __private（不强制）
来源：https://he.zhonguo5118.cn

PHP:  public / protected / private
来源：https://zc.zhonguo4118.cn

JS:   #private 字段；其余公开
来源：https://hq.zhonguo6118.cn

TS:   public / protected / private
来源：https://ja.zhonguo8118.cn

Java: public / protected / private / 默认包级
来源：https://mq.zhonguo4118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://wz.zhonguo2118.cn

Ruby: public / protected / private
来源：https://hn.zhonguo1118.cn

C#:   public / protected / private / internal
来源：https://vi.zhonguo8118.cn

[G11] getter / setter
来源：https://wc.zhonguo5118.cn

Py:   @property 与 @x.setter
来源：https://aw.zhonguo2118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://zx.zhonguo7118.cn

JS:   get name() { return this._name; }
来源：https://yj.zhonguo7118.cn

TS:   get name(): string { return this._name; }
来源：https://if.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://eg.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://nz.zhonguo1118.cn

Ruby: attr_accessor :name
来源：https://ky.zhonguo4118.cn

C#:   public string Name { get; set; }
来源：https://co.zhonguo6118.cn

[G12] 对象转字符串
来源：https://qw.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://uc.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://nu.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://wz.zhonguo3118.cn

TS:   toString(): string { return this.name; }
来源：https://fk.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://dy.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://ip.zhonguo4118.cn

Ruby: def to_s; @name; end
来源：https://he.zhonguo1118.cn

C#:   public override string ToString() => Name;
来源：https://cu.zhonguo7118.cn

[G13] 判断对象类型
来源：https://ai.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://ld.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://ef.zhonguo4118.cn

JS:   u instanceof User
来源：https://vl.zhonguo1118.cn

TS:   u instanceof User
来源：https://lt.zhonguo4118.cn

Java: u instanceof User
来源：https://pp.zhonguo8118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://tz.zhonguo7118.cn

Ruby: u.is_a?(User)
来源：https://yd.zhonguo4118.cn

C#:   u is User
来源：https://po.zhonguo6118.cn

[G14] 数据类 / record
来源：https://lw.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://nt.zhonguo3118.cn

PHP:  // 用 readonly 属性模拟
来源：https://bf.zhonguo1118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://sl.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://od.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://gw.zhonguo7118.cn

Go:   type User struct { Name string; Age int }
来源：https://rp.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://ej.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://sp.zhonguo6118.cn

[G15] 枚举
来源：https://bb.zhonguo3118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://tg.zhonguo4118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://as.zhonguo4118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://wv.zhonguo6118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://hu.zhonguo8118.cn

Java: enum Color { RED, GREEN }
来源：https://kw.zhonguo7118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://rh.zhonguo3118.cn

Ruby: Color = %i[red green].freeze
来源：https://oc.zhonguo8118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://qs.zhonguo4118.cn

[G16] 对象转数组 / 字典
来源：https://sa.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://xt.zhonguo6118.cn

PHP:  get_object_vars($obj);
来源：https://ro.zhonguo8118.cn

JS:   Object.entries(obj)
来源：https://ky.zhonguo1118.cn

TS:   Object.entries(obj)
来源：https://os.zhonguo8118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://th.zhonguo8118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://ct.zhonguo2118.cn

Ruby: obj.instance_variables
来源：https://vy.zhonguo7118.cn

C#:   // 用反射或 System.Text.Json
来源：https://gh.zhonguo1118.cn

================================================================================
来源：https://mw.zhonguo5118.cn

H. 异常与错误处理
来源：https://bj.zhonguo6118.cn

================================================================================
来源：https://ig.zhonguo6118.cn

[H01] try / catch 基础
来源：https://gk.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://xt.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://rm.zhonguo7118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://tq.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://gq.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://vt.zhonguo8118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://fu.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://aj.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ym.zhonguo1118.cn

[H02] finally / ensure 收尾
来源：https://kp.zhonguo6118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://qm.zhonguo7118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://zt.zhonguo4118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://yj.zhonguo4118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ou.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://vf.zhonguo3118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ub.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://xz.zhonguo5118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://sv.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://wt.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://ue.zhonguo4118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://he.zhonguo4118.cn

JS:   throw new Error("错误信息");
来源：https://ox.zhonguo7118.cn

TS:   throw new Error("错误信息");
来源：https://xp.zhonguo7118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://nb.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://lb.zhonguo4118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://nt.zhonguo6118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://rw.zhonguo6118.cn

[H04] 自定义异常类型
来源：https://cu.zhonguo4118.cn

Py:   class MyError(Exception): pass
来源：https://wr.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://bz.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://jj.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://tv.zhonguo3118.cn

Java: class MyException extends RuntimeException {}
来源：https://vj.zhonguo6118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://sh.zhonguo7118.cn

Ruby: class MyError < StandardError; end
来源：https://yg.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://bq.zhonguo1118.cn

[H05] 捕获特定类型
来源：https://uf.zhonguo1118.cn

Py:   except ValueError as e:
来源：https://as.zhonguo5118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://gv.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://gk.zhonguo3118.cn

TS:   if (e instanceof TypeError) {}
来源：https://hc.zhonguo8118.cn

Java: catch (IOException | SQLException e) {}
来源：https://yj.zhonguo5118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://im.zhonguo4118.cn

Ruby: rescue ArgumentError => e
来源：https://mi.zhonguo2118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://dz.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://qh.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://iu.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://mf.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://hb.zhonguo1118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://zq.zhonguo3118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://np.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://dq.zhonguo4118.cn

Ruby: d&.dig(:a, :b)
来源：https://fq.zhonguo1118.cn

C#:   obj?.A?.B ?? default
来源：https://ku.zhonguo3118.cn

[H07] 断言
来源：https://wc.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://en.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://mz.zhonguo2118.cn

JS:   console.assert(x > 0);
来源：https://qc.zhonguo1118.cn

TS:   console.assert(x > 0);
来源：https://yy.zhonguo1118.cn

Java: assert x > 0 : "必须为正";
来源：https://pe.zhonguo4118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://yw.zhonguo8118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ih.zhonguo8118.cn

C#:   Debug.Assert(x > 0);
来源：https://rt.zhonguo8118.cn

[H08] 获取错误信息与堆栈
来源：https://ks.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://yk.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://wc.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://rw.zhonguo3118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://vb.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://uo.zhonguo3118.cn

Go:   err.Error()
来源：https://vy.zhonguo4118.cn

Ruby: e.message;  e.backtrace
来源：https://vp.zhonguo8118.cn

C#:   e.Message;  e.StackTrace
来源：https://ol.zhonguo3118.cn

[H09] 带错误码的异常
来源：https://pc.zhonguo3118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://fx.zhonguo6118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://ol.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://ot.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://hb.zhonguo6118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://jf.zhonguo5118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://xk.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://bc.zhonguo3118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://wu.zhonguo7118.cn

[H10] 资源自动释放
来源：https://il.zhonguo8118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://fh.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://fj.zhonguo3118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://ot.zhonguo4118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://oc.zhonguo2118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://ew.zhonguo7118.cn

Go:   defer f.Close()
来源：https://cw.zhonguo2118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://zs.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://tq.zhonguo8118.cn

================================================================================
来源：https://mp.zhonguo2118.cn

I. 正则表达式
来源：https://qf.zhonguo5118.cn

================================================================================
来源：https://sp.zhonguo3118.cn

[I01] 判断是否匹配
来源：https://rw.zhonguo4118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://pi.zhonguo7118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://iz.zhonguo2118.cn

JS:   /\d+/.test(s)
来源：https://hf.zhonguo3118.cn

TS:   /\d+/.test(s)
来源：https://hl.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://xk.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://dg.zhonguo4118.cn

Ruby: s.match?(/\d+/)
来源：https://sx.zhonguo2118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://ke.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://xe.zhonguo6118.cn

Py:   re.findall(r"\d+", s)
来源：https://og.zhonguo7118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://fw.zhonguo4118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://ur.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://tg.zhonguo8118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://wz.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://eh.zhonguo1118.cn

Ruby: s.scan(/\d+/)
来源：https://bg.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ca.zhonguo4118.cn

[I03] 提取捕获分组
来源：https://ok.zhonguo2118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://zv.zhonguo1118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ho.zhonguo6118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://mb.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://qg.zhonguo8118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://lj.zhonguo3118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://xp.zhonguo1118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://hj.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://tg.zhonguo4118.cn

[I04] 正则替换
来源：https://hu.zhonguo6118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://xu.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://ss.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://fp.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://bg.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://nj.zhonguo7118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://wj.zhonguo8118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://de.zhonguo3118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://of.zhonguo6118.cn

[I05] 按正则拆分
来源：https://bv.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://cb.zhonguo7118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ti.zhonguo8118.cn

JS:   s.split(/\s*,\s*/)
来源：https://yt.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://dj.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://dl.zhonguo3118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://jx.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://vw.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ok.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://or.zhonguo4118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://li.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://cy.zhonguo5118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://eo.zhonguo5118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://ph.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://dl.zhonguo3118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://fs.zhonguo4118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://pw.zhonguo2118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://qv.zhonguo3118.cn

[I07] 忽略大小写与多行模式
来源：https://fr.zhonguo6118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://rh.zhonguo1118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://fp.zhonguo7118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://ql.zhonguo8118.cn

TS:   /error/gim
来源：https://ro.zhonguo3118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://yc.zhonguo7118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://ub.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://mn.zhonguo1118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://cm.zhonguo7118.cn

[I08] 贪婪与非贪婪匹配
来源：https://pi.zhonguo4118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ju.zhonguo2118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://or.zhonguo7118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://hr.zhonguo3118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://qe.zhonguo5118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ir.zhonguo1118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://go.zhonguo6118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://of.zhonguo5118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://qw.zhonguo4118.cn

================================================================================
来源：https://fq.zhonguo5118.cn

J. 日期与时间
来源：https://ed.zhonguo1118.cn

================================================================================
来源：https://fd.zhonguo1118.cn

[J01] 获取当前时间
来源：https://ux.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://bi.zhonguo6118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://sf.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://rw.zhonguo1118.cn

TS:   new Date();  Date.now()
来源：https://bt.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://tw.zhonguo2118.cn

Go:   time.Now()
来源：https://op.zhonguo8118.cn

Ruby: Time.now
来源：https://yw.zhonguo1118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://xc.zhonguo3118.cn

[J02] 格式化输出
来源：https://hb.zhonguo1118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://yf.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ev.zhonguo4118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://gq.zhonguo2118.cn

TS:   d.toISOString()
来源：https://nz.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://pc.zhonguo5118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://dr.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://jt.zhonguo1118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://pu.zhonguo6118.cn

[J03] 字符串解析为日期
来源：https://jk.zhonguo4118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://wr.zhonguo2118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://dy.zhonguo2118.cn

JS:   new Date("2024-01-02")
来源：https://nz.zhonguo2118.cn

TS:   new Date("2024-01-02")
来源：https://rq.zhonguo3118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://pe.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://za.zhonguo3118.cn

Ruby: Date.parse("2024-01-02")
来源：https://zo.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ru.zhonguo4118.cn

[J04] 时间戳与日期互转
来源：https://zg.zhonguo2118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://qo.zhonguo4118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://pl.zhonguo7118.cn


<!-- 参考信息 -->