代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：https://kl.zhonguo1118.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：https://ey.zhonguo8118.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：https://df.zhonguo5118.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：https://ea.zhonguo1118.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：https://zd.zhonguo3118.cn

Go:   defer f.Close()
来源：https://dk.zhonguo8118.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：https://za.zhonguo2118.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：https://gt.zhonguo4118.cn

================================================================================
来源：https://qr.zhonguo7118.cn

I. 正则表达式
来源：https://bi.zhonguo7118.cn

================================================================================
来源：https://gt.zhonguo4118.cn

[I01] 判断是否匹配
来源：https://tl.zhonguo6118.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：https://en.zhonguo4118.cn

PHP:  preg_match('/\d+/', $s);
来源：https://hw.zhonguo2118.cn

JS:   /\d+/.test(s)
来源：https://nc.zhonguo5118.cn

TS:   /\d+/.test(s)
来源：https://oi.zhonguo1118.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://ni.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://wm.zhonguo1118.cn

Ruby: s.match?(/\d+/)
来源：https://vw.zhonguo5118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://on.zhonguo7118.cn

[I02] 提取所有匹配
来源：https://bn.zhonguo1118.cn

Py:   re.findall(r"\d+", s)
来源：https://np.zhonguo6118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://at.zhonguo7118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://nz.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://mo.zhonguo2118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://av.zhonguo8118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://dr.zhonguo1118.cn

Ruby: s.scan(/\d+/)
来源：https://cq.zhonguo1118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://kq.zhonguo6118.cn

[I03] 提取捕获分组
来源：https://wz.zhonguo4118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://mh.zhonguo7118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://ym.zhonguo7118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://ul.zhonguo3118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://uv.zhonguo5118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://rc.zhonguo8118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://po.zhonguo6118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://tq.zhonguo2118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://uh.zhonguo5118.cn

[I04] 正则替换
来源：https://if.zhonguo7118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://tu.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://fb.zhonguo5118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://tb.zhonguo2118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://mk.zhonguo2118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://rq.zhonguo6118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://yx.zhonguo5118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://zf.zhonguo6118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://nr.zhonguo5118.cn

[I05] 按正则拆分
来源：https://gi.zhonguo1118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://uy.zhonguo3118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://xj.zhonguo7118.cn

JS:   s.split(/\s*,\s*/)
来源：https://xj.zhonguo1118.cn

TS:   s.split(/\s*,\s*/)
来源：https://ut.zhonguo2118.cn

Java: s.split("\\s*,\\s*")
来源：https://lo.zhonguo8118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://rz.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://pb.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://dw.zhonguo6118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://aq.zhonguo1118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://im.zhonguo3118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://iz.zhonguo2118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://zu.zhonguo8118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://gq.zhonguo5118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://ql.zhonguo8118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://ep.zhonguo8118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://wt.zhonguo7118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://de.zhonguo5118.cn

[I07] 忽略大小写与多行模式
来源：https://tx.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://sw.zhonguo5118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://ar.zhonguo8118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://kd.zhonguo6118.cn

TS:   /error/gim
来源：https://jm.zhonguo8118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://ed.zhonguo8118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vd.zhonguo3118.cn

Ruby: s.scan(/error/i)
来源：https://pk.zhonguo3118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://bv.zhonguo6118.cn

[I08] 贪婪与非贪婪匹配
来源：https://bw.zhonguo2118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://bk.zhonguo8118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://lh.zhonguo6118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://xb.zhonguo1118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://pw.zhonguo1118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://sh.zhonguo6118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://wn.zhonguo1118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://xe.zhonguo4118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://wt.zhonguo1118.cn

================================================================================
来源：https://tk.zhonguo1118.cn

J. 日期与时间
来源：https://ps.zhonguo1118.cn

================================================================================
来源：https://yr.zhonguo7118.cn

[J01] 获取当前时间
来源：https://mk.zhonguo5118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://qm.zhonguo6118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://ti.zhonguo1118.cn

JS:   new Date();  Date.now()
来源：https://xr.zhonguo1118.cn

TS:   new Date();  Date.now()
来源：https://yw.zhonguo7118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://ac.zhonguo5118.cn

Go:   time.Now()
来源：https://vw.zhonguo5118.cn

Ruby: Time.now
来源：https://ig.zhonguo3118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://ii.zhonguo3118.cn

[J02] 格式化输出
来源：https://xy.zhonguo8118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://id.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://kj.zhonguo5118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://zz.zhonguo4118.cn

TS:   d.toISOString()
来源：https://wu.zhonguo7118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://pe.zhonguo3118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://ho.zhonguo1118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://nk.zhonguo2118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://hd.zhonguo4118.cn

[J03] 字符串解析为日期
来源：https://dk.zhonguo1118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://vd.zhonguo5118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://ue.zhonguo3118.cn

JS:   new Date("2024-01-02")
来源：https://db.zhonguo4118.cn

TS:   new Date("2024-01-02")
来源：https://ka.zhonguo3118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://gd.zhonguo2118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://jl.zhonguo6118.cn

Ruby: Date.parse("2024-01-02")
来源：https://dm.zhonguo1118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://gh.zhonguo1118.cn

[J04] 时间戳与日期互转
来源：https://du.zhonguo6118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://pz.zhonguo3118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://yi.zhonguo1118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://kr.zhonguo2118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://we.zhonguo6118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://bf.zhonguo2118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://ne.zhonguo2118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://tm.zhonguo6118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://ud.zhonguo3118.cn

[J05] 时间加减（加 7 天）
来源：https://rw.zhonguo2118.cn

Py:   now + timedelta(days=7)
来源：https://fq.zhonguo1118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://wn.zhonguo8118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://lp.zhonguo1118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://tf.zhonguo5118.cn

Java: LocalDate.now().plusDays(7)
来源：https://aj.zhonguo3118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://iq.zhonguo5118.cn

Ruby: Time.now + 7 * 86400
来源：https://gj.zhonguo6118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://pq.zhonguo8118.cn

[J06] 计算两时间之差
来源：https://er.zhonguo3118.cn

Py:   (end - start).total_seconds()
来源：https://zm.zhonguo6118.cn

PHP:  $end->diff($start)->days;
来源：https://zi.zhonguo1118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://di.zhonguo6118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://bx.zhonguo5118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://dl.zhonguo3118.cn

Go:   end.Sub(start).Hours()
来源：https://ac.zhonguo1118.cn

Ruby: end - start                 # 返回秒数
来源：https://mf.zhonguo8118.cn

C#:   (end - start).TotalSeconds
来源：https://my.zhonguo2118.cn

[J07] 比较两个日期
来源：https://ws.zhonguo7118.cn

Py:   d1 < d2;  d1 == d2
来源：https://di.zhonguo1118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://vi.zhonguo8118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://wy.zhonguo3118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://qi.zhonguo5118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://io.zhonguo5118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://nt.zhonguo6118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://lf.zhonguo7118.cn

C#:   d1 < d2;  d1 == d2
来源：https://pl.zhonguo3118.cn

[J08] 提取年月日与星期
来源：https://sm.zhonguo7118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://rw.zhonguo7118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://ug.zhonguo1118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://xz.zhonguo4118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://mi.zhonguo3118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://kz.zhonguo4118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://iw.zhonguo6118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ab.zhonguo5118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://nk.zhonguo4118.cn

[J09] 时区处理
来源：https://mb.zhonguo2118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://op.zhonguo7118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://gn.zhonguo2118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://cr.zhonguo4118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://sn.zhonguo3118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://ce.zhonguo5118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://ol.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://jq.zhonguo6118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://qu.zhonguo8118.cn

[J10] 取今天 / 本月第一天
来源：https://tv.zhonguo2118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ki.zhonguo6118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://li.zhonguo8118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://hy.zhonguo6118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://xk.zhonguo3118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://cf.zhonguo7118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://wm.zhonguo7118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://ap.zhonguo6118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://nu.zhonguo2118.cn

================================================================================
来源：https://ag.zhonguo7118.cn

K. JSON 与序列化
来源：https://wd.zhonguo5118.cn

================================================================================
来源：https://wt.zhonguo5118.cn

[K01] 对象转 JSON 字符串
来源：https://bt.zhonguo2118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://hn.zhonguo5118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://ej.zhonguo7118.cn

JS:   JSON.stringify(obj)
来源：https://ym.zhonguo1118.cn

TS:   JSON.stringify(obj)
来源：https://rf.zhonguo1118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://cn.zhonguo2118.cn

Go:   json.Marshal(obj)
来源：https://gq.zhonguo4118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://vr.zhonguo7118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://as.zhonguo1118.cn

[K02] JSON 字符串转对象
来源：https://lb.zhonguo6118.cn

Py:   json.loads(s)
来源：https://ly.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://fe.zhonguo2118.cn

JS:   JSON.parse(s)
来源：https://zz.zhonguo6118.cn

TS:   JSON.parse(s)
来源：https://uv.zhonguo1118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://hf.zhonguo6118.cn

Go:   json.Unmarshal(data, &v)
来源：https://uu.zhonguo3118.cn

Ruby: JSON.parse(s)
来源：https://bv.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://br.zhonguo7118.cn

[K03] JSON 美化输出（带缩进）
来源：https://ss.zhonguo4118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://ti.zhonguo1118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://xn.zhonguo4118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://sg.zhonguo6118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://xz.zhonguo6118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://tw.zhonguo1118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://fc.zhonguo3118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://bi.zhonguo2118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://vh.zhonguo8118.cn

[K04] 读取 JSON 文件
来源：https://yc.zhonguo4118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://hc.zhonguo6118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://hg.zhonguo5118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://qx.zhonguo2118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://iv.zhonguo8118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://yv.zhonguo1118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://tn.zhonguo2118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://mn.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://nc.zhonguo6118.cn

[K05] 深拷贝对象
来源：https://zx.zhonguo8118.cn

Py:   copy.deepcopy(obj)
来源：https://yf.zhonguo6118.cn

PHP:  unserialize(serialize($obj));
来源：https://xm.zhonguo4118.cn

JS:   structuredClone(obj)
来源：https://jh.zhonguo3118.cn

TS:   structuredClone(obj)
来源：https://la.zhonguo6118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://di.zhonguo4118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://td.zhonguo8118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://pl.zhonguo2118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://ng.zhonguo8118.cn

[K06] 解析 URL 查询串
来源：https://oy.zhonguo3118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://ws.zhonguo4118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://yl.zhonguo8118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://po.zhonguo6118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://bh.zhonguo4118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://to.zhonguo8118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://dr.zhonguo4118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://ik.zhonguo6118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://cc.zhonguo3118.cn

[K07] 进制转换
来源：https://ix.zhonguo5118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://sc.zhonguo3118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://wg.zhonguo1118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://zt.zhonguo4118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://po.zhonguo7118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://td.zhonguo6118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://ko.zhonguo7118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://vr.zhonguo6118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://or.zhonguo8118.cn

[K08] 二进制序列化（非 JSON）
来源：https://ry.zhonguo1118.cn

Py:   pickle.dumps(obj)
来源：https://od.zhonguo3118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://oh.zhonguo6118.cn

JS:   v8.serialize(obj)        // Node
来源：https://xp.zhonguo6118.cn

TS:   v8.serialize(obj)        // Node
来源：https://bh.zhonguo7118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://jo.zhonguo3118.cn

Go:   encoding/gob
来源：https://se.zhonguo1118.cn

Ruby: Marshal.dump(obj)
来源：https://tr.zhonguo2118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://eq.zhonguo7118.cn

================================================================================
来源：https://aw.zhonguo3118.cn

L. 网络请求
来源：https://kr.zhonguo2118.cn

================================================================================
来源：https://tm.zhonguo2118.cn

[L01] 发送 GET 请求
来源：https://vl.zhonguo7118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://jc.zhonguo4118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://pz.zhonguo8118.cn

JS:   await fetch(url)
来源：https://vc.zhonguo2118.cn

TS:   await fetch(url)
来源：https://fy.zhonguo2118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://nv.zhonguo2118.cn

Go:   resp, err := http.Get(url)
来源：https://jf.zhonguo2118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://rn.zhonguo8118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://cp.zhonguo7118.cn

[L02] 发送 POST JSON
来源：https://vn.zhonguo6118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://rr.zhonguo1118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://xm.zhonguo2118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://hb.zhonguo2118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://pg.zhonguo5118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://gq.zhonguo1118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://cy.zhonguo6118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://lu.zhonguo1118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://hx.zhonguo3118.cn

[L03] 设置自定义请求头
来源：https://pz.zhonguo4118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://yd.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://xr.zhonguo7118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://bc.zhonguo8118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://xc.zhonguo4118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://yv.zhonguo1118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://ry.zhonguo6118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://kn.zhonguo2118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://im.zhonguo3118.cn

[L04] 设置超时
来源：https://hr.zhonguo6118.cn

Py:   requests.get(url, timeout=5)
来源：https://kb.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://kx.zhonguo6118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://ro.zhonguo5118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://mz.zhonguo4118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://sj.zhonguo1118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://xb.zhonguo5118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://ah.zhonguo8118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://tq.zhonguo6118.cn

[L05] 上传文件（multipart）
来源：https://sn.zhonguo1118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://da.zhonguo5118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://mx.zhonguo2118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://tr.zhonguo2118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://mi.zhonguo6118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://ou.zhonguo7118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://tf.zhonguo7118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://ts.zhonguo4118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://mb.zhonguo7118.cn

[L06] 解析响应为 JSON
来源：https://is.zhonguo6118.cn


<!-- 参考信息 -->