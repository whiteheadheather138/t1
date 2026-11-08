代发 wailian999

Py:   isinstance(u, User)
来源：https://tm.zhonguo6118.cn

PHP:  $u instanceof User
来源：https://sf.zhonguo7118.cn

JS:   u instanceof User
来源：https://dk.zhonguo8118.cn

TS:   u instanceof User
来源：https://dr.zhonguo4118.cn

Java: u instanceof User
来源：https://rt.zhonguo2118.cn

Go:   u, ok := v.(User)            // 类型断言
来源：https://ee.zhonguo8118.cn

Ruby: u.is_a?(User)
来源：https://mw.zhonguo3118.cn

C#:   u is User
来源：https://ay.zhonguo8118.cn

[G14] 数据类 / record
来源：https://zu.zhonguo5118.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：https://io.zhonguo3118.cn

PHP:  // 用 readonly 属性模拟
来源：https://aj.zhonguo5118.cn

JS:   // 无内置：普通类或对象字面量
来源：https://ic.zhonguo7118.cn

TS:   type User = { name: string; age: number };
来源：https://ck.zhonguo2118.cn

Java: record User(String name, int age) {}
来源：https://eg.zhonguo8118.cn

Go:   type User struct { Name string; Age int }
来源：https://wu.zhonguo7118.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：https://le.zhonguo2118.cn

C#:   record User(string Name, int Age);
来源：https://ay.zhonguo4118.cn

[G15] 枚举
来源：https://hh.zhonguo7118.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：https://jq.zhonguo7118.cn

PHP:  enum Color: string { case Red = "red"; }
来源：https://qe.zhonguo7118.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：https://cq.zhonguo7118.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：https://st.zhonguo8118.cn

Java: enum Color { RED, GREEN }
来源：https://da.zhonguo8118.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：https://nt.zhonguo3118.cn

Ruby: Color = %i[red green].freeze
来源：https://wp.zhonguo2118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://om.zhonguo5118.cn

[G16] 对象转数组 / 字典
来源：https://uc.zhonguo1118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://dw.zhonguo3118.cn

PHP:  get_object_vars($obj);
来源：https://jd.zhonguo1118.cn

JS:   Object.entries(obj)
来源：https://ui.zhonguo5118.cn

TS:   Object.entries(obj)
来源：https://lk.zhonguo3118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://rd.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://lh.zhonguo3118.cn

Ruby: obj.instance_variables
来源：https://vn.zhonguo8118.cn

C#:   // 用反射或 System.Text.Json
来源：https://by.zhonguo3118.cn

================================================================================
来源：https://hg.zhonguo5118.cn

H. 异常与错误处理
来源：https://uk.zhonguo5118.cn

================================================================================
来源：https://pc.zhonguo2118.cn

[H01] try / catch 基础
来源：https://uf.zhonguo4118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://wu.zhonguo8118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://jt.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://kl.zhonguo4118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://sz.zhonguo2118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://oh.zhonguo8118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://xy.zhonguo5118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://yq.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://fd.zhonguo2118.cn

[H02] finally / ensure 收尾
来源：https://so.zhonguo4118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://wd.zhonguo8118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://pv.zhonguo6118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://al.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://zu.zhonguo7118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://fw.zhonguo1118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://te.zhonguo6118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://vi.zhonguo3118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://qo.zhonguo7118.cn

[H03] 主动抛出异常
来源：https://rv.zhonguo7118.cn

Py:   raise ValueError("错误信息")
来源：https://jc.zhonguo1118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://og.zhonguo1118.cn

JS:   throw new Error("错误信息");
来源：https://sf.zhonguo7118.cn

TS:   throw new Error("错误信息");
来源：https://uz.zhonguo8118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://ub.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://nu.zhonguo1118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://zs.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://yt.zhonguo8118.cn

[H04] 自定义异常类型
来源：https://xb.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://jg.zhonguo7118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://uj.zhonguo5118.cn

JS:   class MyError extends Error {}
来源：https://wm.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://pt.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://vm.zhonguo6118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://zr.zhonguo8118.cn

Ruby: class MyError < StandardError; end
来源：https://lu.zhonguo8118.cn

C#:   class MyException : Exception {}
来源：https://pz.zhonguo5118.cn

[H05] 捕获特定类型
来源：https://uc.zhonguo2118.cn

Py:   except ValueError as e:
来源：https://qx.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://ig.zhonguo2118.cn

JS:   if (e instanceof TypeError) {}
来源：https://jl.zhonguo4118.cn

TS:   if (e instanceof TypeError) {}
来源：https://zf.zhonguo1118.cn

Java: catch (IOException | SQLException e) {}
来源：https://yx.zhonguo4118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://vc.zhonguo3118.cn

Ruby: rescue ArgumentError => e
来源：https://yh.zhonguo7118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://em.zhonguo6118.cn

[H06] 可选值 / 空值安全访问
来源：https://oz.zhonguo1118.cn

Py:   value = d.get("k") or default
来源：https://az.zhonguo7118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://oe.zhonguo4118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://jd.zhonguo4118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://vu.zhonguo2118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ql.zhonguo3118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://im.zhonguo6118.cn

Ruby: d&.dig(:a, :b)
来源：https://qb.zhonguo3118.cn

C#:   obj?.A?.B ?? default
来源：https://oq.zhonguo2118.cn

[H07] 断言
来源：https://bd.zhonguo4118.cn

Py:   assert x > 0, "必须为正"
来源：https://zm.zhonguo3118.cn

PHP:  assert($x > 0);
来源：https://kr.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://fg.zhonguo4118.cn

TS:   console.assert(x > 0);
来源：https://jt.zhonguo3118.cn

Java: assert x > 0 : "必须为正";
来源：https://vm.zhonguo2118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://xb.zhonguo1118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://rz.zhonguo8118.cn

C#:   Debug.Assert(x > 0);
来源：https://qj.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://za.zhonguo3118.cn

Py:   str(e);  traceback.format_exc()
来源：https://ui.zhonguo4118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://cm.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://eb.zhonguo6118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://lk.zhonguo2118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://rm.zhonguo4118.cn

Go:   err.Error()
来源：https://th.zhonguo8118.cn

Ruby: e.message;  e.backtrace
来源：https://yz.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://wq.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://yw.zhonguo8118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://kn.zhonguo5118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://xh.zhonguo7118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://xg.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://dt.zhonguo6118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ey.zhonguo7118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://xd.zhonguo5118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://gg.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://qj.zhonguo2118.cn

[H10] 资源自动释放
来源：https://cb.zhonguo1118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://cv.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://vz.zhonguo4118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://gv.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://iv.zhonguo8118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://jp.zhonguo1118.cn

Go:   defer f.Close()
来源：https://kw.zhonguo8118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ze.zhonguo7118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://ei.zhonguo6118.cn

================================================================================
来源：https://dp.zhonguo6118.cn

I. 正则表达式
来源：https://ci.zhonguo5118.cn

================================================================================
来源：https://dy.zhonguo1118.cn

[I01] 判断是否匹配
来源：https://ch.zhonguo2118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://uh.zhonguo4118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://uj.zhonguo1118.cn

JS:   /\d+/.test(s)
来源：https://tb.zhonguo7118.cn

TS:   /\d+/.test(s)
来源：https://bu.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://jn.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://xw.zhonguo7118.cn

Ruby: s.match?(/\d+/)
来源：https://lu.zhonguo8118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://jn.zhonguo4118.cn

[I02] 提取所有匹配
来源：https://cd.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://wf.zhonguo1118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ew.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://fn.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://ry.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://lw.zhonguo7118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://zk.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://jk.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://gn.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://eb.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://jm.zhonguo2118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://mz.zhonguo6118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://zc.zhonguo4118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://gw.zhonguo1118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://bc.zhonguo2118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://bt.zhonguo6118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://qa.zhonguo7118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://mq.zhonguo3118.cn

[I04] 正则替换
来源：https://yk.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://kr.zhonguo1118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://aj.zhonguo4118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://ze.zhonguo8118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://tq.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://yq.zhonguo4118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://ck.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ml.zhonguo4118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://gs.zhonguo8118.cn

[I05] 按正则拆分
来源：https://qj.zhonguo6118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://jf.zhonguo4118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://qk.zhonguo8118.cn

JS:   s.split(/\s*,\s*/)
来源：https://qo.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://fs.zhonguo1118.cn

Java: s.split("\\s*,\\s*")
来源：https://jv.zhonguo5118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://ew.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://qg.zhonguo8118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://pd.zhonguo7118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://wr.zhonguo1118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://em.zhonguo3118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://ic.zhonguo6118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://wb.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://wg.zhonguo5118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://rl.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://bn.zhonguo7118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://vq.zhonguo5118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://av.zhonguo5118.cn

[I07] 忽略大小写与多行模式
来源：https://ed.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://zs.zhonguo7118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://sd.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://kr.zhonguo6118.cn

TS:   /error/gim
来源：https://bl.zhonguo7118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://uk.zhonguo7118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://yo.zhonguo8118.cn

Ruby: s.scan(/error/i)
来源：https://eh.zhonguo5118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://hs.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://vx.zhonguo1118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://rf.zhonguo7118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://ao.zhonguo8118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://un.zhonguo5118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://fu.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://vv.zhonguo2118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://lo.zhonguo8118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://xz.zhonguo5118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://au.zhonguo6118.cn

================================================================================
来源：https://le.zhonguo2118.cn

J. 日期与时间
来源：https://xk.zhonguo2118.cn

================================================================================
来源：https://gp.zhonguo3118.cn

[J01] 获取当前时间
来源：https://ru.zhonguo2118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://uf.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://qf.zhonguo3118.cn

JS:   new Date();  Date.now()
来源：https://ii.zhonguo7118.cn

TS:   new Date();  Date.now()
来源：https://dc.zhonguo6118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://uq.zhonguo8118.cn

Go:   time.Now()
来源：https://tu.zhonguo7118.cn

Ruby: Time.now
来源：https://ht.zhonguo6118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://hy.zhonguo6118.cn

[J02] 格式化输出
来源：https://uv.zhonguo4118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://vj.zhonguo6118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://ic.zhonguo4118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://po.zhonguo7118.cn

TS:   d.toISOString()
来源：https://fb.zhonguo1118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://zi.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://rl.zhonguo5118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://gr.zhonguo6118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://ea.zhonguo2118.cn

[J03] 字符串解析为日期
来源：https://dn.zhonguo6118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://ft.zhonguo1118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://vk.zhonguo4118.cn

JS:   new Date("2024-01-02")
来源：https://qu.zhonguo1118.cn

TS:   new Date("2024-01-02")
来源：https://qo.zhonguo4118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://cx.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://of.zhonguo3118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ay.zhonguo7118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://pl.zhonguo8118.cn

[J04] 时间戳与日期互转
来源：https://df.zhonguo1118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://pi.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://ya.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://tl.zhonguo4118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://ua.zhonguo3118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://rk.zhonguo5118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://ub.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://py.zhonguo1118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ha.zhonguo8118.cn

[J05] 时间加减（加 7 天）
来源：https://mg.zhonguo7118.cn

Py:   now + timedelta(days=7)
来源：https://in.zhonguo2118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://gq.zhonguo7118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://vw.zhonguo5118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://fe.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://nq.zhonguo6118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://uc.zhonguo2118.cn

Ruby: Time.now + 7 * 86400
来源：https://dk.zhonguo8118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://qa.zhonguo3118.cn

[J06] 计算两时间之差
来源：https://of.zhonguo6118.cn

Py:   (end - start).total_seconds()
来源：https://lc.zhonguo3118.cn

PHP:  $end->diff($start)->days;
来源：https://na.zhonguo6118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://hh.zhonguo4118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://ty.zhonguo7118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://jr.zhonguo6118.cn

Go:   end.Sub(start).Hours()
来源：https://ke.zhonguo5118.cn

Ruby: end - start                 # 返回秒数
来源：https://tf.zhonguo4118.cn

C#:   (end - start).TotalSeconds
来源：https://le.zhonguo2118.cn

[J07] 比较两个日期
来源：https://ko.zhonguo5118.cn

Py:   d1 < d2;  d1 == d2
来源：https://ip.zhonguo7118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://hb.zhonguo5118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ic.zhonguo3118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://mu.zhonguo8118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://tf.zhonguo1118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ye.zhonguo8118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://jk.zhonguo6118.cn

C#:   d1 < d2;  d1 == d2
来源：https://el.zhonguo7118.cn

[J08] 提取年月日与星期
来源：https://pi.zhonguo1118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://qs.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://bt.zhonguo2118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://zf.zhonguo4118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://px.zhonguo1118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://cb.zhonguo4118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://lb.zhonguo7118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://yj.zhonguo8118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://xl.zhonguo5118.cn

[J09] 时区处理
来源：https://gv.zhonguo1118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://ow.zhonguo1118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://ac.zhonguo2118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://xt.zhonguo6118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://oe.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://bz.zhonguo4118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://gp.zhonguo1118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://af.zhonguo3118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://yo.zhonguo7118.cn

[J10] 取今天 / 本月第一天
来源：https://ty.zhonguo1118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://to.zhonguo1118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://vs.zhonguo3118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://wh.zhonguo5118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://fk.zhonguo8118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ck.zhonguo1118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://zc.zhonguo8118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ys.zhonguo7118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://pk.zhonguo8118.cn

================================================================================
来源：https://zc.zhonguo6118.cn

K. JSON 与序列化
来源：https://yv.zhonguo7118.cn

================================================================================
来源：https://tz.zhonguo1118.cn

[K01] 对象转 JSON 字符串
来源：https://lb.zhonguo4118.cn


<!-- 参考信息 -->