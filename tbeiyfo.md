代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：https://lz.zhonguo1118.cn

Ruby: obj.instance_variables
来源：https://wk.zhonguo6118.cn

C#:   // 用反射或 System.Text.Json
来源：https://nu.zhonguo5118.cn

================================================================================
来源：https://gs.zhonguo2118.cn

H. 异常与错误处理
来源：https://lq.zhonguo3118.cn

================================================================================
来源：https://fv.zhonguo6118.cn

[H01] try / catch 基础
来源：https://dk.zhonguo2118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://lw.zhonguo2118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://zb.zhonguo1118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://tu.zhonguo3118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://ba.zhonguo4118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://lh.zhonguo4118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://an.zhonguo1118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://ln.zhonguo6118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://pq.zhonguo6118.cn

[H02] finally / ensure 收尾
来源：https://jo.zhonguo1118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://dg.zhonguo1118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://lt.zhonguo4118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://cc.zhonguo8118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://by.zhonguo2118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ki.zhonguo5118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://si.zhonguo8118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://gg.zhonguo2118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://ia.zhonguo5118.cn

[H03] 主动抛出异常
来源：https://pl.zhonguo3118.cn

Py:   raise ValueError("错误信息")
来源：https://ff.zhonguo8118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://gw.zhonguo6118.cn

JS:   throw new Error("错误信息");
来源：https://vb.zhonguo4118.cn

TS:   throw new Error("错误信息");
来源：https://ma.zhonguo8118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://ho.zhonguo4118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://ct.zhonguo8118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://ck.zhonguo7118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://fz.zhonguo4118.cn

[H04] 自定义异常类型
来源：https://ss.zhonguo1118.cn

Py:   class MyError(Exception): pass
来源：https://nc.zhonguo4118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://xx.zhonguo1118.cn

JS:   class MyError extends Error {}
来源：https://wd.zhonguo2118.cn

TS:   class MyError extends Error {}
来源：https://dg.zhonguo5118.cn

Java: class MyException extends RuntimeException {}
来源：https://vk.zhonguo5118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://jx.zhonguo8118.cn

Ruby: class MyError < StandardError; end
来源：https://xp.zhonguo3118.cn

C#:   class MyException : Exception {}
来源：https://cj.zhonguo1118.cn

[H05] 捕获特定类型
来源：https://ti.zhonguo2118.cn

Py:   except ValueError as e:
来源：https://uj.zhonguo2118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://do.zhonguo8118.cn

JS:   if (e instanceof TypeError) {}
来源：https://dt.zhonguo1118.cn

TS:   if (e instanceof TypeError) {}
来源：https://in.zhonguo4118.cn

Java: catch (IOException | SQLException e) {}
来源：https://be.zhonguo2118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://wu.zhonguo4118.cn

Ruby: rescue ArgumentError => e
来源：https://mn.zhonguo1118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://ma.zhonguo2118.cn

[H06] 可选值 / 空值安全访问
来源：https://no.zhonguo3118.cn

Py:   value = d.get("k") or default
来源：https://lq.zhonguo8118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://mt.zhonguo7118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://jl.zhonguo3118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://zh.zhonguo6118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://uw.zhonguo1118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ig.zhonguo1118.cn

Ruby: d&.dig(:a, :b)
来源：https://ml.zhonguo5118.cn

C#:   obj?.A?.B ?? default
来源：https://nc.zhonguo1118.cn

[H07] 断言
来源：https://me.zhonguo3118.cn

Py:   assert x > 0, "必须为正"
来源：https://ur.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://sx.zhonguo1118.cn

JS:   console.assert(x > 0);
来源：https://br.zhonguo7118.cn

TS:   console.assert(x > 0);
来源：https://ag.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://rq.zhonguo7118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://uf.zhonguo7118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://kx.zhonguo4118.cn

C#:   Debug.Assert(x > 0);
来源：https://dd.zhonguo2118.cn

[H08] 获取错误信息与堆栈
来源：https://gp.zhonguo2118.cn

Py:   str(e);  traceback.format_exc()
来源：https://bx.zhonguo5118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://jj.zhonguo5118.cn

JS:   e.message;  e.stack
来源：https://at.zhonguo1118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://xy.zhonguo7118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://ea.zhonguo4118.cn

Go:   err.Error()
来源：https://by.zhonguo7118.cn

Ruby: e.message;  e.backtrace
来源：https://tr.zhonguo5118.cn

C#:   e.Message;  e.StackTrace
来源：https://pf.zhonguo1118.cn

[H09] 带错误码的异常
来源：https://ct.zhonguo2118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://gd.zhonguo5118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://nb.zhonguo2118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://no.zhonguo5118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://bm.zhonguo4118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://eb.zhonguo6118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://ez.zhonguo1118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://jx.zhonguo5118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://ps.zhonguo4118.cn

[H10] 资源自动释放
来源：https://iz.zhonguo2118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://fe.zhonguo5118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://sb.zhonguo5118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://rd.zhonguo8118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://kx.zhonguo2118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://fj.zhonguo7118.cn

Go:   defer f.Close()
来源：https://kl.zhonguo3118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://ax.zhonguo2118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://nk.zhonguo3118.cn

================================================================================
来源：https://yq.zhonguo1118.cn

I. 正则表达式
来源：https://hb.zhonguo3118.cn

================================================================================
来源：https://sr.zhonguo5118.cn

[I01] 判断是否匹配
来源：https://dk.zhonguo5118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://me.zhonguo6118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://ep.zhonguo4118.cn

JS:   /\d+/.test(s)
来源：https://dg.zhonguo7118.cn

TS:   /\d+/.test(s)
来源：https://us.zhonguo4118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://mj.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://sr.zhonguo4118.cn

Ruby: s.match?(/\d+/)
来源：https://fa.zhonguo6118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://cx.zhonguo4118.cn

[I02] 提取所有匹配
来源：https://mp.zhonguo5118.cn

Py:   re.findall(r"\d+", s)
来源：https://ox.zhonguo4118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://on.zhonguo4118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://tm.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://he.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://cq.zhonguo1118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://km.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://xo.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://fv.zhonguo4118.cn

[I03] 提取捕获分组
来源：https://qv.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://xj.zhonguo4118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://tt.zhonguo8118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://wq.zhonguo4118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://sc.zhonguo7118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://yt.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://ai.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://lb.zhonguo4118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://by.zhonguo2118.cn

[I04] 正则替换
来源：https://hv.zhonguo5118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://nn.zhonguo6118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://pn.zhonguo7118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://va.zhonguo5118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://ur.zhonguo6118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://ai.zhonguo1118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://qd.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://ks.zhonguo1118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://gp.zhonguo8118.cn

[I05] 按正则拆分
来源：https://jb.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://vz.zhonguo6118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://ei.zhonguo2118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ui.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://vt.zhonguo5118.cn

Java: s.split("\\s*,\\s*")
来源：https://de.zhonguo7118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://lr.zhonguo2118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://el.zhonguo7118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://gh.zhonguo8118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://ev.zhonguo8118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://wl.zhonguo4118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://lp.zhonguo8118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://qm.zhonguo7118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://zw.zhonguo2118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://rb.zhonguo6118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://lp.zhonguo2118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://oq.zhonguo4118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://pg.zhonguo8118.cn

[I07] 忽略大小写与多行模式
来源：https://sf.zhonguo4118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://wd.zhonguo5118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://th.zhonguo6118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://xl.zhonguo3118.cn

TS:   /error/gim
来源：https://se.zhonguo1118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ta.zhonguo1118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://jb.zhonguo2118.cn

Ruby: s.scan(/error/i)
来源：https://kh.zhonguo8118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://nz.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://zt.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://gx.zhonguo8118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://dr.zhonguo6118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://dc.zhonguo2118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://rx.zhonguo7118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://il.zhonguo8118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://mv.zhonguo1118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://ih.zhonguo3118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ax.zhonguo3118.cn

================================================================================
来源：https://jo.zhonguo2118.cn

J. 日期与时间
来源：https://ua.zhonguo7118.cn

================================================================================
来源：https://ca.zhonguo5118.cn

[J01] 获取当前时间
来源：https://wq.zhonguo8118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://si.zhonguo1118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://bc.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://od.zhonguo3118.cn

TS:   new Date();  Date.now()
来源：https://xu.zhonguo6118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://xt.zhonguo1118.cn

Go:   time.Now()
来源：https://zr.zhonguo3118.cn

Ruby: Time.now
来源：https://ux.zhonguo6118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://kc.zhonguo8118.cn

[J02] 格式化输出
来源：https://fn.zhonguo5118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://ty.zhonguo7118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://qp.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://do.zhonguo6118.cn

TS:   d.toISOString()
来源：https://kz.zhonguo6118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://nn.zhonguo6118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://jt.zhonguo7118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://sb.zhonguo6118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://wp.zhonguo8118.cn

[J03] 字符串解析为日期
来源：https://mq.zhonguo1118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://qq.zhonguo3118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://ii.zhonguo6118.cn

JS:   new Date("2024-01-02")
来源：https://cj.zhonguo2118.cn

TS:   new Date("2024-01-02")
来源：https://mh.zhonguo3118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://qj.zhonguo4118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://qu.zhonguo4118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ar.zhonguo5118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ox.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://fo.zhonguo2118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://qf.zhonguo6118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://wo.zhonguo2118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://tp.zhonguo6118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://rv.zhonguo1118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://hm.zhonguo3118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://jd.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://yt.zhonguo8118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://mi.zhonguo7118.cn

[J05] 时间加减（加 7 天）
来源：https://ir.zhonguo2118.cn

Py:   now + timedelta(days=7)
来源：https://xu.zhonguo8118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://zi.zhonguo7118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://uf.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://mt.zhonguo4118.cn

Java: LocalDate.now().plusDays(7)
来源：https://mb.zhonguo1118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://hb.zhonguo1118.cn

Ruby: Time.now + 7 * 86400
来源：https://qu.zhonguo7118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://un.zhonguo8118.cn

[J06] 计算两时间之差
来源：https://px.zhonguo1118.cn

Py:   (end - start).total_seconds()
来源：https://sk.zhonguo1118.cn

PHP:  $end->diff($start)->days;
来源：https://ym.zhonguo5118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://kf.zhonguo6118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://mg.zhonguo4118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://jv.zhonguo4118.cn

Go:   end.Sub(start).Hours()
来源：https://kb.zhonguo7118.cn

Ruby: end - start                 # 返回秒数
来源：https://si.zhonguo7118.cn

C#:   (end - start).TotalSeconds
来源：https://pi.zhonguo7118.cn

[J07] 比较两个日期
来源：https://ng.zhonguo8118.cn

Py:   d1 < d2;  d1 == d2
来源：https://vu.zhonguo2118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://yw.zhonguo3118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ot.zhonguo4118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://ws.zhonguo3118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://pj.zhonguo6118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://jp.zhonguo5118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://gv.zhonguo4118.cn

C#:   d1 < d2;  d1 == d2
来源：https://do.zhonguo5118.cn

[J08] 提取年月日与星期
来源：https://hs.zhonguo2118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://xg.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://fb.zhonguo6118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://ej.zhonguo6118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://cj.zhonguo6118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://pf.zhonguo3118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://rz.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ox.zhonguo7118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://lv.zhonguo7118.cn

[J09] 时区处理
来源：https://oy.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://yd.zhonguo3118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://vf.zhonguo1118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ea.zhonguo7118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://os.zhonguo6118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://hz.zhonguo5118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ne.zhonguo5118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://kz.zhonguo1118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://vj.zhonguo4118.cn

[J10] 取今天 / 本月第一天
来源：https://li.zhonguo8118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://zy.zhonguo8118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://ps.zhonguo4118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://vk.zhonguo1118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://nz.zhonguo6118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://bc.zhonguo3118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://cd.zhonguo6118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://kh.zhonguo1118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://yn.zhonguo6118.cn

================================================================================
来源：https://kv.zhonguo2118.cn

K. JSON 与序列化
来源：https://ix.zhonguo6118.cn

================================================================================
来源：https://ax.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://bp.zhonguo8118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://yh.zhonguo5118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://ou.zhonguo1118.cn

JS:   JSON.stringify(obj)
来源：https://ij.zhonguo3118.cn

TS:   JSON.stringify(obj)
来源：https://sh.zhonguo2118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://cy.zhonguo1118.cn

Go:   json.Marshal(obj)
来源：https://ov.zhonguo5118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://qo.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://zi.zhonguo7118.cn

[K02] JSON 字符串转对象
来源：https://rf.zhonguo4118.cn

Py:   json.loads(s)
来源：https://ed.zhonguo2118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://vn.zhonguo8118.cn

JS:   JSON.parse(s)
来源：https://hs.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://tg.zhonguo7118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://dg.zhonguo4118.cn

Go:   json.Unmarshal(data, &v)
来源：https://wu.zhonguo2118.cn

Ruby: JSON.parse(s)
来源：https://ur.zhonguo3118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://kn.zhonguo4118.cn

[K03] JSON 美化输出（带缩进）
来源：https://jd.zhonguo5118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://ke.zhonguo5118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://pk.zhonguo6118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://ac.zhonguo7118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://oa.zhonguo8118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://wq.zhonguo7118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://zu.zhonguo6118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://og.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://kz.zhonguo2118.cn

[K04] 读取 JSON 文件
来源：https://lf.zhonguo3118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://od.zhonguo7118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://ke.zhonguo7118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://qq.zhonguo5118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://vr.zhonguo5118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://nj.zhonguo1118.cn


<!-- 参考信息 -->