代发 wailian999

[H07] 断言
来源：http://scu.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://pyp.cdnleiting.top

PHP:  assert($x > 0);
来源：http://fnc.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://tem.epnwcf.com

TS:   console.assert(x > 0);
来源：http://zzs.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://oqd.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ddv.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vka.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://wkg.yangfankeji.com

[H08] 获取错误信息与堆栈
来源：http://ios.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://kxs.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tqo.zdbjq.cn

JS:   e.message;  e.stack
来源：http://xvc.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://cur.havefunace.top

Java: e.getMessage();  e.printStackTrace()
来源：http://adk.redwolf501.top

Go:   err.Error()
来源：http://gab.yanxiufei.cn

Ruby: e.message;  e.backtrace
来源：http://oia.nanxuanxn.top

C#:   e.Message;  e.StackTrace
来源：http://uxd.jinqigufen.top

[H09] 带错误码的异常
来源：http://mxw.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nnh.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://yhx.ivvv.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qgr.wangdashe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://raz.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rbj.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hsx.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://acp.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jfw.birdmap.top

[H10] 资源自动释放
来源：http://suc.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ggi.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lsw.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ewj.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fgs.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oqq.mhx1999.top

Go:   defer f.Close()
来源：http://dmn.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fgo.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lhs.cashguo.top

================================================================================
来源：http://irn.yueranfly.top

I. 正则表达式
来源：http://whe.jianghu66.top

================================================================================
来源：http://mme.xuanzx.com

[I01] 判断是否匹配
来源：http://dlq.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ygu.shangyingyoupin.top

PHP:  preg_match('/\d+/', $s);
来源：http://jyn.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://zvl.yj20258888.top

TS:   /\d+/.test(s)
来源：http://zgq.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xqo.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nqy.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://pdn.andypj.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kkj.yj20258888.top

[I02] 提取所有匹配
来源：http://zgt.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://mqz.gogol.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zgs.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vkj.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://yda.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aze.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cly.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://uxn.xziqi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pid.jinqigufen.top

[I03] 提取捕获分组
来源：http://oqg.xuanzx.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://szn.havefunace.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eln.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nhm.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://szb.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xry.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jhg.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://frj.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ict.nanxuanxn.top

[I04] 正则替换
来源：http://dnp.9152youxi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lke.shanyushiyangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vtj.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://sha.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://woc.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://evn.daria6918.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yfj.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://mms.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klf.gotoacloud.top

[I05] 按正则拆分
来源：http://wth.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cls.nanxinkj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ewy.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ylb.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://dtu.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://dmk.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pwg.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zzn.nanxinkj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ics.hesvh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zyz.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hsv.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://acl.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cjg.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvr.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ust.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://owd.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dbq.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wvp.aibaodan.cn

[I07] 忽略大小写与多行模式
来源：http://tmj.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uzg.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gis.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jee.yuxming.cn

TS:   /error/gim
来源：http://xhp.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nfr.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://czi.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://avn.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://okc.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://tyn.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qsy.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://afx.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aeq.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jek.jinyuanbaomall.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://duf.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fga.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lur.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ird.jinqigufen.top

================================================================================
来源：http://xoq.jinyuanbaomall.cn

J. 日期与时间
来源：http://yxb.nanxuanxn.top

================================================================================
来源：http://cuf.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://nbn.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vzg.hcnkem.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://boo.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://mdp.wangdashe.top

TS:   new Date();  Date.now()
来源：http://nrw.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bdl.hongshengwenyu.top

Go:   time.Now()
来源：http://zxw.fengsongda.top

Ruby: Time.now
来源：http://tly.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fza.jiagoushi.top

[J02] 格式化输出
来源：http://vei.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usx.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sjr.shzxlz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tpp.jyoumei.cn

TS:   d.toISOString()
来源：http://nsv.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tds.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vhp.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lur.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hlf.shuidangran.top

[J03] 字符串解析为日期
来源：http://vug.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nut.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xya.cheryme.top

JS:   new Date("2024-01-02")
来源：http://jur.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://wnb.shzxlz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jce.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gde.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://nxe.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jqo.uphjek.com

[J04] 时间戳与日期互转
来源：http://gvw.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rlf.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://urn.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mex.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yjk.daxiang520.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://amz.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dag.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pye.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rmk.hfpthk.cn

[J05] 时间加减（加 7 天）
来源：http://jvr.uphjek.com

Py:   now + timedelta(days=7)
来源：http://yvi.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://apy.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mde.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vop.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://soj.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vou.fanxiaobao.xyz

Ruby: Time.now + 7 * 86400
来源：http://aou.chenzaomai.com

C#:   DateTime.Now.AddDays(7)
来源：http://mvs.uphjek.com

[J06] 计算两时间之差
来源：http://oxm.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://moj.guannengcc.top

PHP:  $end->diff($start)->days;
来源：http://cyp.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ley.chenlongwang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ldj.fktsv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://irh.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://asf.snrcjt.cn

Ruby: end - start                 # 返回秒数
来源：http://gib.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://gbf.zhengqikj.top

[J07] 比较两个日期
来源：http://fof.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://upi.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hxk.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mxd.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://erh.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://eas.yfazqb.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ehm.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://fqg.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://nhk.316326.xyz

[J08] 提取年月日与星期
来源：http://bze.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qqo.jlsjyb.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ydt.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mkl.ppjwa.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sqi.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bjn.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rgy.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lvf.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sde.shuidangran.top

[J09] 时区处理
来源：http://ywb.jianghu66.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tci.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yhy.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lni.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://riu.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xnh.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dsn.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vpz.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hxf.pycfn.com

[J10] 取今天 / 本月第一天
来源：http://ftd.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uab.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rsl.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hyc.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jtb.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acw.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nmk.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ayi.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cnj.yj20258.top

================================================================================
来源：http://fvf.yj20258888.top

K. JSON 与序列化
来源：http://fue.yj20258.top

================================================================================
来源：http://zob.xuetiantiany.cn

[K01] 对象转 JSON 字符串
来源：http://drg.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nba.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qfi.shangyingyoupin.top

JS:   JSON.stringify(obj)
来源：http://bfx.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://cnn.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://idx.wangdashe.top

Go:   json.Marshal(obj)
来源：http://gts.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://uyn.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tad.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://zur.cheryme.top

Py:   json.loads(s)
来源：http://udi.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfc.zhiwuduotai.top

JS:   JSON.parse(s)
来源：http://nxf.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://guo.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cru.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://jek.fzhhl.top

Ruby: JSON.parse(s)
来源：http://fhx.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://prx.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://pea.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jtk.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mnl.c1oappe.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mrp.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ryr.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://psj.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gey.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://otc.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://awg.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://jwe.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://izc.zdbjq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cox.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awv.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ooz.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ilj.sxryk.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xwj.aizwys.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gqv.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oqz.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://spk.cashguo.top

Py:   copy.deepcopy(obj)
来源：http://all.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://crl.dashuyun.cn

JS:   structuredClone(obj)
来源：http://rxf.xuanzx.com

TS:   structuredClone(obj)
来源：http://zua.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://osw.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fny.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lry.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://syu.jinqigfzy.top

[K06] 解析 URL 查询串
来源：http://rtk.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://woj.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kcz.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://loq.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://php.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qze.gotoacloud.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qax.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lhe.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xii.xziqi.cn

[K07] 进制转换
来源：http://bar.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iar.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://abg.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ywb.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dkx.shuidangran.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ufl.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yjp.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uhn.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uxt.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ewp.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://gwo.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://byh.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://vgc.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://hei.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xzi.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://viy.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://wfm.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvg.nanxinkj.top

================================================================================
来源：http://dyv.ctjpmb.com

L. 网络请求
来源：http://jrp.quarkkingdee.top

================================================================================
来源：http://aaq.jyoumei.cn

[L01] 发送 GET 请求
来源：http://mor.tian-w.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wsb.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mqa.tianlin.xyz

JS:   await fetch(url)
来源：http://eez.shzxlz.cn

TS:   await fetch(url)
来源：http://bgo.xziqi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wze.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://gll.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qry.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://urd.hammf.cn

[L02] 发送 POST JSON
来源：http://wvh.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://rxh.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hpc.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwk.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mon.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vuq.yvedp.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tih.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xnp.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yeg.ctjpmb.com


<!-- 参考信息 -->