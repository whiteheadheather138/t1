代发 wailian999

TS:   public / protected / private
来源：https://eq.zhonguo1118.cn

Java: public / protected / private / 默认包级
来源：https://ig.zhonguo3118.cn

Go:   首字母大写可导出，小写仅包内可见
来源：https://is.zhonguo6118.cn

Ruby: public / protected / private
来源：https://wv.zhonguo4118.cn

C#:   public / protected / private / internal
来源：https://vm.zhonguo7118.cn

[G11] getter / setter
来源：https://lc.zhonguo1118.cn

Py:   @property 与 @x.setter
来源：https://zn.zhonguo6118.cn

PHP:  public function getName(): string { return $this->name; }
来源：https://em.zhonguo7118.cn

JS:   get name() { return this._name; }
来源：https://rv.zhonguo1118.cn

TS:   get name(): string { return this._name; }
来源：https://lq.zhonguo5118.cn

Java: public String getName() { return name; }
来源：https://vc.zhonguo6118.cn

Go:   func (u User) GetName() string { return u.Name }
来源：https://fl.zhonguo5118.cn

Ruby: attr_accessor :name
来源：https://ee.zhonguo1118.cn

C#:   public string Name { get; set; }
来源：https://dz.zhonguo6118.cn

[G12] 对象转字符串
来源：https://cv.zhonguo6118.cn

Py:   def __str__(self): return self.name
来源：https://yr.zhonguo5118.cn

PHP:  public function __toString(): string { return $this->name; }
来源：https://gx.zhonguo5118.cn

JS:   toString() { return this.name; }
来源：https://bq.zhonguo4118.cn

TS:   toString(): string { return this.name; }
来源：https://aj.zhonguo7118.cn

Java: @Override public String toString() { return name; }
来源：https://xc.zhonguo8118.cn

Go:   func (u User) String() string { return u.Name }
来源：https://wm.zhonguo8118.cn

Ruby: def to_s; @name; end
来源：https://lx.zhonguo3118.cn

C#:   public override string ToString() => Name;
来源：https://tc.zhonguo7118.cn

[G13] 判断对象类型
来源：https://xj.zhonguo2118.cn

Py:   isinstance(u, User)
来源：https://ye.zhonguo3118.cn

PHP:  $u instanceof User
来源：https://rv.zhonguo6118.cn

JS:   u instanceof User
来源：https://tv.zhonguo2118.cn

TS:   u instanceof User
来源：https://oq.zhonguo8118.cn

Java: u instanceof User
来源：https://dd.zhonguo4118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ge.zhonguo1118.cn

Ruby: u.is_a?(User)
来源：https://ym.zhonguo7118.cn

C#:   u is User
来源：https://xu.zhonguo8118.cn

[G14] 数据类 / record
来源：https://pn.zhonguo6118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://mg.zhonguo6118.cn

PHP:  // 用 readonly 属性模拟
来源：https://ii.zhonguo3118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ed.zhonguo1118.cn

TS:   type User = { name: string; age: number };
来源：https://nm.zhonguo5118.cn

Java: record User(String name, int age) {}
来源：https://jy.zhonguo4118.cn

Go:   type User struct { Name string; Age int }
来源：https://yz.zhonguo5118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://iw.zhonguo4118.cn

C#:   record User(string Name, int Age);
来源：https://je.zhonguo8118.cn

[G15] 枚举
来源：https://io.zhonguo6118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://sd.zhonguo4118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://pm.zhonguo6118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://dr.zhonguo2118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://gx.zhonguo7118.cn

Java: enum Color { RED, GREEN }
来源：https://af.zhonguo4118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://ak.zhonguo6118.cn

Ruby: Color = %i[red green].freeze
来源：https://ng.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://ga.zhonguo7118.cn

[G16] 对象转数组 / 字典
来源：https://jq.zhonguo7118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://yi.zhonguo7118.cn

PHP:  get_object_vars($obj);
来源：https://gp.zhonguo6118.cn

JS:   Object.entries(obj)
来源：https://uk.zhonguo5118.cn

TS:   Object.entries(obj)
来源：https://bl.zhonguo4118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://ex.zhonguo1118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://hb.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://fe.zhonguo4118.cn

C#:   // 用反射或 System.Text.Json
来源：https://fm.zhonguo8118.cn

================================================================================
来源：https://vx.zhonguo2118.cn

H. 异常与错误处理
来源：https://gr.zhonguo5118.cn

================================================================================
来源：https://qn.zhonguo5118.cn

[H01] try / catch 基础
来源：https://as.zhonguo8118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://up.zhonguo7118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://so.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://ru.zhonguo1118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://te.zhonguo2118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://rq.zhonguo2118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://cw.zhonguo7118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://po.zhonguo8118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://kv.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://dv.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://cy.zhonguo1118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://md.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://iu.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://le.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ii.zhonguo6118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://yg.zhonguo1118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://fg.zhonguo2118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ul.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://ce.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://qv.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://ij.zhonguo5118.cn

JS:   throw new Error("错误信息");
来源：https://ft.zhonguo1118.cn

TS:   throw new Error("错误信息");
来源：https://cd.zhonguo5118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://hw.zhonguo8118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://su.zhonguo7118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://wu.zhonguo3118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://fl.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://jt.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://oh.zhonguo8118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://en.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://ye.zhonguo8118.cn

TS:   class MyError extends Error {}
来源：https://xb.zhonguo6118.cn

Java: class MyException extends RuntimeException {}
来源：https://oz.zhonguo3118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://wn.zhonguo3118.cn

Ruby: class MyError < StandardError; end
来源：https://da.zhonguo5118.cn

C#:   class MyException : Exception {}
来源：https://nr.zhonguo1118.cn

[H05] 捕获特定类型
来源：https://us.zhonguo5118.cn

Py:   except ValueError as e:
来源：https://rg.zhonguo7118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://wv.zhonguo3118.cn

JS:   if (e instanceof TypeError) {}
来源：https://ef.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://ca.zhonguo1118.cn

Java: catch (IOException | SQLException e) {}
来源：https://be.zhonguo4118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://gz.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://ga.zhonguo3118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://bb.zhonguo7118.cn

[H06] 可选值 / 空值安全访问
来源：https://qb.zhonguo3118.cn

Py:   value = d.get("k") or default
来源：https://hq.zhonguo4118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://iv.zhonguo8118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://mp.zhonguo8118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://hp.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://kl.zhonguo7118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://kc.zhonguo5118.cn

Ruby: d&.dig(:a, :b)
来源：https://zl.zhonguo5118.cn

C#:   obj?.A?.B ?? default
来源：https://hu.zhonguo4118.cn

[H07] 断言
来源：https://pg.zhonguo6118.cn

Py:   assert x > 0, "必须为正"
来源：https://yu.zhonguo8118.cn

PHP:  assert($x > 0);
来源：https://pf.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://ld.zhonguo8118.cn

TS:   console.assert(x > 0);
来源：https://uq.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://tk.zhonguo6118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://cj.zhonguo4118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://fe.zhonguo8118.cn

C#:   Debug.Assert(x > 0);
来源：https://gz.zhonguo2118.cn

[H08] 获取错误信息与堆栈
来源：https://js.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://hb.zhonguo7118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://jm.zhonguo5118.cn

JS:   e.message;  e.stack
来源：https://if.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://uu.zhonguo4118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ef.zhonguo5118.cn

Go:   err.Error()
来源：https://jx.zhonguo2118.cn

Ruby: e.message;  e.backtrace
来源：https://bh.zhonguo3118.cn

C#:   e.Message;  e.StackTrace
来源：https://hw.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://oj.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://eg.zhonguo3118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://jj.zhonguo4118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://zy.zhonguo3118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://ra.zhonguo8118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://gn.zhonguo4118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://rs.zhonguo1118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://nv.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://bo.zhonguo5118.cn

[H10] 资源自动释放
来源：https://vi.zhonguo4118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://zy.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://aa.zhonguo1118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://oc.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://hl.zhonguo7118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://hm.zhonguo1118.cn

Go:   defer f.Close()
来源：https://al.zhonguo5118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://hu.zhonguo4118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://jo.zhonguo5118.cn

================================================================================
来源：https://we.zhonguo6118.cn

I. 正则表达式
来源：https://qx.zhonguo8118.cn

================================================================================
来源：https://hj.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://lc.zhonguo3118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://ad.zhonguo2118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://fb.zhonguo4118.cn

JS:   /\d+/.test(s)
来源：https://jd.zhonguo4118.cn

TS:   /\d+/.test(s)
来源：https://ya.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://mz.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://zn.zhonguo1118.cn

Ruby: s.match?(/\d+/)
来源：https://tv.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://zw.zhonguo2118.cn

[I02] 提取所有匹配
来源：https://jx.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://ta.zhonguo2118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://xe.zhonguo5118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://nd.zhonguo6118.cn

TS:   s.match(/\d+/g)
来源：https://kt.zhonguo5118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://il.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ro.zhonguo3118.cn

Ruby: s.scan(/\d+/)
来源：https://ca.zhonguo1118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://sk.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://nn.zhonguo2118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://jy.zhonguo4118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://we.zhonguo8118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://rs.zhonguo3118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://jp.zhonguo3118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://ju.zhonguo6118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://ym.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://rf.zhonguo1118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://un.zhonguo5118.cn

[I04] 正则替换
来源：https://jz.zhonguo2118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://ht.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://zg.zhonguo4118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://cj.zhonguo7118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://pa.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://db.zhonguo1118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://xl.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://cq.zhonguo1118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://pr.zhonguo3118.cn

[I05] 按正则拆分
来源：https://va.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://xy.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://wz.zhonguo4118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ns.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://ma.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://eo.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://pn.zhonguo1118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://lv.zhonguo5118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://sm.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://dn.zhonguo7118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://fa.zhonguo3118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://uh.zhonguo3118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://jm.zhonguo2118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://sy.zhonguo3118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://ek.zhonguo2118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://zv.zhonguo3118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://mt.zhonguo5118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://cp.zhonguo2118.cn

[I07] 忽略大小写与多行模式
来源：https://ib.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://iz.zhonguo3118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://fu.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://by.zhonguo8118.cn

TS:   /error/gim
来源：https://lx.zhonguo7118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://mn.zhonguo3118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vl.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://ti.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://gx.zhonguo5118.cn

[I08] 贪婪与非贪婪匹配
来源：https://bn.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://gq.zhonguo5118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://ja.zhonguo8118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://ir.zhonguo2118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://ke.zhonguo8118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ej.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://vp.zhonguo8118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://qe.zhonguo6118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://jw.zhonguo8118.cn

================================================================================
来源：https://pu.zhonguo7118.cn

J. 日期与时间
来源：https://sj.zhonguo3118.cn

================================================================================
来源：https://wm.zhonguo4118.cn

[J01] 获取当前时间
来源：https://qp.zhonguo7118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://lt.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://fb.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://jp.zhonguo8118.cn

TS:   new Date();  Date.now()
来源：https://fk.zhonguo8118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://fm.zhonguo5118.cn

Go:   time.Now()
来源：https://zm.zhonguo2118.cn

Ruby: Time.now
来源：https://jn.zhonguo2118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://oa.zhonguo2118.cn

[J02] 格式化输出
来源：https://eu.zhonguo2118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://rz.zhonguo1118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://zj.zhonguo5118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://jk.zhonguo5118.cn

TS:   d.toISOString()
来源：https://xn.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://co.zhonguo1118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://pe.zhonguo8118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://fs.zhonguo7118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://tk.zhonguo2118.cn

[J03] 字符串解析为日期
来源：https://uj.zhonguo5118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://od.zhonguo7118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://ig.zhonguo5118.cn

JS:   new Date("2024-01-02")
来源：https://wj.zhonguo4118.cn

TS:   new Date("2024-01-02")
来源：https://ws.zhonguo3118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://vo.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://vi.zhonguo3118.cn

Ruby: Date.parse("2024-01-02")
来源：https://yy.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://gt.zhonguo5118.cn

[J04] 时间戳与日期互转
来源：https://vo.zhonguo5118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://pj.zhonguo5118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://mk.zhonguo8118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://hz.zhonguo8118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://rl.zhonguo5118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://gi.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://hk.zhonguo4118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://qs.zhonguo4118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://fn.zhonguo7118.cn

[J05] 时间加减（加 7 天）
来源：https://ng.zhonguo8118.cn

Py:   now + timedelta(days=7)
来源：https://jk.zhonguo1118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://hy.zhonguo1118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://gj.zhonguo4118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://xt.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://zl.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://hy.zhonguo4118.cn

Ruby: Time.now + 7 * 86400
来源：https://vy.zhonguo4118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://kl.zhonguo6118.cn

[J06] 计算两时间之差
来源：https://qu.zhonguo6118.cn

Py:   (end - start).total_seconds()
来源：https://hj.zhonguo3118.cn

PHP:  $end->diff($start)->days;
来源：https://bl.zhonguo2118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://uq.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://lc.zhonguo8118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://xv.zhonguo4118.cn

Go:   end.Sub(start).Hours()
来源：https://gk.zhonguo5118.cn

Ruby: end - start                 # 返回秒数
来源：https://sr.zhonguo8118.cn

C#:   (end - start).TotalSeconds
来源：https://kk.zhonguo3118.cn

[J07] 比较两个日期
来源：https://bh.zhonguo4118.cn

Py:   d1 < d2;  d1 == d2
来源：https://iw.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://yx.zhonguo6118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://cr.zhonguo4118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://bv.zhonguo8118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://jw.zhonguo6118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://dw.zhonguo3118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://jq.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://wt.zhonguo3118.cn

[J08] 提取年月日与星期
来源：https://he.zhonguo1118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://pg.zhonguo1118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ot.zhonguo6118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://sh.zhonguo5118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://af.zhonguo7118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://du.zhonguo1118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://ee.zhonguo6118.cn


<!-- 参考信息 -->