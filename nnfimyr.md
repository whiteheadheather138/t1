代发 wailian999

Ruby: Color = %i[red green].freeze
来源：https://lt.zhonguo4118.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：https://vc.zhonguo8118.cn

[G16] 对象转数组 / 字典
来源：https://zd.zhonguo4118.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：https://ix.zhonguo1118.cn

PHP:  get_object_vars($obj);
来源：https://bw.zhonguo1118.cn

JS:   Object.entries(obj)
来源：https://mt.zhonguo2118.cn

TS:   Object.entries(obj)
来源：https://uf.zhonguo5118.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：https://zs.zhonguo2118.cn

Go:   // 手写转换，或用 mapstructure 库
来源：https://yd.zhonguo8118.cn

Ruby: obj.instance_variables
来源：https://hh.zhonguo5118.cn

C#:   // 用反射或 System.Text.Json
来源：https://wo.zhonguo3118.cn

================================================================================
来源：https://zm.zhonguo6118.cn

H. 异常与错误处理
来源：https://nr.zhonguo4118.cn

================================================================================
来源：https://il.zhonguo4118.cn

[H01] try / catch 基础
来源：https://lu.zhonguo1118.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：https://qi.zhonguo2118.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：https://jy.zhonguo8118.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：https://lf.zhonguo2118.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：https://lr.zhonguo8118.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：https://ju.zhonguo8118.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：https://zt.zhonguo1118.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：https://fm.zhonguo7118.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：https://cd.zhonguo7118.cn

[H02] finally / ensure 收尾
来源：https://om.zhonguo7118.cn

Py:   try: f()⏎finally: cleanup()
来源：https://op.zhonguo6118.cn

PHP:  try { f(); } finally { cleanup(); }
来源：https://wp.zhonguo5118.cn

JS:   try { f(); } finally { cleanup(); }
来源：https://vq.zhonguo2118.cn

TS:   try { f(); } finally { cleanup(); }
来源：https://ez.zhonguo1118.cn

Java: try { f(); } finally { cleanup(); }
来源：https://ad.zhonguo5118.cn

Go:   defer cleanup()             // 函数返回时执行
来源：https://uf.zhonguo6118.cn

Ruby: begin; f; ensure; cleanup; end
来源：https://cg.zhonguo5118.cn

C#:   try { F(); } finally { Cleanup(); }
来源：https://rk.zhonguo8118.cn

[H03] 主动抛出异常
来源：https://xz.zhonguo4118.cn

Py:   raise ValueError("错误信息")
来源：https://im.zhonguo1118.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：https://js.zhonguo5118.cn

JS:   throw new Error("错误信息");
来源：https://up.zhonguo1118.cn

TS:   throw new Error("错误信息");
来源：https://sx.zhonguo7118.cn

Java: throw new IllegalArgumentException("错误信息");
来源：https://rh.zhonguo2118.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：https://vl.zhonguo6118.cn

Ruby: raise ArgumentError, "错误信息"
来源：https://sg.zhonguo6118.cn

C#:   throw new ArgumentException("错误信息");
来源：https://fb.zhonguo7118.cn

[H04] 自定义异常类型
来源：https://yh.zhonguo3118.cn

Py:   class MyError(Exception): pass
来源：https://iy.zhonguo5118.cn

PHP:  class MyError extends RuntimeException {}
来源：https://xs.zhonguo3118.cn

JS:   class MyError extends Error {}
来源：https://je.zhonguo3118.cn

TS:   class MyError extends Error {}
来源：https://hh.zhonguo4118.cn

Java: class MyException extends RuntimeException {}
来源：https://lz.zhonguo7118.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：https://cm.zhonguo5118.cn

Ruby: class MyError < StandardError; end
来源：https://bi.zhonguo4118.cn

C#:   class MyException : Exception {}
来源：https://jt.zhonguo5118.cn

[H05] 捕获特定类型
来源：https://py.zhonguo1118.cn

Py:   except ValueError as e:
来源：https://pr.zhonguo8118.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：https://fg.zhonguo1118.cn

JS:   if (e instanceof TypeError) {}
来源：https://uu.zhonguo5118.cn

TS:   if (e instanceof TypeError) {}
来源：https://iy.zhonguo5118.cn

Java: catch (IOException | SQLException e) {}
来源：https://tf.zhonguo6118.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：https://vm.zhonguo6118.cn

Ruby: rescue ArgumentError => e
来源：https://rf.zhonguo8118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://vu.zhonguo5118.cn

[H06] 可选值 / 空值安全访问
来源：https://jk.zhonguo6118.cn

Py:   value = d.get("k") or default
来源：https://rj.zhonguo2118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://og.zhonguo6118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://rq.zhonguo3118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://uv.zhonguo7118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://tq.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://ts.zhonguo7118.cn

Ruby: d&.dig(:a, :b)
来源：https://oz.zhonguo5118.cn

C#:   obj?.A?.B ?? default
来源：https://ug.zhonguo7118.cn

[H07] 断言
来源：https://gp.zhonguo2118.cn

Py:   assert x > 0, "必须为正"
来源：https://kl.zhonguo2118.cn

PHP:  assert($x > 0);
来源：https://xw.zhonguo4118.cn

JS:   console.assert(x > 0);
来源：https://vk.zhonguo8118.cn

TS:   console.assert(x > 0);
来源：https://dd.zhonguo5118.cn

Java: assert x > 0 : "必须为正";
来源：https://xm.zhonguo5118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://bj.zhonguo5118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://ha.zhonguo1118.cn

C#:   Debug.Assert(x > 0);
来源：https://ex.zhonguo7118.cn

[H08] 获取错误信息与堆栈
来源：https://py.zhonguo8118.cn

Py:   str(e);  traceback.format_exc()
来源：https://cp.zhonguo8118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://lc.zhonguo5118.cn

JS:   e.message;  e.stack
来源：https://xv.zhonguo3118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://pp.zhonguo6118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://pn.zhonguo1118.cn

Go:   err.Error()
来源：https://ha.zhonguo4118.cn

Ruby: e.message;  e.backtrace
来源：https://iz.zhonguo8118.cn

C#:   e.Message;  e.StackTrace
来源：https://fd.zhonguo4118.cn

[H09] 带错误码的异常
来源：https://th.zhonguo1118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://of.zhonguo2118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://od.zhonguo1118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://vz.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://io.zhonguo1118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://iz.zhonguo8118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://bv.zhonguo7118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://qo.zhonguo5118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://uq.zhonguo4118.cn

[H10] 资源自动释放
来源：https://ub.zhonguo7118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://eg.zhonguo2118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://bo.zhonguo8118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://cy.zhonguo6118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://kk.zhonguo7118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://tr.zhonguo4118.cn

Go:   defer f.Close()
来源：https://gw.zhonguo5118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://av.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://xs.zhonguo8118.cn

================================================================================
来源：https://qd.zhonguo7118.cn

I. 正则表达式
来源：https://to.zhonguo8118.cn

================================================================================
来源：https://su.zhonguo3118.cn

[I01] 判断是否匹配
来源：https://sx.zhonguo3118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://za.zhonguo8118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://us.zhonguo4118.cn

JS:   /\d+/.test(s)
来源：https://fq.zhonguo2118.cn

TS:   /\d+/.test(s)
来源：https://xt.zhonguo7118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://nd.zhonguo2118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://gw.zhonguo8118.cn

Ruby: s.match?(/\d+/)
来源：https://ja.zhonguo7118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://kz.zhonguo3118.cn

[I02] 提取所有匹配
来源：https://wa.zhonguo4118.cn

Py:   re.findall(r"\d+", s)
来源：https://kb.zhonguo4118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://fu.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://hk.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://zf.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://ht.zhonguo3118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ob.zhonguo8118.cn

Ruby: s.scan(/\d+/)
来源：https://rn.zhonguo7118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://hc.zhonguo3118.cn

[I03] 提取捕获分组
来源：https://ua.zhonguo8118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://tv.zhonguo1118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://pn.zhonguo5118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://hv.zhonguo2118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://db.zhonguo8118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://wp.zhonguo7118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://pq.zhonguo8118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://to.zhonguo8118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://fg.zhonguo3118.cn

[I04] 正则替换
来源：https://bu.zhonguo3118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://it.zhonguo5118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://wr.zhonguo8118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://vs.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://fn.zhonguo1118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://hf.zhonguo6118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://vn.zhonguo7118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://oe.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://ua.zhonguo4118.cn

[I05] 按正则拆分
来源：https://sg.zhonguo2118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://rg.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://pw.zhonguo5118.cn

JS:   s.split(/\s*,\s*/)
来源：https://oh.zhonguo3118.cn

TS:   s.split(/\s*,\s*/)
来源：https://od.zhonguo4118.cn

Java: s.split("\\s*,\\s*")
来源：https://te.zhonguo6118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://kn.zhonguo8118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://sw.zhonguo8118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://ea.zhonguo8118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://ct.zhonguo1118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://vx.zhonguo6118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://sp.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://jw.zhonguo5118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://rg.zhonguo4118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://sd.zhonguo4118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://pz.zhonguo1118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://iw.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://gd.zhonguo7118.cn

[I07] 忽略大小写与多行模式
来源：https://ct.zhonguo4118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://vo.zhonguo2118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://kk.zhonguo1118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://iq.zhonguo6118.cn

TS:   /error/gim
来源：https://hx.zhonguo8118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ls.zhonguo7118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://ey.zhonguo6118.cn

Ruby: s.scan(/error/i)
来源：https://wo.zhonguo3118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://dl.zhonguo8118.cn

[I08] 贪婪与非贪婪匹配
来源：https://ug.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://ix.zhonguo6118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://ep.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://dy.zhonguo4118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://pa.zhonguo8118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://oh.zhonguo3118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://ek.zhonguo5118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://qw.zhonguo7118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://el.zhonguo7118.cn

================================================================================
来源：https://hv.zhonguo3118.cn

J. 日期与时间
来源：https://pg.zhonguo3118.cn

================================================================================
来源：https://px.zhonguo6118.cn

[J01] 获取当前时间
来源：https://qi.zhonguo4118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://ll.zhonguo4118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://bf.zhonguo8118.cn

JS:   new Date();  Date.now()
来源：https://af.zhonguo2118.cn

TS:   new Date();  Date.now()
来源：https://ev.zhonguo4118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://ym.zhonguo2118.cn

Go:   time.Now()
来源：https://um.zhonguo5118.cn

Ruby: Time.now
来源：https://jy.zhonguo5118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://ax.zhonguo4118.cn

[J02] 格式化输出
来源：https://bp.zhonguo6118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://zl.zhonguo7118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://sg.zhonguo7118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://cp.zhonguo5118.cn

TS:   d.toISOString()
来源：https://zv.zhonguo6118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://qf.zhonguo7118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://dx.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://bw.zhonguo7118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://gn.zhonguo1118.cn

[J03] 字符串解析为日期
来源：https://ch.zhonguo2118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://hv.zhonguo8118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://sr.zhonguo4118.cn

JS:   new Date("2024-01-02")
来源：https://yx.zhonguo7118.cn

TS:   new Date("2024-01-02")
来源：https://wv.zhonguo1118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://vv.zhonguo4118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://gm.zhonguo8118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ro.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://vo.zhonguo6118.cn

[J04] 时间戳与日期互转
来源：https://vm.zhonguo1118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://pl.zhonguo4118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://jh.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://cj.zhonguo4118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://nv.zhonguo3118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://mc.zhonguo4118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://lf.zhonguo3118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://js.zhonguo7118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://jl.zhonguo1118.cn

[J05] 时间加减（加 7 天）
来源：https://iy.zhonguo1118.cn

Py:   now + timedelta(days=7)
来源：https://rk.zhonguo4118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://it.zhonguo6118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://kd.zhonguo5118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://sv.zhonguo6118.cn

Java: LocalDate.now().plusDays(7)
来源：https://cy.zhonguo4118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://jp.zhonguo2118.cn

Ruby: Time.now + 7 * 86400
来源：https://lg.zhonguo7118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://yi.zhonguo7118.cn

[J06] 计算两时间之差
来源：https://ml.zhonguo4118.cn

Py:   (end - start).total_seconds()
来源：https://xs.zhonguo1118.cn

PHP:  $end->diff($start)->days;
来源：https://bw.zhonguo7118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://jz.zhonguo1118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://oe.zhonguo2118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://nc.zhonguo7118.cn

Go:   end.Sub(start).Hours()
来源：https://pk.zhonguo7118.cn

Ruby: end - start                 # 返回秒数
来源：https://hc.zhonguo3118.cn

C#:   (end - start).TotalSeconds
来源：https://bi.zhonguo4118.cn

[J07] 比较两个日期
来源：https://yl.zhonguo2118.cn

Py:   d1 < d2;  d1 == d2
来源：https://ab.zhonguo2118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://mv.zhonguo1118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://os.zhonguo2118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://uk.zhonguo2118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://zz.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://so.zhonguo3118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://tt.zhonguo8118.cn

C#:   d1 < d2;  d1 == d2
来源：https://ad.zhonguo6118.cn

[J08] 提取年月日与星期
来源：https://jm.zhonguo5118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://ag.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://mf.zhonguo4118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://bw.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://hi.zhonguo7118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://pg.zhonguo8118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://vp.zhonguo5118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://yx.zhonguo3118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ty.zhonguo2118.cn

[J09] 时区处理
来源：https://wb.zhonguo5118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://zw.zhonguo6118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://jv.zhonguo2118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://sg.zhonguo2118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://xd.zhonguo5118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://vg.zhonguo2118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://lc.zhonguo3118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://lx.zhonguo7118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://vq.zhonguo7118.cn

[J10] 取今天 / 本月第一天
来源：https://xf.zhonguo4118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://im.zhonguo6118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://up.zhonguo3118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://hx.zhonguo3118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://dh.zhonguo2118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://yg.zhonguo2118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://lp.zhonguo5118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://hz.zhonguo1118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://mi.zhonguo3118.cn

================================================================================
来源：https://jh.zhonguo1118.cn

K. JSON 与序列化
来源：https://co.zhonguo1118.cn

================================================================================
来源：https://st.zhonguo4118.cn

[K01] 对象转 JSON 字符串
来源：https://tr.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://qg.zhonguo5118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://fu.zhonguo8118.cn

JS:   JSON.stringify(obj)
来源：https://mx.zhonguo1118.cn

TS:   JSON.stringify(obj)
来源：https://jt.zhonguo8118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ys.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://pg.zhonguo4118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://jv.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://nc.zhonguo8118.cn

[K02] JSON 字符串转对象
来源：https://ye.zhonguo5118.cn

Py:   json.loads(s)
来源：https://or.zhonguo4118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://qk.zhonguo3118.cn

JS:   JSON.parse(s)
来源：https://lb.zhonguo5118.cn

TS:   JSON.parse(s)
来源：https://ur.zhonguo1118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://tj.zhonguo1118.cn

Go:   json.Unmarshal(data, &v)
来源：https://uo.zhonguo1118.cn

Ruby: JSON.parse(s)
来源：https://wm.zhonguo1118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://gr.zhonguo3118.cn

[K03] JSON 美化输出（带缩进）
来源：https://hf.zhonguo1118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://kr.zhonguo6118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://pm.zhonguo7118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://gh.zhonguo2118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://pv.zhonguo2118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://di.zhonguo6118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://rf.zhonguo8118.cn


<!-- 参考信息 -->