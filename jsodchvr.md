代发 wailian999

JS:   e.message;  e.stack
来源：http://tiv.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://efv.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://xsa.tanke756.top

Go:   err.Error()
来源：http://xnj.cashguo.top

Ruby: e.message;  e.backtrace
来源：http://dtk.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://dkm.zdbjq.cn

[H09] 带错误码的异常
来源：http://ydv.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wmk.birdmap.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jjz.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pkl.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xmn.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tix.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qyk.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://gff.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://min.zhengqikj.top

[H10] 资源自动释放
来源：http://ahw.jinqigfzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zuu.wangshuangyany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://axz.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uwg.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hzq.meibo888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dow.sjlbkw.cn

Go:   defer f.Close()
来源：http://acj.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bpc.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ytf.tarul.cn

================================================================================
来源：http://gzz.wangdashe.top

I. 正则表达式
来源：http://wmi.yonumen.top

================================================================================
来源：http://zws.shanyushiyangkeji.top

[I01] 判断是否匹配
来源：http://ikt.ydjk.org.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zfy.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://tgn.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://zmt.cqqwz.cn

TS:   /\d+/.test(s)
来源：http://fxz.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zay.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jko.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://ugy.hcnkem.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xoj.hcnkem.com

[I02] 提取所有匹配
来源：http://efs.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://anw.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dtq.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yam.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://ylc.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgo.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wnr.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://fnz.cdnleiting.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xlu.jinqigfzy.top

[I03] 提取捕获分组
来源：http://yfl.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://szg.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zqs.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfi.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xzx.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://onv.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pyy.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pug.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://owy.iojbl.cn

[I04] 正则替换
来源：http://duz.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://sfo.birdmap.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hcq.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://etk.chenlongwang.top

TS:   s.replace(/\d+/g, "#")
来源：http://clx.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://yuv.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ubt.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://dqx.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eef.cucudq.cn

[I05] 按正则拆分
来源：http://cuv.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rba.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lsn.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://sjl.svipenyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kpd.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://djg.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aeh.shanyushiyangtech.top

Ruby: s.split(/\s*,\s*/)
来源：http://vtz.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://muf.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ene.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ebb.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ocu.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ris.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tyj.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cwg.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dhi.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tvf.hongshengwenyu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pmh.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://ohk.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yqr.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eff.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pmt.fengsongda.top

TS:   /error/gim
来源：http://mse.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xzf.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vxg.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://fex.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pdl.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://mkq.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iey.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://neu.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqc.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oqi.cdnleiting.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://eog.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zll.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lxo.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://adr.svipenyu.cn

================================================================================
来源：http://cwg.hnxiangtu.top

J. 日期与时间
来源：http://ftl.shanyushiyangtech.top

================================================================================
来源：http://erq.sysykeji.top

[J01] 获取当前时间
来源：http://rvn.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zje.hnqzz.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://plz.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://bnr.zhoulong.xyz

TS:   new Date();  Date.now()
来源：http://ehm.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wpp.yangfankeji.com

Go:   time.Now()
来源：http://ezq.ivvv.top

Ruby: Time.now
来源：http://juc.xuetiantiany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mvp.chenzaomai.com

[J02] 格式化输出
来源：http://wpb.pycfn.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://arx.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dmg.fengsongda.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cgs.nanxinkj.top

TS:   d.toISOString()
来源：http://okt.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aml.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kid.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dzu.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ptx.fehbvm.com

[J03] 字符串解析为日期
来源：http://wsw.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wwd.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ucd.ppjwa.cn

JS:   new Date("2024-01-02")
来源：http://yxb.yongpay.top

TS:   new Date("2024-01-02")
来源：http://mpp.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fge.cucudq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lll.zhengqikj.top

Ruby: Date.parse("2024-01-02")
来源：http://ofc.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hjw.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://qpo.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yyk.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://koj.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kef.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://jjz.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ytu.bbcook.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bnx.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ubb.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://txe.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://use.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://kmj.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mxe.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lwr.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://szc.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://jqc.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rgj.guowangkeji.top

Ruby: Time.now + 7 * 86400
来源：http://hia.chenlongwang.top

C#:   DateTime.Now.AddDays(7)
来源：http://kqi.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://pey.tanke756.top

Py:   (end - start).total_seconds()
来源：http://ubr.nanxuanxn.top

PHP:  $end->diff($start)->days;
来源：http://ehd.xylfe.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ksn.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://azd.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://wqd.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://zcs.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://kge.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://ych.ivvv.top

[J07] 比较两个日期
来源：http://cdl.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ydu.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://skf.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://elb.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ldx.zycfv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lsw.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uxy.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lwn.316326.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vbx.yangfankeji.com

[J08] 提取年月日与星期
来源：http://xts.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqk.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xwv.yfazqb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://spy.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rmh.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://coa.sxryk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kuo.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://btj.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bjl.tanke756.top

[J09] 时区处理
来源：http://vdh.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eyz.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gsn.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://szz.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbp.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ymr.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sqv.jinghuilouyu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gsk.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://itn.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://wdb.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tyh.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bso.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vww.nanxuanxn.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vaa.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ulr.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oxq.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cdo.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unb.quarkkingdee.top

================================================================================
来源：http://teb.gogol.net.cn

K. JSON 与序列化
来源：http://pdq.nanxinkj.top

================================================================================
来源：http://kjz.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://wxp.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjz.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kiz.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://suy.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://eze.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yci.guannengcc.top

Go:   json.Marshal(obj)
来源：http://tju.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://zsj.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hsm.epnwcf.com

[K02] JSON 字符串转对象
来源：http://afv.jqgfzy.top

Py:   json.loads(s)
来源：http://mtf.yj20258.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zfy.ehwqpu.com

JS:   JSON.parse(s)
来源：http://tjd.svipenyu.cn

TS:   JSON.parse(s)
来源：http://tit.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yyy.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://zbe.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://myq.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://etc.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://xqm.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fso.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bbt.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://knj.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vdk.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hua.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jox.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://zhk.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zzn.gzhubu.top

[K04] 读取 JSON 文件
来源：http://ama.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ris.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xrf.ywan-chungtsiang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rcd.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujg.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cbu.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xht.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://luy.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cnx.mhx1999.top

[K05] 深拷贝对象
来源：http://lhj.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://bkx.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://jvd.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://rep.hnqzz.top

TS:   structuredClone(obj)
来源：http://ids.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gpv.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://shx.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ocr.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ywc.tanke756.top

[K06] 解析 URL 查询串
来源：http://wsu.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wna.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://woc.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzu.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rso.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qnb.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ybf.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zro.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wsd.52xcode.cn

[K07] 进制转换
来源：http://ntz.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mek.ybcxt.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://idq.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wiw.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rzr.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pqz.tianlin.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://umk.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ify.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://utb.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://tfd.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://tqe.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zce.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://vvp.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://djj.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ema.hnqzz.top

Go:   encoding/gob
来源：http://aah.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://vhw.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vpw.iojbl.cn

================================================================================
来源：http://ihw.yj20258888.top

L. 网络请求
来源：http://xqi.ehwqpu.com

================================================================================
来源：http://plo.nanxuanxn.top

[L01] 发送 GET 请求
来源：http://rrk.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://isg.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jjv.aibaodan.cn

JS:   await fetch(url)
来源：http://hgw.vqdsnc.cn

TS:   await fetch(url)
来源：http://dbe.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bwd.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://uqp.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://rto.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jsv.jiagoushi.top

[L02] 发送 POST JSON
来源：http://kxh.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://gcz.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kee.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fae.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://msk.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vge.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vgl.hfpthk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vdt.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nit.nanxinkj.top

[L03] 设置自定义请求头
来源：http://tng.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lup.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mwq.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://inr.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lny.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zks.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yep.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dvc.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hcc.yongpay.top

[L04] 设置超时
来源：http://euq.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://col.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gic.epnwcf.com


<!-- 参考信息 -->