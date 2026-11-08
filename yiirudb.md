代发 wailian999

JS:   get name() { return this._name; }
来源：https://ke.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://bp.zhonguo2118.cn

Java: public String getName() { return name; }
来源：https://wb.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://ai.zhonguo2118.cn

Ruby: attr_accessor :name
来源：https://lf.zhonguo1118.cn

C#:   public string Name { get; set; }
来源：https://wn.zhonguo1118.cn

[G12] 对象转字符串
来源：https://mm.zhonguo4118.cn

Py:   def __str__(self): return self.name
来源：https://kb.zhonguo1118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://de.zhonguo3118.cn

JS:   toString() { return this.name; }
来源：https://dh.zhonguo6118.cn

TS:   toString(): string { return this.name; }
来源：https://gd.zhonguo5118.cn

Java: @Override public String toString() { return name; }
来源：https://qj.zhonguo1118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://nj.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://lp.zhonguo6118.cn

C#:   public override string ToString() => Name;
来源：https://pl.zhonguo8118.cn

[G13] 判断对象类型
来源：https://lq.zhonguo3118.cn

Py:   isinstance(u, User)
来源：https://lm.zhonguo7118.cn

PHP:  $u instanceof User
来源：https://sw.zhonguo5118.cn

JS:   u instanceof User
来源：https://md.zhonguo1118.cn

TS:   u instanceof User
来源：https://kn.zhonguo8118.cn

Java: u instanceof User
来源：https://xb.zhonguo4118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ac.zhonguo5118.cn

Ruby: u.is_a?(User)
来源：https://tx.zhonguo1118.cn

C#:   u is User
来源：https://vv.zhonguo3118.cn

[G14] 数据类 / record
来源：https://pv.zhonguo3118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://pc.zhonguo1118.cn

PHP:  // 用 readonly 属性模拟
来源：https://fv.zhonguo6118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ry.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://ai.zhonguo4118.cn

Java: record User(String name, int age) {}
来源：https://vj.zhonguo6118.cn

Go:   type User struct { Name string; Age int }
来源：https://br.zhonguo4118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://qm.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://kc.zhonguo3118.cn

[G15] 枚举
来源：https://ii.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://ag.zhonguo6118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://gd.zhonguo5118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://hb.zhonguo6118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://es.zhonguo1118.cn

Java: enum Color { RED, GREEN }
来源：https://lj.zhonguo1118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://lp.zhonguo2118.cn

Ruby: Color = %i[red green].freeze
来源：https://ie.zhonguo6118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ki.zhonguo7118.cn

[G16] 对象转数组 / 字典
来源：https://iy.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://en.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://wn.zhonguo2118.cn

JS:   Object.entries(obj)
来源：https://un.zhonguo6118.cn

TS:   Object.entries(obj)
来源：https://dx.zhonguo1118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://gj.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://vr.zhonguo4118.cn

Ruby: obj.instance_variables
来源：https://lx.zhonguo3118.cn

C#:   // 用反射或 System.Text.Json
来源：https://es.zhonguo5118.cn

================================================================================
来源：https://gb.zhonguo8118.cn

H. 异常与错误处理
来源：https://so.zhonguo6118.cn

================================================================================
来源：https://ok.zhonguo1118.cn

[H01] try / catch 基础
来源：https://ct.zhonguo7118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://hn.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://rs.zhonguo2118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://uc.zhonguo8118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://qu.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ph.zhonguo7118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://bf.zhonguo6118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://pf.zhonguo6118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://cc.zhonguo2118.cn

[H02] finally / ensure 收尾
来源：https://oq.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://bu.zhonguo4118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://qu.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://lh.zhonguo6118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://lm.zhonguo8118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://fj.zhonguo8118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://kc.zhonguo3118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://ee.zhonguo6118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://vc.zhonguo5118.cn

[H03] 主动抛出异常
来源：https://hy.zhonguo3118.cn

Py:   raise ValueError("错误信息")
来源：https://tc.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ro.zhonguo8118.cn

JS:   throw new Error("错误信息");
来源：https://jk.zhonguo6118.cn

TS:   throw new Error("错误信息");
来源：https://dy.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://vp.zhonguo1118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://le.zhonguo1118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://gm.zhonguo8118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://yg.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://fi.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://lb.zhonguo5118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://ep.zhonguo2118.cn

JS:   class MyError extends Error {}
来源：https://lb.zhonguo5118.cn

TS:   class MyError extends Error {}
来源：https://ae.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://fr.zhonguo7118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://wz.zhonguo5118.cn

Ruby: class MyError < StandardError; end
来源：https://ic.zhonguo2118.cn

C#:   class MyException : Exception {}
来源：https://cj.zhonguo4118.cn

[H05] 捕获特定类型
来源：https://yk.zhonguo4118.cn

Py:   except ValueError as e:
来源：https://st.zhonguo1118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://mg.zhonguo1118.cn

JS:   if (e instanceof TypeError) {}
来源：https://wf.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://qp.zhonguo5118.cn

Java: catch (IOException | SQLException e) {}
来源：https://qm.zhonguo1118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://yr.zhonguo5118.cn

Ruby: rescue ArgumentError => e
来源：https://mt.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://tx.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://nv.zhonguo7118.cn

Py:   value = d.get("k") or default
来源：https://zj.zhonguo5118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://ws.zhonguo5118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://lj.zhonguo5118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://tf.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://bb.zhonguo6118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://wz.zhonguo1118.cn

Ruby: d&.dig(:a, :b)
来源：https://fo.zhonguo7118.cn

C#:   obj?.A?.B ?? default
来源：https://zm.zhonguo3118.cn

[H07] 断言
来源：https://bq.zhonguo6118.cn

Py:   assert x > 0, "必须为正"
来源：https://hf.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://ls.zhonguo7118.cn

JS:   console.assert(x > 0);
来源：https://wy.zhonguo3118.cn

TS:   console.assert(x > 0);
来源：https://mv.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://dd.zhonguo2118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://jf.zhonguo2118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ig.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://fl.zhonguo3118.cn

[H08] 获取错误信息与堆栈
来源：https://ep.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://ti.zhonguo8118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://bz.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://qp.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ye.zhonguo3118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://js.zhonguo6118.cn

Go:   err.Error()
来源：https://pl.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://gk.zhonguo5118.cn

C#:   e.Message;  e.StackTrace
来源：https://ub.zhonguo2118.cn

[H09] 带错误码的异常
来源：https://co.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://mm.zhonguo2118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://is.zhonguo5118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://vc.zhonguo3118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://lc.zhonguo5118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ss.zhonguo2118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://io.zhonguo1118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://vc.zhonguo6118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ji.zhonguo5118.cn

[H10] 资源自动释放
来源：https://aq.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://nj.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://nm.zhonguo4118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://vl.zhonguo5118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://am.zhonguo6118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://xp.zhonguo8118.cn

Go:   defer f.Close()
来源：https://mz.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://to.zhonguo3118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://zt.zhonguo6118.cn

================================================================================
来源：https://dn.zhonguo4118.cn

I. 正则表达式
来源：https://hi.zhonguo6118.cn

================================================================================
来源：https://tg.zhonguo5118.cn

[I01] 判断是否匹配
来源：https://xy.zhonguo3118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://kp.zhonguo7118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://eg.zhonguo8118.cn

JS:   /\d+/.test(s)
来源：https://yk.zhonguo5118.cn

TS:   /\d+/.test(s)
来源：https://vc.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://bu.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://em.zhonguo3118.cn

Ruby: s.match?(/\d+/)
来源：https://tj.zhonguo8118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://ok.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://hd.zhonguo4118.cn

Py:   re.findall(r"\d+", s)
来源：https://dg.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://mp.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://re.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://nu.zhonguo8118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://bc.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://un.zhonguo3118.cn

Ruby: s.scan(/\d+/)
来源：https://pn.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://ll.zhonguo2118.cn

[I03] 提取捕获分组
来源：https://do.zhonguo5118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://vg.zhonguo6118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ic.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://dk.zhonguo4118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://pm.zhonguo4118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://mr.zhonguo2118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://fe.zhonguo5118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://rm.zhonguo2118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ue.zhonguo3118.cn

[I04] 正则替换
来源：https://et.zhonguo6118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://oo.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://aa.zhonguo1118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://sx.zhonguo5118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://xw.zhonguo1118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://oa.zhonguo4118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://ue.zhonguo8118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ak.zhonguo7118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://qz.zhonguo2118.cn

[I05] 按正则拆分
来源：https://wk.zhonguo3118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://af.zhonguo4118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ap.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://la.zhonguo7118.cn

TS:   s.split(/\s*,\s*/)
来源：https://fa.zhonguo7118.cn

Java: s.split("\\s*,\\s*")
来源：https://id.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://zi.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://sl.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://sq.zhonguo3118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://hq.zhonguo4118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://to.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://dz.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://ji.zhonguo2118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://lj.zhonguo6118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://re.zhonguo3118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://ah.zhonguo1118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://oz.zhonguo4118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://vr.zhonguo7118.cn

[I07] 忽略大小写与多行模式
来源：https://ql.zhonguo6118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://ap.zhonguo2118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://to.zhonguo1118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://kx.zhonguo5118.cn

TS:   /error/gim
来源：https://wh.zhonguo2118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://gp.zhonguo6118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://bl.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://za.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://qe.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ix.zhonguo1118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ht.zhonguo5118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://az.zhonguo4118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://bf.zhonguo3118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://uj.zhonguo5118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://oa.zhonguo8118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://id.zhonguo6118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://fd.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ab.zhonguo2118.cn

================================================================================
来源：https://ym.zhonguo8118.cn

J. 日期与时间
来源：https://pf.zhonguo2118.cn

================================================================================
来源：https://ow.zhonguo1118.cn

[J01] 获取当前时间
来源：https://am.zhonguo5118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://aa.zhonguo7118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://xo.zhonguo4118.cn

JS:   new Date();  Date.now()
来源：https://hp.zhonguo3118.cn

TS:   new Date();  Date.now()
来源：https://jk.zhonguo1118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://yl.zhonguo1118.cn

Go:   time.Now()
来源：https://qx.zhonguo4118.cn

Ruby: Time.now
来源：https://ks.zhonguo6118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://br.zhonguo3118.cn

[J02] 格式化输出
来源：https://tg.zhonguo8118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://bj.zhonguo1118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://cx.zhonguo6118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://lm.zhonguo1118.cn

TS:   d.toISOString()
来源：https://ty.zhonguo3118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://lw.zhonguo8118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://tf.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://gb.zhonguo8118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ct.zhonguo6118.cn

[J03] 字符串解析为日期
来源：https://ad.zhonguo8118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://gz.zhonguo3118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://kt.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://bm.zhonguo5118.cn

TS:   new Date("2024-01-02")
来源：https://py.zhonguo7118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://vt.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://ep.zhonguo4118.cn

Ruby: Date.parse("2024-01-02")
来源：https://jk.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://rq.zhonguo4118.cn

[J04] 时间戳与日期互转
来源：https://eh.zhonguo2118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://cc.zhonguo8118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://vu.zhonguo2118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://ri.zhonguo2118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://kw.zhonguo6118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://pw.zhonguo2118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://tb.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://an.zhonguo3118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://jn.zhonguo3118.cn

[J05] 时间加减（加 7 天）
来源：https://ml.zhonguo6118.cn

Py:   now + timedelta(days=7)
来源：https://ga.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://zl.zhonguo5118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://yy.zhonguo3118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://rc.zhonguo6118.cn

Java: LocalDate.now().plusDays(7)
来源：https://yg.zhonguo4118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://rz.zhonguo6118.cn

Ruby: Time.now + 7 * 86400
来源：https://pz.zhonguo4118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://jv.zhonguo3118.cn

[J06] 计算两时间之差
来源：https://wg.zhonguo1118.cn

Py:   (end - start).total_seconds()
来源：https://ri.zhonguo2118.cn

PHP:  $end->diff($start)->days;
来源：https://eb.zhonguo3118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://ma.zhonguo5118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://xe.zhonguo5118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://fv.zhonguo3118.cn

Go:   end.Sub(start).Hours()
来源：https://ac.zhonguo6118.cn

Ruby: end - start                 # 返回秒数
来源：https://bq.zhonguo1118.cn

C#:   (end - start).TotalSeconds
来源：https://zi.zhonguo7118.cn

[J07] 比较两个日期
来源：https://gm.zhonguo3118.cn

Py:   d1 < d2;  d1 == d2
来源：https://mx.zhonguo8118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://vm.zhonguo5118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://nk.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://mm.zhonguo2118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://hi.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://yx.zhonguo1118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://ei.zhonguo7118.cn

C#:   d1 < d2;  d1 == d2
来源：https://jh.zhonguo3118.cn

[J08] 提取年月日与星期
来源：https://av.zhonguo4118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://fx.zhonguo1118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ny.zhonguo3118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://fe.zhonguo4118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://vh.zhonguo5118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://sb.zhonguo1118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://gr.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://hl.zhonguo3118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ex.zhonguo7118.cn

[J09] 时区处理
来源：https://oa.zhonguo3118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://sf.zhonguo8118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://wz.zhonguo7118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://yg.zhonguo6118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://jj.zhonguo1118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://zm.zhonguo8118.cn


<!-- 参考信息 -->