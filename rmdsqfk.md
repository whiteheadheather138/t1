代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：https://pp.zhonguo6118.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：https://hx.zhonguo4118.cn

Ruby: s.match?(/\d+/)
来源：https://kf.zhonguo2118.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：https://by.zhonguo5118.cn

[I02] 提取所有匹配
来源：https://gj.zhonguo7118.cn

Py:   re.findall(r"\d+", s)
来源：https://og.zhonguo4118.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：https://ve.zhonguo2118.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：https://oe.zhonguo3118.cn

TS:   s.match(/\d+/g)
来源：https://rf.zhonguo1118.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：https://nk.zhonguo5118.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：https://ie.zhonguo5118.cn

Ruby: s.scan(/\d+/)
来源：https://yk.zhonguo2118.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：https://xw.zhonguo5118.cn

[I03] 提取捕获分组
来源：https://io.zhonguo7118.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：https://ik.zhonguo5118.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：https://xs.zhonguo6118.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：https://wm.zhonguo5118.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：https://td.zhonguo4118.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：https://ge.zhonguo1118.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：https://hq.zhonguo2118.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：https://ym.zhonguo6118.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：https://sk.zhonguo7118.cn

[I04] 正则替换
来源：https://ub.zhonguo7118.cn

Py:   re.sub(r"\d+", "#", s)
来源：https://bo.zhonguo4118.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：https://wu.zhonguo6118.cn

JS:   s.replace(/\d+/g, "#")
来源：https://rj.zhonguo6118.cn

TS:   s.replace(/\d+/g, "#")
来源：https://lp.zhonguo3118.cn

Java: s.replaceAll("\\d+", "#")
来源：https://vy.zhonguo5118.cn

Go:   re.ReplaceAllString(s, "#")
来源：https://fh.zhonguo2118.cn

Ruby: s.gsub(/\d+/, "#")
来源：https://kl.zhonguo5118.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：https://fb.zhonguo1118.cn

[I05] 按正则拆分
来源：https://eh.zhonguo6118.cn

Py:   re.split(r"\s*,\s*", s)
来源：https://pz.zhonguo8118.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：https://hj.zhonguo4118.cn

JS:   s.split(/\s*,\s*/)
来源：https://ff.zhonguo4118.cn

TS:   s.split(/\s*,\s*/)
来源：https://nw.zhonguo7118.cn

Java: s.split("\\s*,\\s*")
来源：https://hu.zhonguo7118.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：https://zu.zhonguo6118.cn

Ruby: s.split(/\s*,\s*/)
来源：https://qk.zhonguo1118.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：https://fv.zhonguo3118.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：https://hs.zhonguo8118.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：https://sg.zhonguo1118.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：https://xs.zhonguo3118.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://hy.zhonguo2118.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：https://aa.zhonguo8118.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：https://nl.zhonguo5118.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：https://rd.zhonguo2118.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：https://xm.zhonguo6118.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：https://ul.zhonguo3118.cn

[I07] 忽略大小写与多行模式
来源：https://wf.zhonguo5118.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：https://qw.zhonguo4118.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：https://oy.zhonguo4118.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：https://sa.zhonguo3118.cn

TS:   /error/gim
来源：https://ar.zhonguo3118.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：https://je.zhonguo4118.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：https://vz.zhonguo7118.cn

Ruby: s.scan(/error/i)
来源：https://xx.zhonguo6118.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：https://ov.zhonguo1118.cn

[I08] 贪婪与非贪婪匹配
来源：https://we.zhonguo5118.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：https://fj.zhonguo7118.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：https://kk.zhonguo2118.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：https://gd.zhonguo8118.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：https://fn.zhonguo3118.cn

Java: Pattern.compile("<b>.*?</b>")
来源：https://qf.zhonguo3118.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：https://ph.zhonguo1118.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：https://fr.zhonguo3118.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：https://yz.zhonguo1118.cn

================================================================================
来源：https://rv.zhonguo8118.cn

J. 日期与时间
来源：https://sn.zhonguo2118.cn

================================================================================
来源：https://eg.zhonguo5118.cn

[J01] 获取当前时间
来源：https://gq.zhonguo7118.cn

Py:   datetime.now();  datetime.now(UTC)
来源：https://jw.zhonguo2118.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：https://nc.zhonguo6118.cn

JS:   new Date();  Date.now()
来源：https://wp.zhonguo5118.cn

TS:   new Date();  Date.now()
来源：https://ji.zhonguo5118.cn

Java: LocalDateTime.now();  Instant.now()
来源：https://yh.zhonguo3118.cn

Go:   time.Now()
来源：https://mb.zhonguo4118.cn

Ruby: Time.now
来源：https://nf.zhonguo7118.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：https://le.zhonguo1118.cn

[J02] 格式化输出
来源：https://ux.zhonguo8118.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://hf.zhonguo5118.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：https://nh.zhonguo2118.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：https://hb.zhonguo3118.cn

TS:   d.toISOString()
来源：https://qs.zhonguo6118.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：https://ei.zhonguo8118.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：https://dd.zhonguo3118.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：https://bc.zhonguo3118.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：https://nj.zhonguo6118.cn

[J03] 字符串解析为日期
来源：https://ue.zhonguo2118.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：https://xh.zhonguo6118.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：https://vu.zhonguo7118.cn

JS:   new Date("2024-01-02")
来源：https://cx.zhonguo2118.cn

TS:   new Date("2024-01-02")
来源：https://kt.zhonguo2118.cn

Java: LocalDate.parse("2024-01-02")
来源：https://ov.zhonguo3118.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：https://gz.zhonguo1118.cn

Ruby: Date.parse("2024-01-02")
来源：https://ru.zhonguo6118.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：https://iq.zhonguo1118.cn

[J04] 时间戳与日期互转
来源：https://fx.zhonguo7118.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：https://bm.zhonguo4118.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：https://cw.zhonguo3118.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：https://kj.zhonguo2118.cn

TS:   Math.floor(Date.now() / 1000)
来源：https://ep.zhonguo5118.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：https://cj.zhonguo6118.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：https://wj.zhonguo7118.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：https://tg.zhonguo5118.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：https://bm.zhonguo2118.cn

[J05] 时间加减（加 7 天）
来源：https://dv.zhonguo7118.cn

Py:   now + timedelta(days=7)
来源：https://lt.zhonguo2118.cn

PHP:  (new DateTime())->modify("+7 days");
来源：https://vu.zhonguo2118.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：https://ks.zhonguo2118.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：https://ye.zhonguo4118.cn

Java: LocalDate.now().plusDays(7)
来源：https://ay.zhonguo3118.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：https://fq.zhonguo4118.cn

Ruby: Time.now + 7 * 86400
来源：https://go.zhonguo4118.cn

C#:   DateTime.Now.AddDays(7)
来源：https://jc.zhonguo7118.cn

[J06] 计算两时间之差
来源：https://us.zhonguo7118.cn

Py:   (end - start).total_seconds()
来源：https://bl.zhonguo1118.cn

PHP:  $end->diff($start)->days;
来源：https://ya.zhonguo7118.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：https://rv.zhonguo7118.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：https://pp.zhonguo3118.cn

Java: Duration.between(start, end).toSeconds()
来源：https://xo.zhonguo6118.cn

Go:   end.Sub(start).Hours()
来源：https://hk.zhonguo4118.cn

Ruby: end - start                 # 返回秒数
来源：https://pi.zhonguo6118.cn

C#:   (end - start).TotalSeconds
来源：https://dk.zhonguo4118.cn

[J07] 比较两个日期
来源：https://yp.zhonguo4118.cn

Py:   d1 < d2;  d1 == d2
来源：https://ix.zhonguo4118.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：https://bc.zhonguo2118.cn

JS:   d1.getTime() < d2.getTime()
来源：https://pa.zhonguo7118.cn

TS:   d1.getTime() < d2.getTime()
来源：https://wo.zhonguo2118.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：https://or.zhonguo1118.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：https://vo.zhonguo2118.cn

Ruby: d1 < d2;  d1 == d2
来源：https://gh.zhonguo3118.cn

C#:   d1 < d2;  d1 == d2
来源：https://hq.zhonguo8118.cn

[J08] 提取年月日与星期
来源：https://xw.zhonguo7118.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：https://sf.zhonguo5118.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：https://vx.zhonguo2118.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：https://cv.zhonguo2118.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：https://kj.zhonguo7118.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：https://jf.zhonguo7118.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：https://op.zhonguo3118.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：https://ud.zhonguo2118.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：https://fv.zhonguo5118.cn

[J09] 时区处理
来源：https://tq.zhonguo4118.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：https://us.zhonguo8118.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：https://na.zhonguo4118.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://xm.zhonguo4118.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：https://ol.zhonguo2118.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：https://sv.zhonguo4118.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：https://rv.zhonguo2118.cn

Ruby: Time.now.getlocal("+08:00")
来源：https://ql.zhonguo4118.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：https://jb.zhonguo2118.cn

[J10] 取今天 / 本月第一天
来源：https://dv.zhonguo4118.cn

Py:   date.today();  date.today().replace(day=1)
来源：https://ot.zhonguo3118.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：https://je.zhonguo8118.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：https://lz.zhonguo4118.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：https://ei.zhonguo5118.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：https://qb.zhonguo5118.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：https://bz.zhonguo3118.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：https://gr.zhonguo1118.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：https://fm.zhonguo1118.cn

================================================================================
来源：https://ii.zhonguo6118.cn

K. JSON 与序列化
来源：https://aw.zhonguo6118.cn

================================================================================
来源：https://di.zhonguo3118.cn

[K01] 对象转 JSON 字符串
来源：https://ms.zhonguo2118.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：https://od.zhonguo7118.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：https://di.zhonguo8118.cn

JS:   JSON.stringify(obj)
来源：https://ph.zhonguo5118.cn

TS:   JSON.stringify(obj)
来源：https://uk.zhonguo6118.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：https://ca.zhonguo3118.cn

Go:   json.Marshal(obj)
来源：https://cb.zhonguo8118.cn

Ruby: obj.to_json                                     // require "json"
来源：https://yu.zhonguo4118.cn

C#:   JsonSerializer.Serialize(obj)
来源：https://bb.zhonguo8118.cn

[K02] JSON 字符串转对象
来源：https://sn.zhonguo5118.cn

Py:   json.loads(s)
来源：https://us.zhonguo6118.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：https://qg.zhonguo2118.cn

JS:   JSON.parse(s)
来源：https://in.zhonguo6118.cn

TS:   JSON.parse(s)
来源：https://wu.zhonguo7118.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：https://en.zhonguo1118.cn

Go:   json.Unmarshal(data, &v)
来源：https://li.zhonguo1118.cn

Ruby: JSON.parse(s)
来源：https://pj.zhonguo6118.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：https://sz.zhonguo5118.cn

[K03] JSON 美化输出（带缩进）
来源：https://qj.zhonguo1118.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：https://dr.zhonguo1118.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：https://rx.zhonguo6118.cn

JS:   JSON.stringify(obj, null, 2)
来源：https://pe.zhonguo8118.cn

TS:   JSON.stringify(obj, null, 2)
来源：https://yq.zhonguo7118.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：https://tw.zhonguo1118.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：https://zi.zhonguo1118.cn

Ruby: JSON.pretty_generate(obj)
来源：https://zh.zhonguo3118.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：https://wd.zhonguo7118.cn

[K04] 读取 JSON 文件
来源：https://vc.zhonguo5118.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：https://wj.zhonguo5118.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：https://ff.zhonguo3118.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://vq.zhonguo6118.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：https://ie.zhonguo1118.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：https://hq.zhonguo2118.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：https://du.zhonguo2118.cn

Ruby: JSON.parse(File.read("a.json"))
来源：https://bw.zhonguo8118.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：https://ap.zhonguo7118.cn

[K05] 深拷贝对象
来源：https://sb.zhonguo5118.cn

Py:   copy.deepcopy(obj)
来源：https://ea.zhonguo1118.cn

PHP:  unserialize(serialize($obj));
来源：https://ve.zhonguo7118.cn

JS:   structuredClone(obj)
来源：https://eb.zhonguo1118.cn

TS:   structuredClone(obj)
来源：https://ks.zhonguo1118.cn

Java: // 手写拷贝构造，或序列化往返
来源：https://na.zhonguo3118.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：https://sm.zhonguo2118.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：https://wm.zhonguo4118.cn

C#:   // 序列化往返，或自定义 Clone
来源：https://xv.zhonguo6118.cn

[K06] 解析 URL 查询串
来源：https://im.zhonguo2118.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：https://ie.zhonguo2118.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：https://se.zhonguo5118.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://oq.zhonguo4118.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：https://oc.zhonguo4118.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：https://gd.zhonguo2118.cn

Go:   url.ParseQuery("a=1&b=2")
来源：https://nz.zhonguo7118.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：https://tw.zhonguo6118.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：https://to.zhonguo3118.cn

[K07] 进制转换
来源：https://zo.zhonguo1118.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：https://jd.zhonguo8118.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：https://sz.zhonguo4118.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：https://zg.zhonguo8118.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：https://tk.zhonguo8118.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：https://yt.zhonguo5118.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：https://qc.zhonguo4118.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：https://aq.zhonguo8118.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：https://bu.zhonguo1118.cn

[K08] 二进制序列化（非 JSON）
来源：https://wg.zhonguo1118.cn

Py:   pickle.dumps(obj)
来源：https://jj.zhonguo4118.cn

PHP:  serialize($obj);  unserialize($s);
来源：https://jc.zhonguo2118.cn

JS:   v8.serialize(obj)        // Node
来源：https://je.zhonguo7118.cn

TS:   v8.serialize(obj)        // Node
来源：https://us.zhonguo7118.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：https://ov.zhonguo3118.cn

Go:   encoding/gob
来源：https://yp.zhonguo1118.cn

Ruby: Marshal.dump(obj)
来源：https://mc.zhonguo1118.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：https://gx.zhonguo8118.cn

================================================================================
来源：https://pd.zhonguo2118.cn

L. 网络请求
来源：https://yv.zhonguo7118.cn

================================================================================
来源：https://oz.zhonguo1118.cn

[L01] 发送 GET 请求
来源：https://ha.zhonguo6118.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：https://ue.zhonguo2118.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：https://cm.zhonguo2118.cn

JS:   await fetch(url)
来源：https://ws.zhonguo3118.cn

TS:   await fetch(url)
来源：https://zg.zhonguo7118.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：https://xs.zhonguo1118.cn

Go:   resp, err := http.Get(url)
来源：https://xw.zhonguo5118.cn

Ruby: Net::HTTP.get(URI(url))
来源：https://re.zhonguo2118.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：https://mq.zhonguo5118.cn

[L02] 发送 POST JSON
来源：https://fi.zhonguo6118.cn

Py:   requests.post(url, json={"a": 1})
来源：https://jf.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：https://nv.zhonguo7118.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://pd.zhonguo1118.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：https://om.zhonguo7118.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：https://fl.zhonguo2118.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：https://xg.zhonguo3118.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：https://zq.zhonguo3118.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：https://sa.zhonguo8118.cn

[L03] 设置自定义请求头
来源：https://nt.zhonguo4118.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：https://jk.zhonguo7118.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：https://dd.zhonguo2118.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://vd.zhonguo7118.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：https://hr.zhonguo3118.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：https://se.zhonguo8118.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：https://fd.zhonguo7118.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：https://ou.zhonguo1118.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：https://my.zhonguo5118.cn

[L04] 设置超时
来源：https://ik.zhonguo7118.cn

Py:   requests.get(url, timeout=5)
来源：https://mc.zhonguo3118.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：https://gz.zhonguo4118.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://pm.zhonguo7118.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：https://nk.zhonguo7118.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：https://jv.zhonguo7118.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：https://wf.zhonguo4118.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：https://mz.zhonguo4118.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：https://ff.zhonguo4118.cn

[L05] 上传文件（multipart）
来源：https://lg.zhonguo3118.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：https://es.zhonguo2118.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：https://ei.zhonguo4118.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：https://pd.zhonguo3118.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：https://ne.zhonguo3118.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：https://di.zhonguo2118.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：https://vw.zhonguo7118.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：https://xv.zhonguo8118.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：https://sh.zhonguo5118.cn

[L06] 解析响应为 JSON
来源：https://qt.zhonguo3118.cn

Py:   resp.json()
来源：https://gw.zhonguo2118.cn

PHP:  json_decode($body, true);
来源：https://tf.zhonguo7118.cn

JS:   await resp.json()
来源：https://wf.zhonguo6118.cn

TS:   await resp.json()
来源：https://bp.zhonguo3118.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：https://ez.zhonguo4118.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：https://yn.zhonguo7118.cn

Ruby: JSON.parse(resp.body)
来源：https://bn.zhonguo2118.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：https://su.zhonguo5118.cn

[L07] 处理 HTTP 状态码
来源：https://ss.zhonguo6118.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：https://qv.zhonguo6118.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：https://lq.zhonguo6118.cn

JS:   resp.ok;  resp.status
来源：https://rd.zhonguo4118.cn

TS:   resp.ok;  resp.status
来源：https://bq.zhonguo3118.cn

Java: resp.statusCode()
来源：https://dv.zhonguo5118.cn

Go:   resp.StatusCode
来源：https://wk.zhonguo8118.cn

Ruby: resp.code.to_i
来源：https://cf.zhonguo7118.cn


<!-- 参考信息 -->