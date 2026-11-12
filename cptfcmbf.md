代发 wailian999

[H07] 断言
来源：http://mui.jinyuanbaomall.cn

Py:   assert x > 0, "必须为正"
来源：http://mqt.daxiang520.top

PHP:  assert($x > 0);
来源：http://slb.zycfv.cn

JS:   console.assert(x > 0);
来源：http://bzl.aizwys.cn

TS:   console.assert(x > 0);
来源：http://wro.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://bww.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gvu.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rfn.yfazqb.com

C#:   Debug.Assert(x > 0);
来源：http://din.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://poz.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://rbo.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bsg.cucudq.cn

JS:   e.message;  e.stack
来源：http://tsb.shuidangran.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ytx.zdbjq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nim.ctjpmb.com

Go:   err.Error()
来源：http://rde.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://uaw.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://nmn.nanxuanxn.top

[H09] 带错误码的异常
来源：http://pzf.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sua.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://els.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qvc.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://guc.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zbk.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ykj.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://qzd.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zzi.yj202588.top

[H10] 资源自动释放
来源：http://vuw.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vbt.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ggi.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bro.yueranfly.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hsn.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zjj.xuanzx.com

Go:   defer f.Close()
来源：http://sov.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ius.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fqf.ywan-chungtsiang.top

================================================================================
来源：http://xvi.bjfxy.top

I. 正则表达式
来源：http://fxu.sufxvd.cn

================================================================================
来源：http://bqz.vqdsnc.cn

[I01] 判断是否匹配
来源：http://rpl.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ndz.yuxming.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pta.sufxvd.cn

JS:   /\d+/.test(s)
来源：http://xbd.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://ywr.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iai.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nwi.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://rao.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ysc.andypj.xyz

[I02] 提取所有匹配
来源：http://sba.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://iia.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ffg.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pwz.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://cki.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gsx.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zhs.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://sft.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ldp.jinqigufen.top

[I03] 提取捕获分组
来源：http://gvg.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uvq.guannengcc.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jwl.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ufm.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fbq.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://imy.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ykh.gotoacloud.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqx.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypg.hesvh.cn

[I04] 正则替换
来源：http://pst.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jlv.jlsjyb.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hyg.haohaochexian.top

JS:   s.replace(/\d+/g, "#")
来源：http://eni.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://qfd.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://gyx.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://scl.wangdashe.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hyt.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vjz.snrcjt.cn

[I05] 按正则拆分
来源：http://tis.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://rot.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bpz.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://fec.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://agy.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://lzv.birdmap.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wbl.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://fbw.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zst.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lgs.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jet.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pxn.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fud.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rtl.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fvc.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ebp.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ray.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zuf.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://nco.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lkh.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://boy.uphjek.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nst.meibo888.top

TS:   /error/gim
来源：http://zen.fengsongda.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://upd.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jiw.shanyushiyangtech.top

Ruby: s.scan(/error/i)
来源：http://wsl.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ejm.havefunace.top

[I08] 贪婪与非贪婪匹配
来源：http://enu.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ygo.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndu.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://glq.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://moa.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://tjo.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nhc.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yho.nanxinkj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://akw.52xcode.cn

================================================================================
来源：http://zmn.haohaochexian.top

J. 日期与时间
来源：http://ipa.tian-w.cn

================================================================================
来源：http://jky.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://wec.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ajq.xylfe.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xbz.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://uwu.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://cfc.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jva.gaohongyu789.top

Go:   time.Now()
来源：http://uvt.feifeiyinyue.top

Ruby: Time.now
来源：http://wcr.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://biu.ehwqpu.com

[J02] 格式化输出
来源：http://njb.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://roa.zycfv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dqb.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tme.yuanzhike.top

TS:   d.toISOString()
来源：http://rcr.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jkx.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uaz.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qcj.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://feg.jianghu66.top

[J03] 字符串解析为日期
来源：http://pmk.smart0.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jew.pengpengdd.cyou

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qbt.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://mxj.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://pgl.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ger.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://flq.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://jqe.feifeiyinyue.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hfd.gzhubu.top

[J04] 时间戳与日期互转
来源：http://tlb.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dcn.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xsg.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kjw.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ain.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yoe.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cko.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://shw.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zcf.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://kzj.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://nrd.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rzw.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jqa.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hha.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://pvw.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mwd.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://llu.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://dmm.yanxiufei.cn

[J06] 计算两时间之差
来源：http://ist.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://doy.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://cny.aibaodan.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xdd.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qbr.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://tpm.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://pcj.ctjpmb.com

Ruby: end - start                 # 返回秒数
来源：http://hws.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://wlx.xuetiantiany.cn

[J07] 比较两个日期
来源：http://hof.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://iji.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mar.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://sab.tianlin.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://avz.yj202588.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sou.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iqc.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://drd.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://ijd.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://fup.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nln.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lvc.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dmi.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wvm.gogol.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://brz.yonumen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tmv.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ggk.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rja.gaohongyu789.top

[J09] 时区处理
来源：http://kfz.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nse.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://skb.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://niu.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cae.ywan-chungtsiang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wuo.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bby.hcnkem.com

Ruby: Time.now.getlocal("+08:00")
来源：http://wkz.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iio.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://jiv.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cva.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vxg.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://els.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mac.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ntj.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ocw.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ull.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dos.birdmap.top

================================================================================
来源：http://tiz.shanyushiyangtech.top

K. JSON 与序列化
来源：http://bdg.zhixingplan.top

================================================================================
来源：http://mkz.ehwqpu.com

[K01] 对象转 JSON 字符串
来源：http://iyz.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bkz.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ckl.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://lyh.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://kug.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmz.bjfxy.top

Go:   json.Marshal(obj)
来源：http://gqq.yvedp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wgo.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mri.ydzc1.top

[K02] JSON 字符串转对象
来源：http://npx.jqgufenzy.top

Py:   json.loads(s)
来源：http://ysf.chenjidiqi.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qoe.yj202588.top

JS:   JSON.parse(s)
来源：http://dhd.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://jqp.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zhx.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://obc.nwbrower.top

Ruby: JSON.parse(s)
来源：http://krb.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://chw.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://dwe.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dve.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://atj.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lgv.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://vlc.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oin.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sqb.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://psg.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pcx.zycfv.cn

[K04] 读取 JSON 文件
来源：http://xal.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kaa.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ipz.jiagoushi.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gvl.gaohongyu789.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zbw.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nvx.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ckk.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sst.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oab.tianlin.xyz

[K05] 深拷贝对象
来源：http://dpr.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://aoz.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://tio.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://cfr.hywenlv.cn

TS:   structuredClone(obj)
来源：http://bwj.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://emt.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jkv.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ewu.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://euk.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://igy.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bvn.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lwm.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ttl.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyl.nwbrower.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fwf.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://suu.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ldx.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uat.wangdashe.top

[K07] 进制转换
来源：http://shq.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://unc.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oii.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://muy.chenzaomai.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cue.fanxiaobao.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fhb.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nqg.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xir.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://crc.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://rsr.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://qxm.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bal.pycfn.com

JS:   v8.serialize(obj)        // Node
来源：http://yyr.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://bac.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aqi.yfazqb.com

Go:   encoding/gob
来源：http://nnf.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://jqb.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wii.0kj1m.cn

================================================================================
来源：http://ooy.meibo888.top

L. 网络请求
来源：http://eva.cheryme.top

================================================================================
来源：http://qia.pycfn.com

[L01] 发送 GET 请求
来源：http://jvz.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kok.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://poh.yangfankeji.com

JS:   await fetch(url)
来源：http://nxx.zhiwuduotai.top

TS:   await fetch(url)
来源：http://ink.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qio.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://vuj.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vfd.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jdf.guannengcc.top

[L02] 发送 POST JSON
来源：http://xke.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://emy.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xzh.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://umi.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fvy.zhongyouzk.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ozx.ctjpmb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mth.52xcode.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jgr.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ahh.guowangkeji.top


<!-- 参考信息 -->