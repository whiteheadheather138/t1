代发 wailian999

PHP:  get_object_vars($obj);
来源：https://kf.zhonguo4118.cn

JS:   Object.entries(obj)
来源：https://ak.zhonguo5118.cn

TS:   Object.entries(obj)
来源：https://qy.zhonguo6118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://qz.zhonguo7118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://wj.zhonguo8118.cn

Ruby: obj.instance_variables
来源：https://pc.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://eu.zhonguo7118.cn

================================================================================
来源：https://uy.zhonguo1118.cn

H. 异常与错误处理
来源：https://fu.zhonguo1118.cn

================================================================================
来源：https://ys.zhonguo8118.cn

[H01] try / catch 基础
来源：https://yi.zhonguo3118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://oa.zhonguo1118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://jz.zhonguo3118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://me.zhonguo5118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://tx.zhonguo6118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://yv.zhonguo2118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://ue.zhonguo2118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://um.zhonguo6118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://ae.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://up.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://fz.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://al.zhonguo7118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://ct.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://dl.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://nc.zhonguo4118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://na.zhonguo5118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://zs.zhonguo1118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://vd.zhonguo3118.cn

[H03] 主动抛出异常
来源：https://sj.zhonguo3118.cn

Py:   raise ValueError("错误信息")
来源：https://mr.zhonguo2118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://zh.zhonguo2118.cn

JS:   throw new Error("错误信息");
来源：https://pw.zhonguo3118.cn

TS:   throw new Error("错误信息");
来源：https://zl.zhonguo3118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://xj.zhonguo3118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://rx.zhonguo2118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://mz.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://sp.zhonguo2118.cn

[H04] 自定义异常类型
来源：https://ij.zhonguo3118.cn

Py:   class MyError(Exception): pass
来源：https://jd.zhonguo2118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://qg.zhonguo4118.cn

JS:   class MyError extends Error {}
来源：https://si.zhonguo6118.cn

TS:   class MyError extends Error {}
来源：https://qe.zhonguo8118.cn

Java: class MyException extends RuntimeException {}
来源：https://yu.zhonguo3118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://pl.zhonguo1118.cn

Ruby: class MyError < StandardError; end
来源：https://nq.zhonguo6118.cn

C#:   class MyException : Exception {}
来源：https://re.zhonguo7118.cn

[H05] 捕获特定类型
来源：https://fn.zhonguo6118.cn

Py:   except ValueError as e:
来源：https://rc.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://jq.zhonguo4118.cn

JS:   if (e instanceof TypeError) {}
来源：https://zp.zhonguo2118.cn

TS:   if (e instanceof TypeError) {}
来源：https://in.zhonguo7118.cn

Java: catch (IOException | SQLException e) {}
来源：https://xp.zhonguo8118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://bc.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://ke.zhonguo6118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://dv.zhonguo4118.cn

[H06] 可选值 / 空值安全访问
来源：https://ws.zhonguo5118.cn

Py:   value = d.get("k") or default
来源：https://xu.zhonguo3118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://nn.zhonguo5118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://lv.zhonguo6118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://fs.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://my.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://js.zhonguo7118.cn

Ruby: d&.dig(:a, :b)
来源：https://tc.zhonguo4118.cn

C#:   obj?.A?.B ?? default
来源：https://pq.zhonguo5118.cn

[H07] 断言
来源：https://vm.zhonguo2118.cn

Py:   assert x > 0, "必须为正"
来源：https://dp.zhonguo7118.cn

PHP:  assert($x > 0);
来源：https://pp.zhonguo8118.cn

JS:   console.assert(x > 0);
来源：https://wm.zhonguo6118.cn

TS:   console.assert(x > 0);
来源：https://jr.zhonguo2118.cn

Java: assert x > 0 : "必须为正";
来源：https://wa.zhonguo4118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://ev.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ki.zhonguo6118.cn

C#:   Debug.Assert(x > 0);
来源：https://qy.zhonguo7118.cn

[H08] 获取错误信息与堆栈
来源：https://ng.zhonguo4118.cn

Py:   str(e);  traceback.format_exc()
来源：https://fh.zhonguo5118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://au.zhonguo7118.cn

JS:   e.message;  e.stack
来源：https://ss.zhonguo6118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://dc.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ql.zhonguo3118.cn

Go:   err.Error()
来源：https://cd.zhonguo3118.cn

Ruby: e.message;  e.backtrace
来源：https://ut.zhonguo7118.cn

C#:   e.Message;  e.StackTrace
来源：https://hw.zhonguo6118.cn

[H09] 带错误码的异常
来源：https://yp.zhonguo5118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://ha.zhonguo3118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://et.zhonguo3118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://kh.zhonguo1118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://op.zhonguo8118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://zq.zhonguo4118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://do.zhonguo5118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ac.zhonguo7118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ln.zhonguo6118.cn

[H10] 资源自动释放
来源：https://lt.zhonguo5118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://io.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://jp.zhonguo5118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://qh.zhonguo3118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ij.zhonguo6118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://qx.zhonguo4118.cn

Go:   defer f.Close()
来源：https://ay.zhonguo6118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ii.zhonguo2118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://jj.zhonguo2118.cn

================================================================================
来源：https://ql.zhonguo2118.cn

I. 正则表达式
来源：https://qi.zhonguo3118.cn

================================================================================
来源：https://fh.zhonguo3118.cn

[I01] 判断是否匹配
来源：https://pd.zhonguo8118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://yc.zhonguo2118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://rr.zhonguo5118.cn

JS:   /\d+/.test(s)
来源：https://bg.zhonguo1118.cn

TS:   /\d+/.test(s)
来源：https://rq.zhonguo8118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://bq.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://jz.zhonguo1118.cn

Ruby: s.match?(/\d+/)
来源：https://sn.zhonguo3118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://kx.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://ed.zhonguo3118.cn

Py:   re.findall(r"\d+", s)
来源：https://hk.zhonguo3118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ib.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://hz.zhonguo8118.cn

TS:   s.match(/\d+/g)
来源：https://kp.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ke.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ia.zhonguo4118.cn

Ruby: s.scan(/\d+/)
来源：https://tk.zhonguo4118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://tr.zhonguo2118.cn

[I03] 提取捕获分组
来源：https://ka.zhonguo6118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://xv.zhonguo5118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://nm.zhonguo4118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://ii.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://rm.zhonguo2118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://mf.zhonguo1118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://th.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ce.zhonguo6118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://oo.zhonguo6118.cn

[I04] 正则替换
来源：https://gh.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://hi.zhonguo7118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://ew.zhonguo3118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://hp.zhonguo1118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://du.zhonguo1118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://kl.zhonguo4118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://yr.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://nw.zhonguo2118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://zo.zhonguo7118.cn

[I05] 按正则拆分
来源：https://bi.zhonguo4118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://ey.zhonguo3118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://gf.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://lm.zhonguo2118.cn

TS:   s.split(/\s*,\s*/)
来源：https://iv.zhonguo1118.cn

Java: s.split("\\s*,\\s*")
来源：https://gi.zhonguo5118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://gp.zhonguo2118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://zr.zhonguo2118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://hs.zhonguo3118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://oq.zhonguo5118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://sb.zhonguo4118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://mm.zhonguo6118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://xc.zhonguo2118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://so.zhonguo8118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://jp.zhonguo1118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://jh.zhonguo3118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://un.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://xv.zhonguo7118.cn

[I07] 忽略大小写与多行模式
来源：https://sy.zhonguo6118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://ay.zhonguo5118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://ba.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://ey.zhonguo3118.cn

TS:   /error/gim
来源：https://gb.zhonguo5118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://jp.zhonguo6118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://yo.zhonguo5118.cn

Ruby: s.scan(/error/i)
来源：https://vc.zhonguo5118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://ua.zhonguo3118.cn

[I08] 贪婪与非贪婪匹配
来源：https://kg.zhonguo8118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ub.zhonguo8118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://co.zhonguo7118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://li.zhonguo5118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://vs.zhonguo4118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://be.zhonguo8118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://pw.zhonguo2118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://jj.zhonguo6118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://md.zhonguo4118.cn

================================================================================
来源：https://gj.zhonguo4118.cn

J. 日期与时间
来源：https://py.zhonguo5118.cn

================================================================================
来源：https://ju.zhonguo5118.cn

[J01] 获取当前时间
来源：https://kg.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://cb.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://sj.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://ei.zhonguo1118.cn

TS:   new Date();  Date.now()
来源：https://cp.zhonguo4118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://cm.zhonguo2118.cn

Go:   time.Now()
来源：https://hz.zhonguo7118.cn

Ruby: Time.now
来源：https://jl.zhonguo4118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://cm.zhonguo2118.cn

[J02] 格式化输出
来源：https://ot.zhonguo5118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://by.zhonguo8118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://pn.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://ki.zhonguo1118.cn

TS:   d.toISOString()
来源：https://pg.zhonguo1118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://dd.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://dp.zhonguo6118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://fb.zhonguo2118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://wc.zhonguo5118.cn

[J03] 字符串解析为日期
来源：https://tp.zhonguo2118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://yz.zhonguo3118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://rb.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://kz.zhonguo3118.cn

TS:   new Date("2024-01-02")
来源：https://fy.zhonguo4118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://un.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://qw.zhonguo8118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ef.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://lz.zhonguo2118.cn

[J04] 时间戳与日期互转
来源：https://vt.zhonguo4118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://pt.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://lv.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://xa.zhonguo5118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://nb.zhonguo8118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://fd.zhonguo6118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://ci.zhonguo7118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://fr.zhonguo8118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://re.zhonguo4118.cn

[J05] 时间加减（加 7 天）
来源：https://cf.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://xd.zhonguo6118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://pm.zhonguo6118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://jn.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://nm.zhonguo6118.cn

Java: LocalDate.now().plusDays(7)
来源：https://xf.zhonguo7118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://fb.zhonguo3118.cn

Ruby: Time.now + 7 * 86400
来源：https://hs.zhonguo8118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://ns.zhonguo8118.cn

[J06] 计算两时间之差
来源：https://tu.zhonguo1118.cn

Py:   (end - start).total_seconds()
来源：https://ya.zhonguo7118.cn

PHP:  $end->diff($start)->days;
来源：https://ts.zhonguo5118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://au.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://gh.zhonguo7118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://an.zhonguo5118.cn

Go:   end.Sub(start).Hours()
来源：https://ch.zhonguo1118.cn

Ruby: end - start                 # 返回秒数
来源：https://mk.zhonguo8118.cn

C#:   (end - start).TotalSeconds
来源：https://xu.zhonguo7118.cn

[J07] 比较两个日期
来源：https://xa.zhonguo8118.cn

Py:   d1 < d2;  d1 == d2
来源：https://hz.zhonguo5118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://up.zhonguo3118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://tl.zhonguo5118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://da.zhonguo8118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://vn.zhonguo4118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://ta.zhonguo2118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://kg.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://tr.zhonguo3118.cn

[J08] 提取年月日与星期
来源：https://yh.zhonguo8118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://rp.zhonguo6118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://hz.zhonguo3118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://bm.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://cp.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://bk.zhonguo2118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://hz.zhonguo8118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://zi.zhonguo7118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://dl.zhonguo3118.cn

[J09] 时区处理
来源：https://jh.zhonguo8118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://ip.zhonguo6118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://na.zhonguo3118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://jm.zhonguo5118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://so.zhonguo6118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://rj.zhonguo6118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ps.zhonguo1118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://rq.zhonguo1118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://ed.zhonguo1118.cn

[J10] 取今天 / 本月第一天
来源：https://co.zhonguo5118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://op.zhonguo7118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://rn.zhonguo8118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://tj.zhonguo8118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://ym.zhonguo4118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://uq.zhonguo1118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://my.zhonguo6118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ba.zhonguo6118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://mz.zhonguo1118.cn

================================================================================
来源：https://zd.zhonguo5118.cn

K. JSON 与序列化
来源：https://ni.zhonguo2118.cn

================================================================================
来源：https://pe.zhonguo6118.cn

[K01] 对象转 JSON 字符串
来源：https://vd.zhonguo1118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://jr.zhonguo8118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://fq.zhonguo7118.cn

JS:   JSON.stringify(obj)
来源：https://ev.zhonguo8118.cn

TS:   JSON.stringify(obj)
来源：https://hi.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://dn.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://ou.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://ib.zhonguo8118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://hc.zhonguo7118.cn

[K02] JSON 字符串转对象
来源：https://ok.zhonguo6118.cn

Py:   json.loads(s)
来源：https://eo.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://ug.zhonguo2118.cn

JS:   JSON.parse(s)
来源：https://sm.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://iv.zhonguo1118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://uj.zhonguo7118.cn

Go:   json.Unmarshal(data, &v)
来源：https://iw.zhonguo2118.cn

Ruby: JSON.parse(s)
来源：https://hq.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://bs.zhonguo3118.cn

[K03] JSON 美化输出（带缩进）
来源：https://nb.zhonguo1118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://ms.zhonguo4118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://rl.zhonguo4118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://aj.zhonguo2118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://fo.zhonguo7118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://dv.zhonguo8118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://mp.zhonguo2118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://ot.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://wb.zhonguo2118.cn

[K04] 读取 JSON 文件
来源：https://bt.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://ig.zhonguo3118.cn


<!-- 参考信息 -->