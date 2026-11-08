代发 wailian999

PHP:  public static function f() {}
来源：https://az.zhonguo4118.cn

JS:   static f() {}
来源：https://ad.zhonguo2118.cn

TS:   static f(): void {}
来源：https://pf.zhonguo1118.cn

Java: static void f() {}
来源：https://oe.zhonguo3118.cn

Go:   // 无 static：用包级函数，按包名调用
来源：https://of.zhonguo3118.cn

Ruby: def self.f; end
来源：https://qf.zhonguo6118.cn

C#:   public static void F() {}
来源：https://am.zhonguo7118.cn

[G09] 接口 / 抽象类
来源：https://am.zhonguo1118.cn

Py:   from abc import ABC, abstractmethod
来源：https://jd.zhonguo2118.cn

PHP:  interface Shape { public function area(): float; }
来源：https://jq.zhonguo3118.cn

JS:   // 无接口：靠约定或 JSDoc
来源：https://rk.zhonguo3118.cn

TS:   interface Shape { area(): number; }
来源：https://vh.zhonguo8118.cn

Java: interface Shape { double area(); }
来源：https://px.zhonguo8118.cn

Go:   type Shape interface { Area() float64 }
来源：https://uf.zhonguo5118.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：https://lp.zhonguo1118.cn

C#:   interface IShape { double Area(); }
来源：https://yt.zhonguo5118.cn

[G10] 访问控制
来源：https://vt.zhonguo7118.cn

Py:   约定 _protected / __private（不强制）
来源：https://lh.zhonguo4118.cn

PHP:  public / protected / private
来源：https://ke.zhonguo5118.cn

JS:   #private 字段；其余公开
来源：https://lu.zhonguo7118.cn

TS:   public / protected / private
来源：https://yo.zhonguo8118.cn

Java: public / protected / private / 默认包级
来源：https://cv.zhonguo7118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://zw.zhonguo2118.cn

Ruby: public / protected / private
来源：https://mk.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://ns.zhonguo8118.cn

[G11] getter / setter
来源：https://dc.zhonguo5118.cn

Py:   @property 与 @x.setter
来源：https://pv.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://eb.zhonguo7118.cn

JS:   get name() { return this._name; }
来源：https://al.zhonguo2118.cn

TS:   get name(): string { return this._name; }
来源：https://iv.zhonguo1118.cn

Java: public String getName() { return name; }
来源：https://va.zhonguo7118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://tu.zhonguo8118.cn

Ruby: attr_accessor :name
来源：https://dy.zhonguo1118.cn

C#:   public string Name { get; set; }
来源：https://qs.zhonguo6118.cn

[G12] 对象转字符串
来源：https://di.zhonguo2118.cn

Py:   def __str__(self): return self.name
来源：https://js.zhonguo8118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://sn.zhonguo4118.cn

JS:   toString() { return this.name; }
来源：https://uh.zhonguo4118.cn

TS:   toString(): string { return this.name; }
来源：https://ps.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://gc.zhonguo2118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://ub.zhonguo2118.cn

Ruby: def to_s; @name; end
来源：https://aq.zhonguo8118.cn

C#:   public override string ToString() => Name;
来源：https://di.zhonguo2118.cn

[G13] 判断对象类型
来源：https://uz.zhonguo1118.cn

Py:   isinstance(u, User)
来源：https://gt.zhonguo4118.cn

PHP:  $u instanceof User
来源：https://pu.zhonguo2118.cn

JS:   u instanceof User
来源：https://gx.zhonguo1118.cn

TS:   u instanceof User
来源：https://zy.zhonguo6118.cn

Java: u instanceof User
来源：https://ns.zhonguo6118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ex.zhonguo2118.cn

Ruby: u.is_a?(User)
来源：https://zc.zhonguo6118.cn

C#:   u is User
来源：https://zo.zhonguo8118.cn

[G14] 数据类 / record
来源：https://sp.zhonguo6118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://hq.zhonguo7118.cn

PHP:  // 用 readonly 属性模拟
来源：https://md.zhonguo2118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://bz.zhonguo8118.cn

TS:   type User = { name: string; age: number };
来源：https://sp.zhonguo1118.cn

Java: record User(String name, int age) {}
来源：https://nm.zhonguo5118.cn

Go:   type User struct { Name string; Age int }
来源：https://qf.zhonguo5118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://yp.zhonguo5118.cn

C#:   record User(string Name, int Age);
来源：https://jy.zhonguo7118.cn

[G15] 枚举
来源：https://qq.zhonguo1118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://pz.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://uq.zhonguo8118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://dj.zhonguo1118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://ez.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://fx.zhonguo8118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://bi.zhonguo3118.cn

Ruby: Color = %i[red green].freeze
来源：https://qm.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ti.zhonguo1118.cn

[G16] 对象转数组 / 字典
来源：https://vc.zhonguo2118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ih.zhonguo8118.cn

PHP:  get_object_vars($obj);
来源：https://xw.zhonguo5118.cn

JS:   Object.entries(obj)
来源：https://lw.zhonguo7118.cn

TS:   Object.entries(obj)
来源：https://dj.zhonguo4118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://rg.zhonguo4118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://tt.zhonguo6118.cn

Ruby: obj.instance_variables
来源：https://of.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://zm.zhonguo1118.cn

================================================================================
来源：https://tt.zhonguo7118.cn

H. 异常与错误处理
来源：https://po.zhonguo3118.cn

================================================================================
来源：https://ar.zhonguo6118.cn

[H01] try / catch 基础
来源：https://zs.zhonguo3118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://zg.zhonguo3118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://oy.zhonguo4118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://vl.zhonguo2118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://tg.zhonguo3118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://zz.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://eu.zhonguo3118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://zk.zhonguo4118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://sg.zhonguo2118.cn

[H02] finally / ensure 收尾
来源：https://es.zhonguo5118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://qz.zhonguo5118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://ci.zhonguo1118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://we.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://gp.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://xe.zhonguo7118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://gr.zhonguo2118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://se.zhonguo1118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://wo.zhonguo1118.cn

[H03] 主动抛出异常
来源：https://cp.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://qm.zhonguo6118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ps.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://ln.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://my.zhonguo6118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://oq.zhonguo8118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://hp.zhonguo4118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ll.zhonguo2118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://mu.zhonguo1118.cn

[H04] 自定义异常类型
来源：https://ly.zhonguo8118.cn

Py:   class MyError(Exception): pass
来源：https://pd.zhonguo6118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ja.zhonguo1118.cn

JS:   class MyError extends Error {}
来源：https://wj.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://gz.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://sy.zhonguo1118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://xu.zhonguo4118.cn

Ruby: class MyError < StandardError; end
来源：https://mb.zhonguo3118.cn

C#:   class MyException : Exception {}
来源：https://lc.zhonguo5118.cn

[H05] 捕获特定类型
来源：https://dt.zhonguo6118.cn

Py:   except ValueError as e:
来源：https://kd.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://ft.zhonguo5118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ol.zhonguo1118.cn

TS:   if (e instanceof TypeError) {}
来源：https://sj.zhonguo6118.cn

Java: catch (IOException | SQLException e) {}
来源：https://tm.zhonguo8118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://hy.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://hh.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://dr.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://fn.zhonguo6118.cn

Py:   value = d.get("k") or default
来源：https://tu.zhonguo6118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://gp.zhonguo7118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://fs.zhonguo4118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://ds.zhonguo7118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://xd.zhonguo7118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://tb.zhonguo8118.cn

Ruby: d&.dig(:a, :b)
来源：https://my.zhonguo8118.cn

C#:   obj?.A?.B ?? default
来源：https://rv.zhonguo2118.cn

[H07] 断言
来源：https://rg.zhonguo2118.cn

Py:   assert x > 0, "必须为正"
来源：https://gv.zhonguo4118.cn

PHP:  assert($x > 0);
来源：https://yn.zhonguo3118.cn

JS:   console.assert(x > 0);
来源：https://rd.zhonguo8118.cn

TS:   console.assert(x > 0);
来源：https://gf.zhonguo6118.cn

Java: assert x > 0 : "必须为正";
来源：https://ke.zhonguo2118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://vf.zhonguo5118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://tn.zhonguo2118.cn

C#:   Debug.Assert(x > 0);
来源：https://yl.zhonguo6118.cn

[H08] 获取错误信息与堆栈
来源：https://iq.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://xd.zhonguo6118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://yk.zhonguo8118.cn

JS:   e.message;  e.stack
来源：https://ru.zhonguo4118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://gp.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ap.zhonguo4118.cn

Go:   err.Error()
来源：https://hi.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://zn.zhonguo5118.cn

C#:   e.Message;  e.StackTrace
来源：https://ey.zhonguo8118.cn

[H09] 带错误码的异常
来源：https://rs.zhonguo3118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://fc.zhonguo4118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://bc.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://lp.zhonguo3118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://xw.zhonguo2118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ap.zhonguo4118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://hv.zhonguo2118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://au.zhonguo3118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://go.zhonguo3118.cn

[H10] 资源自动释放
来源：https://gg.zhonguo1118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://co.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://or.zhonguo5118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://tj.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://yb.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://re.zhonguo4118.cn

Go:   defer f.Close()
来源：https://ma.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://mx.zhonguo6118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://ax.zhonguo7118.cn

================================================================================
来源：https://qf.zhonguo2118.cn

I. 正则表达式
来源：https://pf.zhonguo4118.cn

================================================================================
来源：https://ew.zhonguo7118.cn

[I01] 判断是否匹配
来源：https://km.zhonguo3118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://xu.zhonguo3118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://qt.zhonguo7118.cn

JS:   /\d+/.test(s)
来源：https://vg.zhonguo2118.cn

TS:   /\d+/.test(s)
来源：https://xr.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://fb.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://gq.zhonguo7118.cn

Ruby: s.match?(/\d+/)
来源：https://pk.zhonguo5118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://nr.zhonguo4118.cn

[I02] 提取所有匹配
来源：https://ds.zhonguo3118.cn

Py:   re.findall(r"\d+", s)
来源：https://oi.zhonguo3118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://bz.zhonguo1118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://bg.zhonguo2118.cn

TS:   s.match(/\d+/g)
来源：https://ar.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://wd.zhonguo4118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://oq.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://ni.zhonguo8118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ec.zhonguo7118.cn

[I03] 提取捕获分组
来源：https://id.zhonguo3118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://hn.zhonguo6118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://hs.zhonguo3118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://mf.zhonguo5118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://mh.zhonguo7118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://sc.zhonguo6118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://jj.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://fx.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ax.zhonguo2118.cn

[I04] 正则替换
来源：https://tc.zhonguo1118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://tk.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://fw.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://sr.zhonguo7118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://la.zhonguo4118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://ju.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://uc.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://rx.zhonguo5118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://pd.zhonguo5118.cn

[I05] 按正则拆分
来源：https://ol.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://yk.zhonguo4118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://km.zhonguo1118.cn

JS:   s.split(/\s*,\s*/)
来源：https://gv.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://nn.zhonguo5118.cn

Java: s.split("\\s*,\\s*")
来源：https://re.zhonguo2118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://wi.zhonguo1118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://fq.zhonguo3118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://mr.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://wb.zhonguo6118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://by.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://yj.zhonguo8118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://cc.zhonguo4118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xp.zhonguo6118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://xq.zhonguo6118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://rc.zhonguo2118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://sa.zhonguo1118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://jx.zhonguo3118.cn

[I07] 忽略大小写与多行模式
来源：https://ca.zhonguo8118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://at.zhonguo2118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://pb.zhonguo6118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://nt.zhonguo4118.cn

TS:   /error/gim
来源：https://yh.zhonguo2118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://yl.zhonguo5118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vs.zhonguo2118.cn

Ruby: s.scan(/error/i)
来源：https://xa.zhonguo6118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://yc.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://da.zhonguo6118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://mv.zhonguo6118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://cg.zhonguo3118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://wg.zhonguo7118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://sm.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://id.zhonguo6118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://vh.zhonguo5118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://bi.zhonguo3118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://go.zhonguo3118.cn

================================================================================
来源：https://tz.zhonguo3118.cn

J. 日期与时间
来源：https://mt.zhonguo8118.cn

================================================================================
来源：https://qg.zhonguo6118.cn

[J01] 获取当前时间
来源：https://eq.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://zf.zhonguo7118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://wf.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://or.zhonguo4118.cn

TS:   new Date();  Date.now()
来源：https://sa.zhonguo6118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://jy.zhonguo3118.cn

Go:   time.Now()
来源：https://qp.zhonguo7118.cn

Ruby: Time.now
来源：https://gn.zhonguo2118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://ob.zhonguo4118.cn

[J02] 格式化输出
来源：https://mt.zhonguo8118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://vs.zhonguo1118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ie.zhonguo4118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://st.zhonguo6118.cn

TS:   d.toISOString()
来源：https://xe.zhonguo6118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ny.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://zf.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://jj.zhonguo7118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://di.zhonguo7118.cn

[J03] 字符串解析为日期
来源：https://vy.zhonguo3118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://bz.zhonguo6118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://te.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://jt.zhonguo5118.cn

TS:   new Date("2024-01-02")
来源：https://pz.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://it.zhonguo5118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://nb.zhonguo7118.cn

Ruby: Date.parse("2024-01-02")
来源：https://cf.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://vr.zhonguo7118.cn

[J04] 时间戳与日期互转
来源：https://fg.zhonguo6118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://rp.zhonguo2118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://av.zhonguo8118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://cw.zhonguo8118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://fj.zhonguo2118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://dq.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://nb.zhonguo6118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://mq.zhonguo2118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://mx.zhonguo4118.cn

[J05] 时间加减（加 7 天）
来源：https://rw.zhonguo8118.cn

Py:   now + timedelta(days=7)
来源：https://fl.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://ft.zhonguo4118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://lg.zhonguo2118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://sl.zhonguo1118.cn

Java: LocalDate.now().plusDays(7)
来源：https://si.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://bl.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://bq.zhonguo6118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://mx.zhonguo1118.cn

[J06] 计算两时间之差
来源：https://ll.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://du.zhonguo4118.cn

PHP:  $end->diff($start)->days;
来源：https://nv.zhonguo5118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://vt.zhonguo2118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ms.zhonguo4118.cn


<!-- 参考信息 -->