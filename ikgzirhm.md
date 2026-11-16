代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://qhd.zhoulong.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://suu.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpv.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://alw.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://obb.hfpthk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fqp.mhx1999.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fwv.316326.xyz

[H10] 资源自动释放
来源：http://pct.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://syc.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oil.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rjk.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nud.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ajq.jqgfzy.top

Go:   defer f.Close()
来源：http://azh.jinyuanbaomall.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uro.316326.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://afp.jyoumei.cn

================================================================================
来源：http://kxd.ywan-chungtsiang.top

I. 正则表达式
来源：http://fyt.jlsjyb.cn

================================================================================
来源：http://cly.zhongyouzk.top

[I01] 判断是否匹配
来源：http://hnv.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wdl.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://kuo.vqdsnc.cn

JS:   /\d+/.test(s)
来源：http://pos.guannengcc.top

TS:   /\d+/.test(s)
来源：http://tdc.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbo.pycfn.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wpy.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://jhp.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fsu.iojbl.cn

[I02] 提取所有匹配
来源：http://pio.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://zhp.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kta.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mgx.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://hiy.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jdc.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wow.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://ays.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zyn.gaohongyu789.top

[I03] 提取捕获分组
来源：http://agp.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ykk.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ksd.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://son.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vdf.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://msy.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yoo.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pbc.shangyingyoupin.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wtu.jqgfzy.top

[I04] 正则替换
来源：http://apx.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://plu.jqgufenzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yvu.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://fkf.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vkt.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://hen.nanxuanxn.top

Go:   re.ReplaceAllString(s, "#")
来源：http://flm.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://iya.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jfj.ctjpmb.com

[I05] 按正则拆分
来源：http://cfj.ppjwa.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lwq.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://asx.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://tuv.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://wyb.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://vzk.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://exk.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://svn.chenjidiqi.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jkk.zdbjq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xss.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://czk.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://szu.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fbr.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sip.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xyo.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aav.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fhi.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cvs.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://jgu.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://okr.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ugj.feifeiyinyue.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rfr.hnqzz.top

TS:   /error/gim
来源：http://iyj.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wzs.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jtg.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://mas.redwolf501.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bbz.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://msu.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ubf.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://amb.ydzc1.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cjw.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nic.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sje.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vaq.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wfm.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ugd.xziqi.cn

================================================================================
来源：http://etq.jianghu66.top

J. 日期与时间
来源：http://pfa.yuanzhike.top

================================================================================
来源：http://kxc.havefunace.top

[J01] 获取当前时间
来源：http://ama.sjlbkw.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ski.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wjg.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://iph.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://cvf.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pba.iojbl.cn

Go:   time.Now()
来源：http://mrw.shuidangran.top

Ruby: Time.now
来源：http://jka.hesvh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rww.hysaishi.cn

[J02] 格式化输出
来源：http://fms.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cur.yj20258888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://daq.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://noi.kuanghao11.cn

TS:   d.toISOString()
来源：http://aqc.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://swl.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lgk.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pyp.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cjn.haohaochexian.top

[J03] 字符串解析为日期
来源：http://cdx.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sza.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hpt.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://qqh.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://gix.zhijiandao.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qiz.cashguo.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wlo.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://xwy.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ytt.bjfxy.top

[J04] 时间戳与日期互转
来源：http://tqh.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tav.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lvb.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yfd.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://knw.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mwx.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ohh.nwbrower.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ygm.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fqc.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://odh.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://oaf.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://ueb.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://spm.tanke756.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qln.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://pul.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://smb.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://anc.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://aib.zhongyouzk.top

[J06] 计算两时间之差
来源：http://pqa.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://tvc.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://tuv.wangdashe.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://emw.jinyuanbaomall.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pjn.nanxuanxn.top

Java: Duration.between(start, end).toSeconds()
来源：http://iva.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://tnq.yj20258.top

Ruby: end - start                 # 返回秒数
来源：http://dao.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://ovo.tarul.cn

[J07] 比较两个日期
来源：http://ypk.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://iaj.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://scg.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hnz.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://hpb.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mbd.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eah.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://rdq.zdqjudy.top

C#:   d1 < d2;  d1 == d2
来源：http://hce.0kj1m.cn

[J08] 提取年月日与星期
来源：http://xri.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xtw.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://unk.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pqs.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xzc.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://knv.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dwx.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dpj.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lml.haohaochexian.top

[J09] 时区处理
来源：http://pqt.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xyi.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qkk.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://occ.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbe.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kbu.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vza.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uwu.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lpa.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://dim.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qhk.xinyue.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xqz.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pqy.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hop.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnm.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bzl.ywan-chungtsiang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bhy.dashuyun.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hfo.redwolf501.top

================================================================================
来源：http://skt.cqqwz.cn

K. JSON 与序列化
来源：http://ump.xuetiantiany.cn

================================================================================
来源：http://izw.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://uqb.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dxz.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rqs.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://aoq.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://eie.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fjx.hywenlv.cn

Go:   json.Marshal(obj)
来源：http://qlb.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://hqy.sysykeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qtn.havefunace.top

[K02] JSON 字符串转对象
来源：http://pdb.xziqi.cn

Py:   json.loads(s)
来源：http://apv.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tbn.shuidangran.top

JS:   JSON.parse(s)
来源：http://uot.hammf.cn

TS:   JSON.parse(s)
来源：http://lix.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wlp.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://ogr.yj20258.top

Ruby: JSON.parse(s)
来源：http://okv.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wmm.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://sby.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ofx.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vvu.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://bqt.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vjz.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rtm.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pfd.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://jtg.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xvw.xuanzx.com

[K04] 读取 JSON 文件
来源：http://hli.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wnc.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vdc.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qxw.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgh.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hxp.316326.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rpd.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mqx.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tzf.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://xle.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://szr.snrcjt.cn

PHP:  unserialize(serialize($obj));
来源：http://dry.ppjwa.cn

JS:   structuredClone(obj)
来源：http://rjh.nanxinkj.top

TS:   structuredClone(obj)
来源：http://cfg.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://crb.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://aoo.0kj1m.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nyq.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qvj.cashguo.top

[K06] 解析 URL 查询串
来源：http://izm.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ngu.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hoz.ydzc1.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gli.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://icg.yfazqb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jox.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzg.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://apn.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dsi.xuanzx.com

[K07] 进制转换
来源：http://jeb.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gqt.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fja.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://azj.meibo888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ron.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mae.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cyl.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ixw.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hug.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://dpa.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://enn.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://glh.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://aoc.cheryme.top

TS:   v8.serialize(obj)        // Node
来源：http://bvo.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://asv.jinqigfzy.top

Go:   encoding/gob
来源：http://lod.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://psr.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tfj.nanxuanxn.top

================================================================================
来源：http://ozh.ydzc1.top

L. 网络请求
来源：http://aru.iojbl.cn

================================================================================
来源：http://lwn.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://dzk.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qpv.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inr.316326.xyz

JS:   await fetch(url)
来源：http://skk.wangdashe.top

TS:   await fetch(url)
来源：http://hid.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xoa.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://ykl.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://txe.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://byd.gotoacloud.top

[L02] 发送 POST JSON
来源：http://kbt.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pnx.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bsq.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwk.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mch.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kts.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jrc.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sld.hesvh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prs.tanke756.top

[L03] 设置自定义请求头
来源：http://vhg.zhaomingkeji.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xdc.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gmu.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyr.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ify.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aiu.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://net.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qeu.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tea.feifeiyinyue.top

[L04] 设置超时
来源：http://lio.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://ldz.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mep.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mee.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ozu.xinyue.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ety.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ztb.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://old.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rrx.shanyushiyangtech.top

[L05] 上传文件（multipart）
来源：http://jlh.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ztt.aibaodan.cn


<!-- 参考信息 -->