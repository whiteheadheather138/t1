代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://zr.zhonguo5118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://qh.zhonguo1118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ej.zhonguo1118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://dt.zhonguo5118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://vi.zhonguo1118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ok.zhonguo2118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://wp.zhonguo4118.cn

[H02] finally / ensure 收尾
来源：https://fk.zhonguo6118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://lc.zhonguo5118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://xo.zhonguo3118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://ca.zhonguo5118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://uw.zhonguo6118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://my.zhonguo7118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://ud.zhonguo7118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://yi.zhonguo4118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://cg.zhonguo6118.cn

[H03] 主动抛出异常
来源：https://az.zhonguo6118.cn

Py:   raise ValueError("错误信息")
来源：https://ki.zhonguo6118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://lp.zhonguo7118.cn

JS:   throw new Error("错误信息");
来源：https://aw.zhonguo2118.cn

TS:   throw new Error("错误信息");
来源：https://gq.zhonguo2118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://re.zhonguo3118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ng.zhonguo5118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://vm.zhonguo1118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://qa.zhonguo1118.cn

[H04] 自定义异常类型
来源：https://im.zhonguo5118.cn

Py:   class MyError(Exception): pass
来源：https://cv.zhonguo3118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://dq.zhonguo4118.cn

JS:   class MyError extends Error {}
来源：https://bu.zhonguo4118.cn

TS:   class MyError extends Error {}
来源：https://pg.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://zd.zhonguo4118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://cp.zhonguo1118.cn

Ruby: class MyError < StandardError; end
来源：https://ln.zhonguo8118.cn

C#:   class MyException : Exception {}
来源：https://bq.zhonguo6118.cn

[H05] 捕获特定类型
来源：https://ni.zhonguo4118.cn

Py:   except ValueError as e:
来源：https://dv.zhonguo3118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://xk.zhonguo7118.cn

JS:   if (e instanceof TypeError) {}
来源：https://jb.zhonguo7118.cn

TS:   if (e instanceof TypeError) {}
来源：https://ff.zhonguo3118.cn

Java: catch (IOException | SQLException e) {}
来源：https://sp.zhonguo4118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://wg.zhonguo4118.cn

Ruby: rescue ArgumentError => e
来源：https://io.zhonguo6118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://jd.zhonguo1118.cn

[H06] 可选值 / 空值安全访问
来源：https://cj.zhonguo3118.cn

Py:   value = d.get("k") or default
来源：https://tg.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://kx.zhonguo5118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://uk.zhonguo1118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://pv.zhonguo7118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://bp.zhonguo5118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://nd.zhonguo3118.cn

Ruby: d&.dig(:a, :b)
来源：https://ut.zhonguo2118.cn

C#:   obj?.A?.B ?? default
来源：https://kn.zhonguo2118.cn

[H07] 断言
来源：https://vl.zhonguo7118.cn

Py:   assert x > 0, "必须为正"
来源：https://nh.zhonguo1118.cn

PHP:  assert($x > 0);
来源：https://ab.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://gc.zhonguo1118.cn

TS:   console.assert(x > 0);
来源：https://zf.zhonguo1118.cn

Java: assert x > 0 : "必须为正";
来源：https://sm.zhonguo2118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://xg.zhonguo1118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://pq.zhonguo5118.cn

C#:   Debug.Assert(x > 0);
来源：https://rw.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://zh.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://km.zhonguo2118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://ja.zhonguo3118.cn

JS:   e.message;  e.stack
来源：https://vb.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://jq.zhonguo2118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://bd.zhonguo1118.cn

Go:   err.Error()
来源：https://sw.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://jr.zhonguo8118.cn

C#:   e.Message;  e.StackTrace
来源：https://su.zhonguo7118.cn

[H09] 带错误码的异常
来源：https://ys.zhonguo3118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://wl.zhonguo8118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://wh.zhonguo4118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://sk.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://qg.zhonguo3118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://qx.zhonguo1118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://dg.zhonguo5118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://ue.zhonguo1118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://sw.zhonguo8118.cn

[H10] 资源自动释放
来源：https://ks.zhonguo6118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://sa.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://tj.zhonguo1118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://jg.zhonguo8118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ui.zhonguo8118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://io.zhonguo6118.cn

Go:   defer f.Close()
来源：https://fk.zhonguo5118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://vf.zhonguo2118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://ze.zhonguo6118.cn

================================================================================
来源：https://jm.zhonguo5118.cn

I. 正则表达式
来源：https://pa.zhonguo7118.cn

================================================================================
来源：https://rt.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://nx.zhonguo6118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://hu.zhonguo1118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://yv.zhonguo2118.cn

JS:   /\d+/.test(s)
来源：https://tj.zhonguo8118.cn

TS:   /\d+/.test(s)
来源：https://jt.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://pu.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://ed.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://bk.zhonguo1118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://kz.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://lx.zhonguo4118.cn

Py:   re.findall(r"\d+", s)
来源：https://xr.zhonguo1118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ut.zhonguo3118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://nm.zhonguo4118.cn

TS:   s.match(/\d+/g)
来源：https://di.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://nh.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://uf.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://td.zhonguo5118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://gz.zhonguo1118.cn

[I03] 提取捕获分组
来源：https://xm.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://jo.zhonguo2118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://wp.zhonguo6118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://cb.zhonguo5118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://gc.zhonguo5118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://cu.zhonguo5118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://qf.zhonguo2118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://uw.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://uv.zhonguo7118.cn

[I04] 正则替换
来源：https://dg.zhonguo8118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://zf.zhonguo3118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://nh.zhonguo3118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://ig.zhonguo5118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://wj.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://iy.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://ny.zhonguo5118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://nq.zhonguo7118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://cy.zhonguo6118.cn

[I05] 按正则拆分
来源：https://kq.zhonguo3118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://wd.zhonguo6118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://gc.zhonguo4118.cn

JS:   s.split(/\s*,\s*/)
来源：https://nl.zhonguo5118.cn

TS:   s.split(/\s*,\s*/)
来源：https://ia.zhonguo5118.cn

Java: s.split("\\s*,\\s*")
来源：https://zv.zhonguo3118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://ft.zhonguo4118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://kn.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://pr.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://qi.zhonguo2118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://pn.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://lu.zhonguo4118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://hm.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://jv.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://yt.zhonguo5118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://jg.zhonguo8118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://fv.zhonguo3118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://ac.zhonguo8118.cn

[I07] 忽略大小写与多行模式
来源：https://xg.zhonguo8118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://un.zhonguo6118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://uz.zhonguo2118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://cb.zhonguo5118.cn

TS:   /error/gim
来源：https://mo.zhonguo4118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://wy.zhonguo2118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://jz.zhonguo6118.cn

Ruby: s.scan(/error/i)
来源：https://zf.zhonguo7118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://ia.zhonguo4118.cn

[I08] 贪婪与非贪婪匹配
来源：https://yn.zhonguo8118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://mb.zhonguo6118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://rl.zhonguo8118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://ow.zhonguo7118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://wo.zhonguo2118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://ni.zhonguo6118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://ev.zhonguo6118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://jv.zhonguo6118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://py.zhonguo5118.cn

================================================================================
来源：https://gs.zhonguo1118.cn

J. 日期与时间
来源：https://hv.zhonguo3118.cn

================================================================================
来源：https://hx.zhonguo5118.cn

[J01] 获取当前时间
来源：https://zu.zhonguo6118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://zi.zhonguo3118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://wo.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://mw.zhonguo5118.cn

TS:   new Date();  Date.now()
来源：https://bo.zhonguo2118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://xr.zhonguo6118.cn

Go:   time.Now()
来源：https://rb.zhonguo1118.cn

Ruby: Time.now
来源：https://ml.zhonguo5118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://ji.zhonguo8118.cn

[J02] 格式化输出
来源：https://on.zhonguo5118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://lz.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://xd.zhonguo5118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://qh.zhonguo3118.cn

TS:   d.toISOString()
来源：https://kp.zhonguo2118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://cy.zhonguo1118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://og.zhonguo1118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://mq.zhonguo3118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://cu.zhonguo8118.cn

[J03] 字符串解析为日期
来源：https://bt.zhonguo3118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://go.zhonguo2118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://vq.zhonguo1118.cn

JS:   new Date("2024-01-02")
来源：https://ea.zhonguo5118.cn

TS:   new Date("2024-01-02")
来源：https://at.zhonguo8118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://dh.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://zd.zhonguo5118.cn

Ruby: Date.parse("2024-01-02")
来源：https://bc.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://um.zhonguo1118.cn

[J04] 时间戳与日期互转
来源：https://fr.zhonguo3118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://vb.zhonguo5118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://cf.zhonguo5118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://ee.zhonguo1118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://fh.zhonguo1118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://bm.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://rn.zhonguo7118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://em.zhonguo4118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ux.zhonguo6118.cn

[J05] 时间加减（加 7 天）
来源：https://gh.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://xq.zhonguo3118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://so.zhonguo2118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://hi.zhonguo7118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://ki.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://ro.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://vs.zhonguo7118.cn

Ruby: Time.now + 7 * 86400
来源：https://kg.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://wa.zhonguo6118.cn

[J06] 计算两时间之差
来源：https://il.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://kb.zhonguo6118.cn

PHP:  $end->diff($start)->days;
来源：https://iy.zhonguo4118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://hh.zhonguo3118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://gj.zhonguo2118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://cj.zhonguo4118.cn

Go:   end.Sub(start).Hours()
来源：https://me.zhonguo2118.cn

Ruby: end - start                 # 返回秒数
来源：https://ql.zhonguo3118.cn

C#:   (end - start).TotalSeconds
来源：https://di.zhonguo7118.cn

[J07] 比较两个日期
来源：https://ys.zhonguo7118.cn

Py:   d1 < d2;  d1 == d2
来源：https://zc.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://qp.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ig.zhonguo4118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://gx.zhonguo7118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://fb.zhonguo8118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://jw.zhonguo6118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://rz.zhonguo8118.cn

C#:   d1 < d2;  d1 == d2
来源：https://xx.zhonguo8118.cn

[J08] 提取年月日与星期
来源：https://gj.zhonguo6118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://od.zhonguo6118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://qv.zhonguo8118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://nc.zhonguo1118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://hx.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://pa.zhonguo6118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://qw.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ov.zhonguo1118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ug.zhonguo2118.cn

[J09] 时区处理
来源：https://jj.zhonguo1118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://zo.zhonguo5118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://pz.zhonguo8118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://yb.zhonguo5118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://lb.zhonguo6118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://nw.zhonguo7118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://hx.zhonguo5118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://cn.zhonguo8118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://ok.zhonguo7118.cn

[J10] 取今天 / 本月第一天
来源：https://qf.zhonguo2118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ki.zhonguo6118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://wh.zhonguo1118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://dd.zhonguo2118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://jh.zhonguo2118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://wn.zhonguo3118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://nz.zhonguo2118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://bi.zhonguo7118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://aw.zhonguo5118.cn

================================================================================
来源：https://ah.zhonguo3118.cn

K. JSON 与序列化
来源：https://jw.zhonguo3118.cn

================================================================================
来源：https://qv.zhonguo5118.cn

[K01] 对象转 JSON 字符串
来源：https://ix.zhonguo1118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://fe.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://nm.zhonguo3118.cn

JS:   JSON.stringify(obj)
来源：https://su.zhonguo2118.cn

TS:   JSON.stringify(obj)
来源：https://ek.zhonguo6118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://mi.zhonguo7118.cn

Go:   json.Marshal(obj)
来源：https://vb.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://kf.zhonguo6118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://yw.zhonguo2118.cn

[K02] JSON 字符串转对象
来源：https://df.zhonguo5118.cn

Py:   json.loads(s)
来源：https://mh.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://is.zhonguo4118.cn

JS:   JSON.parse(s)
来源：https://ij.zhonguo1118.cn

TS:   JSON.parse(s)
来源：https://ol.zhonguo5118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://ti.zhonguo5118.cn

Go:   json.Unmarshal(data, &v)
来源：https://na.zhonguo7118.cn

Ruby: JSON.parse(s)
来源：https://py.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://wa.zhonguo6118.cn

[K03] JSON 美化输出（带缩进）
来源：https://mi.zhonguo6118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://lw.zhonguo2118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://xi.zhonguo4118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://qj.zhonguo3118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://qe.zhonguo7118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://vh.zhonguo5118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://dy.zhonguo4118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://yd.zhonguo5118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://fu.zhonguo3118.cn

[K04] 读取 JSON 文件
来源：https://vp.zhonguo8118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://pn.zhonguo4118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://eb.zhonguo4118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ik.zhonguo8118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://mt.zhonguo7118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://un.zhonguo8118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://uf.zhonguo1118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://zn.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://jz.zhonguo3118.cn

[K05] 深拷贝对象
来源：https://uc.zhonguo4118.cn

Py:   copy.deepcopy(obj)
来源：https://vp.zhonguo6118.cn

PHP:  unserialize(serialize($obj));
来源：https://uh.zhonguo8118.cn

JS:   structuredClone(obj)
来源：https://jd.zhonguo8118.cn

TS:   structuredClone(obj)
来源：https://lk.zhonguo2118.cn


<!-- 参考信息 -->