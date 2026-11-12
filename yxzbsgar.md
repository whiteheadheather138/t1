代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lyp.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://npa.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dje.zhixingplan.top

[H06] 可选值 / 空值安全访问
来源：http://cgx.shuidangran.top

Py:   value = d.get("k") or default
来源：http://dth.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dqp.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://lci.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://vsv.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yxi.tianlin.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://aps.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://yxc.jyoumei.cn

C#:   obj?.A?.B ?? default
来源：http://ajf.epnwcf.com

[H07] 断言
来源：http://kfp.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://swj.xuanzx.com

PHP:  assert($x > 0);
来源：http://pjb.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://duf.sweek.top

TS:   console.assert(x > 0);
来源：http://ydl.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://lxf.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://etx.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qyv.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://ups.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://chl.hfpthk.cn

Py:   str(e);  traceback.format_exc()
来源：http://ujz.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xaq.zhiwuduotai.top

JS:   e.message;  e.stack
来源：http://fhz.aibaodan.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bwf.cucudq.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://riy.kuanghao11.cn

Go:   err.Error()
来源：http://cgh.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://gzq.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://uov.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://ueh.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gyc.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://oae.sxryk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ezg.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kto.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://srh.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nmc.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://kgo.vehdjk.com

C#:   // 自定义异常类中加 Code 属性
来源：http://etc.yongpay.top

[H10] 资源自动释放
来源：http://rsf.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nug.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dlm.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ilz.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hqy.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pug.xylfe.cn

Go:   defer f.Close()
来源：http://lbb.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kgz.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vpj.shuidangran.top

================================================================================
来源：http://bba.ywan-chungtsiang.top

I. 正则表达式
来源：http://kzr.bjfxy.top

================================================================================
来源：http://gav.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://tpa.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://enb.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://utj.hcnkem.com

JS:   /\d+/.test(s)
来源：http://ale.yj20258888.top

TS:   /\d+/.test(s)
来源：http://obb.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bbw.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kgj.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://ypc.fehbvm.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fpa.haohaochexian.top

[I02] 提取所有匹配
来源：http://qpk.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://cbr.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cll.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ddq.jqgfzy.top

TS:   s.match(/\d+/g)
来源：http://ehv.jiagoushi.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vyr.zycfv.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://reo.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://lyw.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://svo.hysaishi.cn

[I03] 提取捕获分组
来源：http://etd.jyoumei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dho.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mvz.zdqjudy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kst.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tlc.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dfb.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://elw.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zwk.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vid.zhiwuduotai.top

[I04] 正则替换
来源：http://mrq.yj20258.top

Py:   re.sub(r"\d+", "#", s)
来源：http://anf.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tjv.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cso.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://lgf.hammf.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gex.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lau.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://icw.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aok.havefunace.top

[I05] 按正则拆分
来源：http://owq.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vmo.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jkx.yj202588.top

JS:   s.split(/\s*,\s*/)
来源：http://twv.epnwcf.com

TS:   s.split(/\s*,\s*/)
来源：http://sgj.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://rdr.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qlw.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ijz.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yza.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://prg.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://btp.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://trp.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtw.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vzv.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://afk.svipenyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bqy.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mvp.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aav.gaohongyu789.top

[I07] 忽略大小写与多行模式
来源：http://kgm.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qyh.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xqp.guowangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bof.smart0.xyz

TS:   /error/gim
来源：http://num.cqqwz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rsc.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uyy.havefunace.top

Ruby: s.scan(/error/i)
来源：http://dpt.ydjk.org.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kuz.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://ypk.hysaishi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://btq.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://odc.nanxinkj.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mxc.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mup.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qho.zhoulong.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eip.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://psd.hongshengwenyu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wpy.snrcjt.cn

================================================================================
来源：http://ahx.jyoumei.cn

J. 日期与时间
来源：http://sul.pengpengdd.cyou

================================================================================
来源：http://tuw.gotoacloud.top

[J01] 获取当前时间
来源：http://six.cqqwz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ijd.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hun.hnqzz.top

JS:   new Date();  Date.now()
来源：http://rko.tian-w.cn

TS:   new Date();  Date.now()
来源：http://lqn.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gks.chenzaomai.com

Go:   time.Now()
来源：http://xue.yonumen.top

Ruby: Time.now
来源：http://hom.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jse.quarkkingdee.top

[J02] 格式化输出
来源：http://ozw.cucudq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzj.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mkb.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dlb.ivvv.top

TS:   d.toISOString()
来源：http://oox.svipenyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ysb.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hjg.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bul.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xxl.shuidangran.top

[J03] 字符串解析为日期
来源：http://cyp.yuxming.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://clu.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lsn.ydzc1.top

JS:   new Date("2024-01-02")
来源：http://hem.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://dak.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://isq.wangshuangyany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ror.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://llk.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sok.nwbrower.top

[J04] 时间戳与日期互转
来源：http://qvg.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://odv.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uvq.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://myt.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qpa.sufxvd.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://geb.yangfankeji.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ksk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvd.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nec.daria6918.cn

[J05] 时间加减（加 7 天）
来源：http://fno.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://xvq.iojbl.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ygh.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jli.vehdjk.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqp.shanyushiyangtech.top

Java: LocalDate.now().plusDays(7)
来源：http://hqw.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tsg.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://sxy.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://odo.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://nbk.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://lvf.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://aek.hnxiangtu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lwv.kuanghao11.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eew.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zuz.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://jpi.vqdsnc.cn

Ruby: end - start                 # 返回秒数
来源：http://qtz.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://cyf.xziqi.cn

[J07] 比较两个日期
来源：http://zlh.chenzaomai.com

Py:   d1 < d2;  d1 == d2
来源：http://odq.tianlin.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tba.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://amn.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://klu.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ocq.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uxq.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://air.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://vmj.feifeiyinyue.top

[J08] 提取年月日与星期
来源：http://fce.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kos.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tcb.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xco.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rel.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rms.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iyy.yfazqb.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rqz.yuanzhike.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nnq.jiagoushi.top

[J09] 时区处理
来源：http://xki.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ajt.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cdp.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbi.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wqz.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sdt.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hmb.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mje.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lee.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://slk.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://bmy.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ldb.tarul.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iye.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://htr.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://myy.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nia.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wda.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sdb.tarul.cn

================================================================================
来源：http://paq.aizwys.cn

K. JSON 与序列化
来源：http://umj.yongpay.top

================================================================================
来源：http://equ.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://waq.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ucc.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dlr.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://fjv.jinghuilouyu.cn

TS:   JSON.stringify(obj)
来源：http://kep.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://erm.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://gpv.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://iey.chenlongwang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aia.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://ngt.chenjidiqi.icu

Py:   json.loads(s)
来源：http://kpw.guannengcc.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qbe.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://kgm.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://wxr.iojbl.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sab.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://nxx.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://uwb.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qzf.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://vwt.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kja.vehdjk.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wde.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://smy.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pjo.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mwh.c1oappe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://slu.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://dql.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hhk.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://qvt.gotoacloud.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rqg.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zpc.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://npx.daxiang520.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://krh.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://djv.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyg.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://sgd.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kiz.xylfe.cn

[K05] 深拷贝对象
来源：http://fus.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://pbi.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://ecw.fehbvm.com

JS:   structuredClone(obj)
来源：http://zgx.52xcode.cn

TS:   structuredClone(obj)
来源：http://qyf.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://lkr.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jnp.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vsr.redwolf501.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cuk.xinyue.icu

[K06] 解析 URL 查询串
来源：http://odd.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://etb.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jfc.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gvo.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dtu.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ahl.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://npb.52xcode.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ucw.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hnf.xuanzx.com

[K07] 进制转换
来源：http://rye.tianlin.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://izd.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iev.zhongyouzk.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yrz.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bda.tarul.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ggg.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zyj.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gqy.yvedp.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nmo.yfazqb.com

[K08] 二进制序列化（非 JSON）
来源：http://dwt.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://vji.shangyingyoupin.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qid.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://fjp.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://gka.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rtk.aibaodan.cn

Go:   encoding/gob
来源：http://jpx.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://vyp.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tuz.chenjidiqi.icu

================================================================================
来源：http://kev.fengsongda.top

L. 网络请求
来源：http://hwl.fehbvm.com

================================================================================
来源：http://rem.mhx1999.top

[L01] 发送 GET 请求
来源：http://eoc.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dzx.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hxh.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://uxc.xuanzx.com

TS:   await fetch(url)
来源：http://ecu.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lul.zhoulong.xyz


<!-- 参考信息 -->