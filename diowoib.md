代发 wailian999

JS:   super.greet();
来源：https://tm.zhonguo6118.cn

TS:   super.greet();
来源：https://re.zhonguo4118.cn

Java: super.greet();
来源：https://ai.zhonguo6118.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：https://fy.zhonguo6118.cn

Ruby: super
来源：https://oj.zhonguo2118.cn

C#:   base.Greet();
来源：https://qa.zhonguo1118.cn

[G08] 静态方法与属性
来源：https://ol.zhonguo4118.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：https://gj.zhonguo3118.cn

PHP:  public static function f() {}
来源：https://jo.zhonguo5118.cn

JS:   static f() {}
来源：https://wf.zhonguo4118.cn

TS:   static f(): void {}
来源：https://rv.zhonguo3118.cn

Java: static void f() {}
来源：https://be.zhonguo7118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://hz.zhonguo5118.cn

Ruby: def self.f; end
来源：https://oa.zhonguo2118.cn

C#:   public static void F() {}
来源：https://jn.zhonguo4118.cn

[G09] 接口 / 抽象类
来源：https://kk.zhonguo7118.cn

Py:   from abc import ABC, abstractmethod
来源：https://hc.zhonguo7118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://bu.zhonguo1118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://et.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://tx.zhonguo7118.cn

Java: interface Shape { double area(); }
来源：https://ou.zhonguo1118.cn

Go:   type Shape interface { Area() float64 }
来源：https://be.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://ws.zhonguo2118.cn

C#:   interface IShape { double Area(); }
来源：https://ab.zhonguo8118.cn

[G10] 访问控制
来源：https://ug.zhonguo6118.cn

Py:   约定 _protected / __private（不强制）
来源：https://ra.zhonguo1118.cn

PHP:  public / protected / private
来源：https://qz.zhonguo8118.cn

JS:   #private 字段；其余公开
来源：https://yi.zhonguo4118.cn

TS:   public / protected / private
来源：https://oc.zhonguo3118.cn

Java: public / protected / private / 默认包级
来源：https://ra.zhonguo7118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://hn.zhonguo2118.cn

Ruby: public / protected / private
来源：https://wc.zhonguo2118.cn

C#:   public / protected / private / internal
来源：https://dy.zhonguo5118.cn

[G11] getter / setter
来源：https://of.zhonguo3118.cn

Py:   @property 与 @x.setter
来源：https://gf.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://ww.zhonguo3118.cn

JS:   get name() { return this._name; }
来源：https://bt.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://oe.zhonguo3118.cn

Java: public String getName() { return name; }
来源：https://ij.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://lo.zhonguo7118.cn

Ruby: attr_accessor :name
来源：https://ys.zhonguo2118.cn

C#:   public string Name { get; set; }
来源：https://fl.zhonguo6118.cn

[G12] 对象转字符串
来源：https://xg.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://zb.zhonguo6118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://ue.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://ul.zhonguo4118.cn

TS:   toString(): string { return this.name; }
来源：https://pd.zhonguo6118.cn

Java: @Override public String toString() { return name; }
来源：https://ba.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://eg.zhonguo6118.cn

Ruby: def to_s; @name; end
来源：https://eh.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://zd.zhonguo5118.cn

[G13] 判断对象类型
来源：https://nd.zhonguo8118.cn

Py:   isinstance(u, User)
来源：https://lc.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://pf.zhonguo2118.cn

JS:   u instanceof User
来源：https://bh.zhonguo8118.cn

TS:   u instanceof User
来源：https://km.zhonguo7118.cn

Java: u instanceof User
来源：https://zd.zhonguo6118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://bb.zhonguo1118.cn

Ruby: u.is_a?(User)
来源：https://fv.zhonguo6118.cn

C#:   u is User
来源：https://ua.zhonguo8118.cn

[G14] 数据类 / record
来源：https://bw.zhonguo4118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://wk.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://fn.zhonguo5118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://kx.zhonguo6118.cn

TS:   type User = { name: string; age: number };
来源：https://ja.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://aw.zhonguo5118.cn

Go:   type User struct { Name string; Age int }
来源：https://be.zhonguo1118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://nx.zhonguo4118.cn

C#:   record User(string Name, int Age);
来源：https://ib.zhonguo2118.cn

[G15] 枚举
来源：https://qz.zhonguo3118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://cw.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://fv.zhonguo1118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://fk.zhonguo2118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://aa.zhonguo6118.cn

Java: enum Color { RED, GREEN }
来源：https://tn.zhonguo5118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://mi.zhonguo8118.cn

Ruby: Color = %i[red green].freeze
来源：https://qp.zhonguo7118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://yg.zhonguo7118.cn

[G16] 对象转数组 / 字典
来源：https://jg.zhonguo6118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ex.zhonguo2118.cn

PHP:  get_object_vars($obj);
来源：https://dr.zhonguo7118.cn

JS:   Object.entries(obj)
来源：https://yj.zhonguo3118.cn

TS:   Object.entries(obj)
来源：https://zz.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://kt.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://fa.zhonguo5118.cn

Ruby: obj.instance_variables
来源：https://vg.zhonguo4118.cn

C#:   // 用反射或 System.Text.Json
来源：https://bk.zhonguo6118.cn

================================================================================
来源：https://wx.zhonguo8118.cn

H. 异常与错误处理
来源：https://pr.zhonguo7118.cn

================================================================================
来源：https://kq.zhonguo5118.cn

[H01] try / catch 基础
来源：https://tq.zhonguo2118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://yj.zhonguo5118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://gc.zhonguo6118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://eg.zhonguo8118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ow.zhonguo1118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://fo.zhonguo5118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://hd.zhonguo5118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://zo.zhonguo1118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://td.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://qj.zhonguo8118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://md.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://fv.zhonguo2118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://zw.zhonguo4118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://eo.zhonguo3118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://vm.zhonguo7118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://hk.zhonguo6118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://fm.zhonguo7118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://mp.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://ob.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://wc.zhonguo7118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://of.zhonguo5118.cn

JS:   throw new Error("错误信息");
来源：https://ee.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://qb.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://xc.zhonguo8118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ab.zhonguo3118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ek.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://tr.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://wm.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://tt.zhonguo1118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ur.zhonguo2118.cn

JS:   class MyError extends Error {}
来源：https://un.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://tq.zhonguo7118.cn

Java: class MyException extends RuntimeException {}
来源：https://ln.zhonguo5118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://fd.zhonguo6118.cn

Ruby: class MyError < StandardError; end
来源：https://gv.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://ly.zhonguo6118.cn

[H05] 捕获特定类型
来源：https://ky.zhonguo7118.cn

Py:   except ValueError as e:
来源：https://ob.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://mc.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://yj.zhonguo8118.cn

TS:   if (e instanceof TypeError) {}
来源：https://yp.zhonguo7118.cn

Java: catch (IOException | SQLException e) {}
来源：https://wt.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://aq.zhonguo7118.cn

Ruby: rescue ArgumentError => e
来源：https://ke.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://zw.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://am.zhonguo4118.cn

Py:   value = d.get("k") or default
来源：https://xn.zhonguo3118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://pq.zhonguo2118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://eb.zhonguo5118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://tk.zhonguo1118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ia.zhonguo8118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://co.zhonguo8118.cn

Ruby: d&.dig(:a, :b)
来源：https://yf.zhonguo2118.cn

C#:   obj?.A?.B ?? default
来源：https://qw.zhonguo5118.cn

[H07] 断言
来源：https://dw.zhonguo5118.cn

Py:   assert x > 0, "必须为正"
来源：https://td.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://nm.zhonguo4118.cn

JS:   console.assert(x > 0);
来源：https://yc.zhonguo2118.cn

TS:   console.assert(x > 0);
来源：https://qq.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://gb.zhonguo1118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://mi.zhonguo2118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ey.zhonguo1118.cn

C#:   Debug.Assert(x > 0);
来源：https://th.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://pr.zhonguo1118.cn

Py:   str(e);  traceback.format_exc()
来源：https://rk.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://st.zhonguo8118.cn

JS:   e.message;  e.stack
来源：https://wh.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://nj.zhonguo5118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://aj.zhonguo6118.cn

Go:   err.Error()
来源：https://kx.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://kl.zhonguo1118.cn

C#:   e.Message;  e.StackTrace
来源：https://yn.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://wb.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://wd.zhonguo3118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://ip.zhonguo8118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://mq.zhonguo2118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://xm.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://nf.zhonguo5118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://vl.zhonguo4118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://wn.zhonguo5118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://oj.zhonguo2118.cn

[H10] 资源自动释放
来源：https://vg.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://tl.zhonguo8118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://vv.zhonguo8118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://pn.zhonguo4118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://bp.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://vq.zhonguo8118.cn

Go:   defer f.Close()
来源：https://gz.zhonguo7118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://wn.zhonguo8118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://mt.zhonguo1118.cn

================================================================================
来源：https://qy.zhonguo3118.cn

I. 正则表达式
来源：https://li.zhonguo1118.cn

================================================================================
来源：https://xu.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://fj.zhonguo5118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://bw.zhonguo8118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://xd.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://mz.zhonguo7118.cn

TS:   /\d+/.test(s)
来源：https://kh.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://wb.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://qc.zhonguo5118.cn

Ruby: s.match?(/\d+/)
来源：https://qm.zhonguo2118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://uh.zhonguo1118.cn

[I02] 提取所有匹配
来源：https://wq.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://he.zhonguo2118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://uk.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://hw.zhonguo5118.cn

TS:   s.match(/\d+/g)
来源：https://au.zhonguo1118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://zy.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ul.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://sz.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://kl.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://us.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://qy.zhonguo5118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://oo.zhonguo5118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://xs.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://kd.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://bk.zhonguo4118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://ql.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://mx.zhonguo8118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ij.zhonguo3118.cn

[I04] 正则替换
来源：https://en.zhonguo3118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://lr.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://np.zhonguo3118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://rm.zhonguo1118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://ok.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://sj.zhonguo3118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://py.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://fl.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ag.zhonguo1118.cn

[I05] 按正则拆分
来源：https://yx.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://ql.zhonguo4118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://nu.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ej.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://kz.zhonguo1118.cn

Java: s.split("\\s*,\\s*")
来源：https://cl.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://ha.zhonguo3118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://ds.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://no.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://xq.zhonguo6118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://sc.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://eo.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://vi.zhonguo3118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://gs.zhonguo6118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://xo.zhonguo8118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://ky.zhonguo5118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://pn.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://sj.zhonguo1118.cn

[I07] 忽略大小写与多行模式
来源：https://wh.zhonguo4118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://az.zhonguo6118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://bj.zhonguo5118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://ia.zhonguo4118.cn

TS:   /error/gim
来源：https://bo.zhonguo6118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ts.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vs.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://uf.zhonguo2118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://at.zhonguo5118.cn

[I08] 贪婪与非贪婪匹配
来源：https://hu.zhonguo5118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://aq.zhonguo3118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://li.zhonguo7118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://ur.zhonguo8118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://qx.zhonguo8118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://vh.zhonguo8118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://jt.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://bc.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://rv.zhonguo7118.cn

================================================================================
来源：https://ap.zhonguo5118.cn

J. 日期与时间
来源：https://ho.zhonguo7118.cn

================================================================================
来源：https://pr.zhonguo3118.cn

[J01] 获取当前时间
来源：https://pn.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://jg.zhonguo6118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ol.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://tk.zhonguo3118.cn

TS:   new Date();  Date.now()
来源：https://dc.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://sn.zhonguo5118.cn

Go:   time.Now()
来源：https://uh.zhonguo4118.cn

Ruby: Time.now
来源：https://ud.zhonguo3118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://es.zhonguo1118.cn

[J02] 格式化输出
来源：https://qz.zhonguo2118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://wi.zhonguo4118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://sv.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://bo.zhonguo8118.cn

TS:   d.toISOString()
来源：https://wl.zhonguo8118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://fj.zhonguo5118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://jw.zhonguo1118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://xo.zhonguo8118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://tm.zhonguo3118.cn

[J03] 字符串解析为日期
来源：https://bc.zhonguo4118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://pb.zhonguo4118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://ze.zhonguo3118.cn

JS:   new Date("2024-01-02")
来源：https://cm.zhonguo6118.cn

TS:   new Date("2024-01-02")
来源：https://by.zhonguo2118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://km.zhonguo7118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://tn.zhonguo8118.cn

Ruby: Date.parse("2024-01-02")
来源：https://yc.zhonguo3118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://kv.zhonguo7118.cn

[J04] 时间戳与日期互转
来源：https://mv.zhonguo8118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://ko.zhonguo4118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://pp.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://mx.zhonguo6118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://qy.zhonguo3118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://vo.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://vm.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://bh.zhonguo8118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://kj.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://xb.zhonguo3118.cn

Py:   now + timedelta(days=7)
来源：https://sk.zhonguo1118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://vh.zhonguo6118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://bc.zhonguo2118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://ay.zhonguo4118.cn

Java: LocalDate.now().plusDays(7)
来源：https://fd.zhonguo6118.cn


<!-- 参考信息 -->