代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：https://wb.zhonguo8118.cn

Ruby: rescue ArgumentError => e
来源：https://qx.zhonguo5118.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：https://cx.zhonguo2118.cn

[H06] 可选值 / 空值安全访问
来源：https://vm.zhonguo8118.cn

Py:   value = d.get("k") or default
来源：https://er.zhonguo6118.cn

PHP:  $v = $d["k"] ?? null;
来源：https://rr.zhonguo8118.cn

JS:   obj?.a?.b;  d ?? default
来源：https://mo.zhonguo6118.cn

TS:   obj?.a?.b;  d ?? default
来源：https://ai.zhonguo8118.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：https://ue.zhonguo4118.cn

Go:   if v, ok := m["k"]; ok { }
来源：https://rz.zhonguo2118.cn

Ruby: d&.dig(:a, :b)
来源：https://bm.zhonguo7118.cn

C#:   obj?.A?.B ?? default
来源：https://bt.zhonguo2118.cn

[H07] 断言
来源：https://wb.zhonguo6118.cn

Py:   assert x > 0, "必须为正"
来源：https://xz.zhonguo4118.cn

PHP:  assert($x > 0);
来源：https://wb.zhonguo8118.cn

JS:   console.assert(x > 0);
来源：https://fq.zhonguo4118.cn

TS:   console.assert(x > 0);
来源：https://wd.zhonguo7118.cn

Java: assert x > 0 : "必须为正";
来源：https://oj.zhonguo1118.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：https://gk.zhonguo8118.cn

Ruby: raise "必须为正" unless x > 0
来源：https://vq.zhonguo3118.cn

C#:   Debug.Assert(x > 0);
来源：https://cl.zhonguo1118.cn

[H08] 获取错误信息与堆栈
来源：https://of.zhonguo6118.cn

Py:   str(e);  traceback.format_exc()
来源：https://lt.zhonguo3118.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：https://op.zhonguo1118.cn

JS:   e.message;  e.stack
来源：https://bk.zhonguo8118.cn

TS:   e instanceof Error ? e.message : String(e)
来源：https://ly.zhonguo1118.cn

Java: e.getMessage();  e.printStackTrace()
来源：https://sm.zhonguo3118.cn

Go:   err.Error()
来源：https://sm.zhonguo1118.cn

Ruby: e.message;  e.backtrace
来源：https://vb.zhonguo4118.cn

C#:   e.Message;  e.StackTrace
来源：https://tf.zhonguo5118.cn

[H09] 带错误码的异常
来源：https://at.zhonguo5118.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：https://ov.zhonguo4118.cn

PHP:  throw new RuntimeException("fail", 500);
来源：https://zb.zhonguo6118.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：https://cv.zhonguo7118.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：https://is.zhonguo5118.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：https://ek.zhonguo3118.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：https://hm.zhonguo8118.cn

Ruby: raise MyError.new("fail", 500)
来源：https://zh.zhonguo7118.cn

C#:   // 自定义异常类中加 Code 属性
来源：https://jy.zhonguo2118.cn

[H10] 资源自动释放
来源：https://rj.zhonguo5118.cn

Py:   with open("a.txt") as f: data = f.read()
来源：https://ij.zhonguo6118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://yc.zhonguo7118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://ul.zhonguo5118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://uc.zhonguo7118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://hi.zhonguo4118.cn

Go:   defer f.Close()
来源：https://db.zhonguo2118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://hq.zhonguo1118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://kq.zhonguo4118.cn

================================================================================
来源：https://qm.zhonguo3118.cn

I. 正则表达式
来源：https://eo.zhonguo6118.cn

================================================================================
来源：https://vq.zhonguo1118.cn

[I01] 判断是否匹配
来源：https://mk.zhonguo2118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://zt.zhonguo7118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://qm.zhonguo3118.cn

JS:   /\d+/.test(s)
来源：https://jj.zhonguo7118.cn

TS:   /\d+/.test(s)
来源：https://bj.zhonguo3118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://bm.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://gh.zhonguo3118.cn

Ruby: s.match?(/\d+/)
来源：https://un.zhonguo2118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://vi.zhonguo4118.cn

[I02] 提取所有匹配
来源：https://bb.zhonguo8118.cn

Py:   re.findall(r"\d+", s)
来源：https://ez.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ro.zhonguo8118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://aq.zhonguo1118.cn

TS:   s.match(/\d+/g)
来源：https://nf.zhonguo6118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://kf.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://et.zhonguo3118.cn

Ruby: s.scan(/\d+/)
来源：https://or.zhonguo6118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://xc.zhonguo1118.cn

[I03] 提取捕获分组
来源：https://kk.zhonguo1118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://rv.zhonguo6118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://uj.zhonguo1118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://hb.zhonguo6118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://mi.zhonguo6118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://vh.zhonguo7118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://oc.zhonguo3118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://wf.zhonguo5118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://ye.zhonguo4118.cn

[I04] 正则替换
来源：https://rp.zhonguo2118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://gq.zhonguo7118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://fs.zhonguo7118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://sv.zhonguo1118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://wy.zhonguo5118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://vc.zhonguo4118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://qu.zhonguo6118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://yc.zhonguo5118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://by.zhonguo3118.cn

[I05] 按正则拆分
来源：https://bk.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://an.zhonguo2118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://mx.zhonguo7118.cn

JS:   s.split(/\s*,\s*/)
来源：https://eh.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://by.zhonguo7118.cn

Java: s.split("\\s*,\\s*")
来源：https://lx.zhonguo2118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://nv.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://jb.zhonguo6118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://wc.zhonguo5118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://dz.zhonguo4118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://ip.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://wh.zhonguo7118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://uz.zhonguo1118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://as.zhonguo1118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://my.zhonguo5118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://hd.zhonguo7118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://jv.zhonguo4118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://uz.zhonguo4118.cn

[I07] 忽略大小写与多行模式
来源：https://mb.zhonguo1118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://zd.zhonguo7118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://lm.zhonguo5118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://gn.zhonguo1118.cn

TS:   /error/gim
来源：https://hf.zhonguo7118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://if.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://hq.zhonguo4118.cn

Ruby: s.scan(/error/i)
来源：https://fd.zhonguo2118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://mo.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://qg.zhonguo4118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://kx.zhonguo4118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://zq.zhonguo8118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://eo.zhonguo3118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://kt.zhonguo1118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://bu.zhonguo5118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://lj.zhonguo7118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://nf.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://ks.zhonguo4118.cn

================================================================================
来源：https://ps.zhonguo5118.cn

J. 日期与时间
来源：https://cq.zhonguo2118.cn

================================================================================
来源：https://bd.zhonguo7118.cn

[J01] 获取当前时间
来源：https://rq.zhonguo3118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://dt.zhonguo2118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://sj.zhonguo5118.cn

JS:   new Date();  Date.now()
来源：https://ru.zhonguo1118.cn

TS:   new Date();  Date.now()
来源：https://rm.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://zl.zhonguo7118.cn

Go:   time.Now()
来源：https://oy.zhonguo3118.cn

Ruby: Time.now
来源：https://pf.zhonguo3118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://tk.zhonguo8118.cn

[J02] 格式化输出
来源：https://ec.zhonguo5118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://rk.zhonguo8118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://dc.zhonguo1118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://cs.zhonguo4118.cn

TS:   d.toISOString()
来源：https://hq.zhonguo4118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://xe.zhonguo4118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://pr.zhonguo1118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://cv.zhonguo1118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://eq.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://ky.zhonguo6118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://qw.zhonguo1118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://dd.zhonguo8118.cn

JS:   new Date("2024-01-02")
来源：https://ih.zhonguo4118.cn

TS:   new Date("2024-01-02")
来源：https://jz.zhonguo5118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://jw.zhonguo8118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://qn.zhonguo3118.cn

Ruby: Date.parse("2024-01-02")
来源：https://wm.zhonguo8118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://ok.zhonguo3118.cn

[J04] 时间戳与日期互转
来源：https://np.zhonguo7118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://gh.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://kb.zhonguo7118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://ju.zhonguo7118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://uz.zhonguo8118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://fc.zhonguo7118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://qu.zhonguo1118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://gy.zhonguo5118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ui.zhonguo1118.cn

[J05] 时间加减（加 7 天）
来源：https://ck.zhonguo3118.cn

Py:   now + timedelta(days=7)
来源：https://ab.zhonguo6118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://tj.zhonguo5118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://nt.zhonguo2118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://bn.zhonguo6118.cn

Java: LocalDate.now().plusDays(7)
来源：https://mp.zhonguo2118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://xi.zhonguo4118.cn

Ruby: Time.now + 7 * 86400
来源：https://cf.zhonguo5118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://nc.zhonguo6118.cn

[J06] 计算两时间之差
来源：https://pl.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://nh.zhonguo5118.cn

PHP:  $end->diff($start)->days;
来源：https://tv.zhonguo1118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://kj.zhonguo1118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://gz.zhonguo4118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://wd.zhonguo1118.cn

Go:   end.Sub(start).Hours()
来源：https://mb.zhonguo8118.cn

Ruby: end - start                 # 返回秒数
来源：https://il.zhonguo5118.cn

C#:   (end - start).TotalSeconds
来源：https://mw.zhonguo4118.cn

[J07] 比较两个日期
来源：https://ln.zhonguo3118.cn

Py:   d1 < d2;  d1 == d2
来源：https://gg.zhonguo3118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://tr.zhonguo7118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://ea.zhonguo5118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://aw.zhonguo2118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://db.zhonguo3118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://uh.zhonguo2118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://vp.zhonguo1118.cn

C#:   d1 < d2;  d1 == d2
来源：https://te.zhonguo1118.cn

[J08] 提取年月日与星期
来源：https://wd.zhonguo4118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://pu.zhonguo5118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://qc.zhonguo3118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://nx.zhonguo6118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://qn.zhonguo8118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://dv.zhonguo3118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://fb.zhonguo7118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ba.zhonguo3118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://ux.zhonguo1118.cn

[J09] 时区处理
来源：https://et.zhonguo7118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://dy.zhonguo1118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://nj.zhonguo5118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://lr.zhonguo3118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ft.zhonguo8118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://uk.zhonguo7118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://nu.zhonguo7118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://og.zhonguo8118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://jb.zhonguo1118.cn

[J10] 取今天 / 本月第一天
来源：https://eo.zhonguo5118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://df.zhonguo8118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://bg.zhonguo2118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://hi.zhonguo7118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://tb.zhonguo1118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://ks.zhonguo2118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://pr.zhonguo4118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://rm.zhonguo8118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://bi.zhonguo6118.cn

================================================================================
来源：https://ho.zhonguo2118.cn

K. JSON 与序列化
来源：https://yq.zhonguo3118.cn

================================================================================
来源：https://rn.zhonguo8118.cn

[K01] 对象转 JSON 字符串
来源：https://pc.zhonguo4118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://bf.zhonguo4118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://kz.zhonguo1118.cn

JS:   JSON.stringify(obj)
来源：https://as.zhonguo1118.cn

TS:   JSON.stringify(obj)
来源：https://fz.zhonguo7118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ik.zhonguo5118.cn

Go:   json.Marshal(obj)
来源：https://iy.zhonguo1118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://ar.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://zr.zhonguo8118.cn

[K02] JSON 字符串转对象
来源：https://hw.zhonguo5118.cn

Py:   json.loads(s)
来源：https://hy.zhonguo8118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://af.zhonguo5118.cn

JS:   JSON.parse(s)
来源：https://cu.zhonguo7118.cn

TS:   JSON.parse(s)
来源：https://fe.zhonguo8118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://fm.zhonguo2118.cn

Go:   json.Unmarshal(data, &v)
来源：https://uc.zhonguo4118.cn

Ruby: JSON.parse(s)
来源：https://mz.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://vc.zhonguo4118.cn

[K03] JSON 美化输出（带缩进）
来源：https://ub.zhonguo5118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://pf.zhonguo8118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://en.zhonguo8118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://xc.zhonguo4118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://ah.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://ju.zhonguo8118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://oe.zhonguo1118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://at.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://zk.zhonguo5118.cn

[K04] 读取 JSON 文件
来源：https://pq.zhonguo1118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://mt.zhonguo7118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://ma.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://vv.zhonguo1118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://bt.zhonguo8118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://bm.zhonguo7118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://ge.zhonguo7118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://dd.zhonguo2118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://kf.zhonguo6118.cn

[K05] 深拷贝对象
来源：https://bn.zhonguo7118.cn

Py:   copy.deepcopy(obj)
来源：https://ed.zhonguo8118.cn

PHP:  unserialize(serialize($obj));
来源：https://mp.zhonguo8118.cn

JS:   structuredClone(obj)
来源：https://jc.zhonguo4118.cn

TS:   structuredClone(obj)
来源：https://cm.zhonguo5118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://lg.zhonguo5118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://hq.zhonguo1118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://ks.zhonguo2118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ec.zhonguo7118.cn

[K06] 解析 URL 查询串
来源：https://ly.zhonguo7118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://yl.zhonguo8118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://gp.zhonguo7118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://dx.zhonguo6118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://bp.zhonguo5118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://yc.zhonguo5118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://ij.zhonguo3118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://xg.zhonguo4118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://we.zhonguo4118.cn

[K07] 进制转换
来源：https://bo.zhonguo5118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://aj.zhonguo4118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://zv.zhonguo4118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://mn.zhonguo4118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://vy.zhonguo8118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://nk.zhonguo2118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ux.zhonguo2118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://ah.zhonguo3118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://gf.zhonguo3118.cn

[K08] 二进制序列化（非 JSON）
来源：https://kd.zhonguo5118.cn

Py:   pickle.dumps(obj)
来源：https://xc.zhonguo2118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://cl.zhonguo4118.cn

JS:   v8.serialize(obj)        // Node
来源：https://vz.zhonguo7118.cn

TS:   v8.serialize(obj)        // Node
来源：https://gb.zhonguo4118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://zw.zhonguo4118.cn

Go:   encoding/gob
来源：https://da.zhonguo8118.cn

Ruby: Marshal.dump(obj)
来源：https://kr.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://nd.zhonguo1118.cn

================================================================================
来源：https://dw.zhonguo6118.cn

L. 网络请求
来源：https://xw.zhonguo5118.cn

================================================================================
来源：https://pz.zhonguo3118.cn

[L01] 发送 GET 请求
来源：https://lc.zhonguo1118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://lr.zhonguo3118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://sd.zhonguo4118.cn

JS:   await fetch(url)
来源：https://ii.zhonguo1118.cn

TS:   await fetch(url)
来源：https://ac.zhonguo7118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://yh.zhonguo7118.cn


<!-- 参考信息 -->