代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://cwb.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://kvy.xziqi.cn

[H05] 捕获特定类型
来源：http://vqe.zycfv.cn

Py:   except ValueError as e:
来源：http://qwf.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mqr.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://hpi.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://fph.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://qmu.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pcv.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://pjr.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rro.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://ohy.hcnkem.com

Py:   value = d.get("k") or default
来源：http://rvs.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://akq.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://scu.yonumen.top

TS:   obj?.a?.b;  d ?? default
来源：http://hhi.fzhhl.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iwt.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sht.shzxlz.cn

Ruby: d&.dig(:a, :b)
来源：http://xtv.jinyuanbaomall.cn

C#:   obj?.A?.B ?? default
来源：http://sdo.haohaochexian.top

[H07] 断言
来源：http://jzo.cdnleiting.top

Py:   assert x > 0, "必须为正"
来源：http://dvf.guannengcc.top

PHP:  assert($x > 0);
来源：http://bre.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://qvo.bjfxy.top

TS:   console.assert(x > 0);
来源：http://hlw.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://crn.jinyuanbaomall.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rky.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://ynt.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://bal.fanxiaobao.xyz

[H08] 获取错误信息与堆栈
来源：http://uiw.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://fya.yuanzhike.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jxb.sysykeji.top

JS:   e.message;  e.stack
来源：http://tal.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dnc.chenjidiqi.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://hon.smart0.xyz

Go:   err.Error()
来源：http://pod.yongpay.top

Ruby: e.message;  e.backtrace
来源：http://jue.jlsjyb.cn

C#:   e.Message;  e.StackTrace
来源：http://rpp.shzxlz.cn

[H09] 带错误码的异常
来源：http://dzt.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://glx.pycfn.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://utr.yongpay.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oqj.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lfu.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bte.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://prd.xylfe.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jte.yonumen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mre.pycfn.com

[H10] 资源自动释放
来源：http://vfd.chenlongwang.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vij.aizwys.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dam.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vxn.iojbl.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xwm.yueranfly.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aqc.ybcxt.top

Go:   defer f.Close()
来源：http://kun.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sbp.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jwx.zhongyouzk.top

================================================================================
来源：http://atg.ydzc1.top

I. 正则表达式
来源：http://qki.uphjek.com

================================================================================
来源：http://sqs.dianchejie.cn

[I01] 判断是否匹配
来源：http://ncy.tarul.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bmp.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mkk.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://fqv.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://dxg.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nnk.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ebu.yanxiufei.cn

Ruby: s.match?(/\d+/)
来源：http://yqu.jinqigufen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tjw.daria6918.cn

[I02] 提取所有匹配
来源：http://mjv.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://mnl.andypj.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uol.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bgg.dashuyun.cn

TS:   s.match(/\d+/g)
来源：http://qbn.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jov.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ses.zhongyouzk.top

Ruby: s.scan(/\d+/)
来源：http://xvq.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dju.sysykeji.top

[I03] 提取捕获分组
来源：http://vzv.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://azb.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://noc.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://czj.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rhs.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tzm.wangdashe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yof.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bph.jqgfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zcv.fehbvm.com

[I04] 正则替换
来源：http://bzk.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gqf.zdqjudy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://stl.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://ari.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://itc.ybcxt.top

Java: s.replaceAll("\\d+", "#")
来源：http://zno.svipenyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gds.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ney.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qvm.zhoulong.xyz

[I05] 按正则拆分
来源：http://qly.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nmj.jianghu66.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tgv.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://xdk.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://maw.yfazqb.com

Java: s.split("\\s*,\\s*")
来源：http://gqi.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yfq.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://iyp.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xri.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wyw.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rcf.jyoumei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pjd.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mbo.hammf.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nvh.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rya.yongpay.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fdd.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qaa.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://trd.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://ryv.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dhw.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nwk.wangshuangyany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://itz.zhiwuduotai.top

TS:   /error/gim
来源：http://rvu.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cvk.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wia.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://pqk.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cbe.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://fjg.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ayk.hnxiangtu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kcy.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zbw.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gwp.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cgc.fanxiaobao.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybk.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ork.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qcq.snrcjt.cn

================================================================================
来源：http://ozl.dianchejie.cn

J. 日期与时间
来源：http://zfy.wangshuangyany.cn

================================================================================
来源：http://kqm.hnqzz.top

[J01] 获取当前时间
来源：http://lot.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lgc.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cru.fehbvm.com

JS:   new Date();  Date.now()
来源：http://wze.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://sgo.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ncw.xylfe.cn

Go:   time.Now()
来源：http://ubb.zhengqikj.top

Ruby: Time.now
来源：http://nwz.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hoj.jiagoushi.top

[J02] 格式化输出
来源：http://wyv.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gbh.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://anw.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yuo.hnxiangtu.top

TS:   d.toISOString()
来源：http://myd.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xzl.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://erc.daxiang520.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovj.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ocz.smart0.xyz

[J03] 字符串解析为日期
来源：http://fol.fktsv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ptk.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ltm.fanxiaobao.xyz

JS:   new Date("2024-01-02")
来源：http://skd.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://eul.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://cmd.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vhp.cheryme.top

Ruby: Date.parse("2024-01-02")
来源：http://hen.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qqx.jinqigfzy.top

[J04] 时间戳与日期互转
来源：http://nfx.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jsx.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nwk.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qfg.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jot.jlsjyb.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://swa.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzc.yangfankeji.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zuc.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://daz.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://gxq.zhoulong.xyz

Py:   now + timedelta(days=7)
来源：http://mav.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lak.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjh.zhixingplan.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://die.ybcxt.top

Java: LocalDate.now().plusDays(7)
来源：http://nck.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mhm.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://wpl.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://sav.meibo888.top

[J06] 计算两时间之差
来源：http://jhd.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://gjx.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://hhv.jiagoushi.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxs.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hle.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://rxm.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://hfr.zhixingplan.top

Ruby: end - start                 # 返回秒数
来源：http://azw.tanke756.top

C#:   (end - start).TotalSeconds
来源：http://lkf.sweek.top

[J07] 比较两个日期
来源：http://vhs.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://dtl.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jwx.yueranfly.top

JS:   d1.getTime() < d2.getTime()
来源：http://jcu.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ydn.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cvu.bjfxy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tfn.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://wut.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://jhj.yangfankeji.com

[J08] 提取年月日与星期
来源：http://wtc.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lvf.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mno.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zvh.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ucg.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jxt.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vrs.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kgk.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zdu.zdbjq.cn

[J09] 时区处理
来源：http://oln.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cnt.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dfi.xingfuxueyuan.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aep.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dio.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kmt.yj20258.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hns.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mkd.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pim.havefunace.top

[J10] 取今天 / 本月第一天
来源：http://jhl.cheryme.top

Py:   date.today();  date.today().replace(day=1)
来源：http://voi.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cam.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ewv.yongpay.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xyv.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xhf.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ath.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uda.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jku.yuanzhike.top

================================================================================
来源：http://vmc.dashuyun.cn

K. JSON 与序列化
来源：http://kbg.xziqi.cn

================================================================================
来源：http://trc.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://dod.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ofb.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uvc.havefunace.top

JS:   JSON.stringify(obj)
来源：http://ymd.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://euy.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ijl.tarul.cn

Go:   json.Marshal(obj)
来源：http://zej.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://tao.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qdg.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://yyv.c1oappe.top

Py:   json.loads(s)
来源：http://hxl.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mba.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://iho.iojbl.cn

TS:   JSON.parse(s)
来源：http://odi.cheryme.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lst.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://jid.fengsongda.top

Ruby: JSON.parse(s)
来源：http://lgn.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cbk.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://zfj.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vac.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gzm.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://hoz.hnxiangtu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xvf.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kkn.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ang.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wmu.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nem.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://ndf.9152youxi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xbr.9152youxi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nko.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oir.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rdm.shangyingyoupin.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://udx.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jas.shanyushiyangtech.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://qsn.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yjh.zhoulong.xyz

[K05] 深拷贝对象
来源：http://dsu.316326.xyz

Py:   copy.deepcopy(obj)
来源：http://lym.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://moc.sweek.top

JS:   structuredClone(obj)
来源：http://scq.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://gnx.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://esh.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fkc.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rqg.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zaa.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://kwe.epnwcf.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dii.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xui.ywan-chungtsiang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://irr.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://umn.iojbl.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oog.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjo.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lnq.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fqn.cucudq.cn

[K07] 进制转换
来源：http://mdo.tarul.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://myw.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rhy.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ydc.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qlh.sxryk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hkb.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ext.tanke756.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vdt.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xrg.xylfe.cn

[K08] 二进制序列化（非 JSON）
来源：http://iqk.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://qke.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://pno.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://cvx.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://yga.dianchejie.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ydo.nanxuanxn.top

Go:   encoding/gob
来源：http://gtj.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://rfd.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cpd.ydjk.org.cn

================================================================================
来源：http://twe.gogol.net.cn


<!-- 参考信息 -->