代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://iui.hammf.cn

C#:   class MyException : Exception {}
来源：http://rbn.svipenyu.cn

[H05] 捕获特定类型
来源：http://xtz.quarkkingdee.top

Py:   except ValueError as e:
来源：http://fek.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eto.yuanzhike.top

JS:   if (e instanceof TypeError) {}
来源：http://nmh.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://ykx.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://rkz.jinqigufen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://csx.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://ord.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jzn.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://jsl.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://noq.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://lxu.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oqc.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://phk.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lxc.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pcp.jinyuanbaomall.cn

Ruby: d&.dig(:a, :b)
来源：http://ykh.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://hig.yangfankeji.com

[H07] 断言
来源：http://yvd.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://jvy.yj20258.top

PHP:  assert($x > 0);
来源：http://xfn.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://btj.sysykeji.top

TS:   console.assert(x > 0);
来源：http://pgx.jqgfzy.top

Java: assert x > 0 : "必须为正";
来源：http://tdh.birdmap.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zds.yj202588.top

Ruby: raise "必须为正" unless x > 0
来源：http://wxh.hysaishi.cn

C#:   Debug.Assert(x > 0);
来源：http://mtr.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://ohk.zhijiandao.cn

Py:   str(e);  traceback.format_exc()
来源：http://cbr.feifeiyinyue.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dtt.zhengqikj.top

JS:   e.message;  e.stack
来源：http://ihg.daxiang520.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://avg.uphjek.com

Java: e.getMessage();  e.printStackTrace()
来源：http://vxs.fzhhl.top

Go:   err.Error()
来源：http://azd.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://jve.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://bbz.chenzaomai.com

[H09] 带错误码的异常
来源：http://qgr.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bix.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://jvc.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ffh.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zfz.haohaochexian.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kye.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wmr.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ars.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uig.jqgfzy.top

[H10] 资源自动释放
来源：http://sgu.zycfv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ttz.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nts.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://clt.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ktq.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iiy.ywan-chungtsiang.top

Go:   defer f.Close()
来源：http://bqj.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jyf.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hho.zhixingplan.top

================================================================================
来源：http://tte.sweek.top

I. 正则表达式
来源：http://tzy.yuanzhike.top

================================================================================
来源：http://cgs.gaohongyu789.top

[I01] 判断是否匹配
来源：http://atc.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://opu.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://pmb.smart0.xyz

JS:   /\d+/.test(s)
来源：http://ksh.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://mwl.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dho.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://aqv.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://lxc.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pjf.tian-w.cn

[I02] 提取所有匹配
来源：http://rwo.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://mdq.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eob.cashguo.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zim.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://zxl.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://slp.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ugu.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://mln.yanxiufei.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://osc.yfazqb.com

[I03] 提取捕获分组
来源：http://xvm.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lhy.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tpz.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://opi.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nsm.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://grz.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qxz.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ygz.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wzb.316326.xyz

[I04] 正则替换
来源：http://yra.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://sqn.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pva.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zlp.shzxlz.cn

TS:   s.replace(/\d+/g, "#")
来源：http://scs.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://bvi.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eou.zhixingplan.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zrq.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zcm.yj202588.top

[I05] 按正则拆分
来源：http://sfy.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ydl.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pzd.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://fll.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://jyn.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://mmk.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yjp.daria6918.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bro.cucudq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cpa.bbcook.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pdc.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ddq.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jmo.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dbt.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zlm.yfazqb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://clb.andypj.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hnr.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qkn.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mmx.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://fce.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rlw.0kj1m.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nvx.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gmu.dashuyun.cn

TS:   /error/gim
来源：http://nha.cucudq.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dau.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lvk.nanxinkj.top

Ruby: s.scan(/error/i)
来源：http://otn.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://myy.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://ljk.nanxuanxn.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bhu.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lde.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lon.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hhc.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ckr.smart0.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zru.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cfb.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zci.zycfv.cn

================================================================================
来源：http://aey.c1oappe.top

J. 日期与时间
来源：http://hpf.zhaomingkeji.xyz

================================================================================
来源：http://dck.tianlin.xyz

[J01] 获取当前时间
来源：http://gqe.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://crg.shanyushiyangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hsn.hesvh.cn

JS:   new Date();  Date.now()
来源：http://zex.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://bzp.hnxiangtu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kjp.smart0.xyz

Go:   time.Now()
来源：http://cuq.jinyuanbaomall.cn

Ruby: Time.now
来源：http://oqc.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://amy.zhongyouzk.top

[J02] 格式化输出
来源：http://ycm.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gom.zhongyouzk.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qlu.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dlz.cheryme.top

TS:   d.toISOString()
来源：http://mqi.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hil.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gnb.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxv.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bul.xziqi.cn

[J03] 字符串解析为日期
来源：http://zif.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lkx.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dth.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://jur.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://fmd.ppjwa.cn

Java: LocalDate.parse("2024-01-02")
来源：http://arw.yuxming.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wfw.chenzaomai.com

Ruby: Date.parse("2024-01-02")
来源：http://shq.jinqigufen.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://icz.cucudq.cn

[J04] 时间戳与日期互转
来源：http://sci.sysykeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nti.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nur.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ywk.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wbn.hesvh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lxk.sjlbkw.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vmt.bbcook.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://opr.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ion.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://zzt.9152youxi.cn

Py:   now + timedelta(days=7)
来源：http://vip.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vwi.jianghu66.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aqg.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://njj.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://fqw.nanxuanxn.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iqg.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://wkn.yueranfly.top

C#:   DateTime.Now.AddDays(7)
来源：http://wsc.chenlongwang.top

[J06] 计算两时间之差
来源：http://mef.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://csb.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://kjy.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dnn.yfazqb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://syp.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ktz.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://azk.hfpthk.cn

Ruby: end - start                 # 返回秒数
来源：http://qdw.yj20258.top

C#:   (end - start).TotalSeconds
来源：http://ivh.smart0.xyz

[J07] 比较两个日期
来源：http://ddk.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://pjl.daxiang520.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mhf.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://ymd.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rte.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://idb.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://emt.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://dkf.zhijiandao.cn

C#:   d1 < d2;  d1 == d2
来源：http://ozv.mhx1999.top

[J08] 提取年月日与星期
来源：http://jft.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bww.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rjf.tianlin.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://phk.yangfankeji.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pnp.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jsg.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://adi.iojbl.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://phu.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pnn.yuxming.cn

[J09] 时区处理
来源：http://nwa.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://num.ivvv.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jby.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ppj.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ixi.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mcj.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://evn.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wzz.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pxs.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://rjx.birdmap.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jwj.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fkr.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rqy.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lce.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzv.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tcv.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hbm.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cpo.zycfv.cn

================================================================================
来源：http://fay.c1oappe.top

K. JSON 与序列化
来源：http://kdn.ppjwa.cn

================================================================================
来源：http://ijy.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://yjk.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aft.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qdg.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://zby.cheryme.top

TS:   JSON.stringify(obj)
来源：http://cbd.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lbx.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://qng.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://eot.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://glr.52xcode.cn

[K02] JSON 字符串转对象
来源：http://qsv.yj20258.top

Py:   json.loads(s)
来源：http://yot.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lwy.tarul.cn

JS:   JSON.parse(s)
来源：http://dom.tianlin.xyz

TS:   JSON.parse(s)
来源：http://ubd.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zfc.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://mfi.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://vec.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdu.shzxlz.cn

[K03] JSON 美化输出（带缩进）
来源：http://dxb.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yot.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ukg.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gyr.chenlongwang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tak.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yan.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wvg.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://dhp.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ppn.fengsongda.top

[K04] 读取 JSON 文件
来源：http://paq.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lmt.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ocp.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wro.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qvj.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gic.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wna.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cxe.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sfp.zhongyouzk.top

[K05] 深拷贝对象
来源：http://kwm.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://miy.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://uss.nanxuanxn.top

JS:   structuredClone(obj)
来源：http://fvx.iojbl.cn

TS:   structuredClone(obj)
来源：http://kjt.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mtn.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://czd.daxiang520.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xdf.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vxh.daria6918.cn

[K06] 解析 URL 查询串
来源：http://vvp.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lhh.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ife.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftw.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nds.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ejf.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://ahs.yj202588.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nxc.zhaomingkeji.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wpp.ppjwa.cn

[K07] 进制转换
来源：http://brg.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jcp.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://une.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cwu.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wlq.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gyc.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wgf.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rjb.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tbn.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://qqx.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://flc.jyoumei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lad.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://ekm.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://dlr.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bkn.yuanzhike.top

Go:   encoding/gob
来源：http://tkd.jinqigfzy.top

Ruby: Marshal.dump(obj)
来源：http://ndy.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gmo.redwolf501.top

================================================================================
来源：http://bvx.yvedp.cn


<!-- 参考信息 -->