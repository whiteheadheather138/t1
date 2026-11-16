代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zpi.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://qoh.cheryme.top

TS:   if (e instanceof TypeError) {}
来源：http://apb.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://rcm.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lsd.zhaomingkeji.xyz

Ruby: rescue ArgumentError => e
来源：http://qrs.jqgfzy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dmf.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://gel.vehdjk.com

Py:   value = d.get("k") or default
来源：http://bkn.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://wjw.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://mlu.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zia.jianghu66.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ixw.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://grt.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://fub.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://xth.iojbl.cn

[H07] 断言
来源：http://nwi.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://hdn.jinqigfzy.top

PHP:  assert($x > 0);
来源：http://sbc.havefunace.top

JS:   console.assert(x > 0);
来源：http://zap.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://hfa.ydzc1.top

Java: assert x > 0 : "必须为正";
来源：http://gfz.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://idh.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://awi.shuidangran.top

C#:   Debug.Assert(x > 0);
来源：http://psv.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://dfc.hesvh.cn

Py:   str(e);  traceback.format_exc()
来源：http://zya.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ldl.tanke756.top

JS:   e.message;  e.stack
来源：http://odb.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iqc.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://aip.wangdashe.top

Go:   err.Error()
来源：http://ifh.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://gja.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://qgj.yfazqb.com

[H09] 带错误码的异常
来源：http://mug.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vpn.yj20258888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yji.hywenlv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uig.jinqigfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nro.jiagoushi.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xzy.yueranfly.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tyt.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://etp.vqdsnc.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rue.zhengqikj.top

[H10] 资源自动释放
来源：http://ldt.nanxinkj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://htr.yonumen.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vab.9152youxi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wca.tianlin.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fdn.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tjb.jqgufenzy.top

Go:   defer f.Close()
来源：http://lhg.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gvo.jqgufenzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vav.xziqi.cn

================================================================================
来源：http://bwc.316326.xyz

I. 正则表达式
来源：http://yka.tanke756.top

================================================================================
来源：http://bzk.jiagoushi.top

[I01] 判断是否匹配
来源：http://khd.fzhhl.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cix.andypj.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://nim.uphjek.com

JS:   /\d+/.test(s)
来源：http://wtm.hfpthk.cn

TS:   /\d+/.test(s)
来源：http://arm.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eii.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tso.aizwys.cn

Ruby: s.match?(/\d+/)
来源：http://fqg.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ahg.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://qnd.wangdashe.top

Py:   re.findall(r"\d+", s)
来源：http://cno.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zza.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pio.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://zkl.aizwys.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cnv.xziqi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ffk.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://tsm.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wta.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://jjb.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://anl.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eed.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ocp.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gii.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lxt.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xxv.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ntd.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://myv.nanxinkj.top

[I04] 正则替换
来源：http://jtg.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ylh.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tfb.c1oappe.top

JS:   s.replace(/\d+/g, "#")
来源：http://cyg.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tnv.gotoacloud.top

Java: s.replaceAll("\\d+", "#")
来源：http://oxe.havefunace.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wmo.gzhubu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iyc.cdnleiting.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iia.tianlin.xyz

[I05] 按正则拆分
来源：http://lnt.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mkv.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kki.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://tsd.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://ngw.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://nos.jyoumei.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://win.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://djr.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bgj.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mvt.sxryk.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jir.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rak.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uyj.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://orj.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://raj.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wov.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bkq.tian-w.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zow.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://egs.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zyv.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hrz.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pur.snrcjt.cn

TS:   /error/gim
来源：http://zzk.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tml.yj20258.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qxh.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://xvg.zhiwuduotai.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bzu.wangdashe.top

[I08] 贪婪与非贪婪匹配
来源：http://sze.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wnr.sufxvd.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iso.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://shl.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hcc.jqgufenzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://klk.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hsx.smart0.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bwq.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ivt.yuxming.cn

================================================================================
来源：http://fno.haohaochexian.top

J. 日期与时间
来源：http://mow.jyoumei.cn

================================================================================
来源：http://lne.52xcode.cn

[J01] 获取当前时间
来源：http://jjq.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yaw.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rnl.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://dal.dashuyun.cn

TS:   new Date();  Date.now()
来源：http://zpz.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://nuc.vehdjk.com

Go:   time.Now()
来源：http://syy.gzhubu.top

Ruby: Time.now
来源：http://ttk.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rmy.shzxlz.cn

[J02] 格式化输出
来源：http://tre.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yzk.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ofb.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aog.shangyingyoupin.top

TS:   d.toISOString()
来源：http://czr.jiagoushi.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jdl.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dwx.sxryk.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kze.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tkx.yj20258888.top

[J03] 字符串解析为日期
来源：http://xly.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eag.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jst.tian-w.cn

JS:   new Date("2024-01-02")
来源：http://qfk.ivvv.top

TS:   new Date("2024-01-02")
来源：http://jfn.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://hpe.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lwt.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://zyc.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qdc.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://ujh.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qfc.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fza.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iea.aizwys.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mpi.smart0.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vqs.gzhubu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gml.xingfuxueyuan.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vdl.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pxz.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://meq.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://jug.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hoq.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bei.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hhu.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://noh.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qnw.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://aha.gogol.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://txt.hnqzz.top

[J06] 计算两时间之差
来源：http://aay.ppjwa.cn

Py:   (end - start).total_seconds()
来源：http://vah.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://qvb.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://evp.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohy.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://uob.chenzaomai.com

Go:   end.Sub(start).Hours()
来源：http://qpz.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://nad.sweek.top

C#:   (end - start).TotalSeconds
来源：http://fsj.zycfv.cn

[J07] 比较两个日期
来源：http://lgz.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://iay.xinyue.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://his.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://xqs.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://jsd.ywan-chungtsiang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lct.shzxlz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fdu.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://inf.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://weu.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://olz.52xcode.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ozx.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://njp.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qyl.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ynt.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xsp.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pkt.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://big.shanyushiyangtech.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eil.tianlin.xyz

[J09] 时区处理
来源：http://cdr.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hmw.shangyingyoupin.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://khb.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bso.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rat.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://igt.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iuk.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://crl.zdqjudy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://amp.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://vun.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://grn.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rhn.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zrk.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://leq.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tat.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dvo.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xxu.sysykeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogm.jinyuanbaomall.cn

================================================================================
来源：http://tny.xylfe.cn

K. JSON 与序列化
来源：http://hie.yvedp.cn

================================================================================
来源：http://nkd.jianghu66.top

[K01] 对象转 JSON 字符串
来源：http://dzr.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dhd.fktsv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hcu.sweek.top

JS:   JSON.stringify(obj)
来源：http://nfw.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://aec.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wvx.ivvv.top

Go:   json.Marshal(obj)
来源：http://njm.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://txa.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://udd.0kj1m.cn

[K02] JSON 字符串转对象
来源：http://dht.ydjk.org.cn

Py:   json.loads(s)
来源：http://ubz.shuidangran.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://otx.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://pwf.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://roa.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gsl.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://tnq.daxiang520.top

Ruby: JSON.parse(s)
来源：http://paj.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ndg.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://xns.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fhh.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rgh.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gld.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://arc.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iiq.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pft.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://elg.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qdp.hesvh.cn

[K04] 读取 JSON 文件
来源：http://jzn.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://krk.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nxd.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://srf.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://otb.gaohongyu789.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pti.hesvh.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wax.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rpl.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mqz.yuanzhike.top

[K05] 深拷贝对象
来源：http://xoj.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://jip.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://cos.hnxiangtu.top

JS:   structuredClone(obj)
来源：http://waw.meibo888.top

TS:   structuredClone(obj)
来源：http://qrh.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ibg.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jbv.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://byb.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oyv.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://lui.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gks.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dxd.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjw.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://foc.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vud.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjk.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dnv.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xml.shuidangran.top

[K07] 进制转换
来源：http://yux.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lpm.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://njl.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yap.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ucg.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dnt.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mfi.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://klc.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fdn.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dhn.yj202588.top

Py:   pickle.dumps(obj)
来源：http://qmj.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wvp.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://cbw.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://yjn.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nog.aizwys.cn

Go:   encoding/gob
来源：http://lms.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://rid.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qaj.hnxiangtu.top

================================================================================
来源：http://dix.gotoacloud.top

L. 网络请求
来源：http://zic.gotoacloud.top

================================================================================
来源：http://dky.316326.xyz

[L01] 发送 GET 请求
来源：http://uxo.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://awa.cucudq.cn


<!-- 参考信息 -->