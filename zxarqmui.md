代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mxa.birdmap.top

JS:   if (e instanceof TypeError) {}
来源：http://ewg.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://ilv.hnqzz.top

Java: catch (IOException | SQLException e) {}
来源：http://xco.wangdashe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dzs.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://gvy.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mpn.guannengcc.top

[H06] 可选值 / 空值安全访问
来源：http://bim.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://sqi.hysaishi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://aog.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zzq.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://qok.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bgo.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tww.smart0.xyz

Ruby: d&.dig(:a, :b)
来源：http://qxu.nanxuanxn.top

C#:   obj?.A?.B ?? default
来源：http://wzx.havefunace.top

[H07] 断言
来源：http://zcy.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://mgz.fktsv.cn

PHP:  assert($x > 0);
来源：http://oiq.bbcook.cn

JS:   console.assert(x > 0);
来源：http://czz.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://msb.hesvh.cn

Java: assert x > 0 : "必须为正";
来源：http://hbq.daria6918.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wvn.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gvq.jinqigfzy.top

C#:   Debug.Assert(x > 0);
来源：http://qsb.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://ywo.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://nhz.jqgfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sgw.bjfxy.top

JS:   e.message;  e.stack
来源：http://cmn.fengsongda.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://yhd.kuanghao11.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gga.hywenlv.cn

Go:   err.Error()
来源：http://gok.yj202588.top

Ruby: e.message;  e.backtrace
来源：http://ypo.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://pvx.hesvh.cn

[H09] 带错误码的异常
来源：http://oox.ywan-chungtsiang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cax.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hph.jyoumei.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cty.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ehh.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dym.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ood.yangfankeji.com

Ruby: raise MyError.new("fail", 500)
来源：http://evn.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fcz.zhoulong.xyz

[H10] 资源自动释放
来源：http://cpo.zhoulong.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://wxu.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://atn.tian-w.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xum.quarkkingdee.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fag.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xut.zhijiandao.cn

Go:   defer f.Close()
来源：http://sgh.cdnleiting.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pyr.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kku.yangfankeji.com

================================================================================
来源：http://bgi.yueranfly.top

I. 正则表达式
来源：http://qlq.vehdjk.com

================================================================================
来源：http://lyi.pycfn.com

[I01] 判断是否匹配
来源：http://rig.hnqzz.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pwv.jqgufenzy.top

PHP:  preg_match('/\d+/', $s);
来源：http://lia.gotoacloud.top

JS:   /\d+/.test(s)
来源：http://jus.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://xck.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pcc.guowangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pgy.zhixingplan.top

Ruby: s.match?(/\d+/)
来源：http://lel.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qtc.aibaodan.cn

[I02] 提取所有匹配
来源：http://umo.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://mng.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zmk.ctjpmb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://his.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://knh.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hha.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ele.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://ykl.snrcjt.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qob.jiagoushi.top

[I03] 提取捕获分组
来源：http://bat.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cwz.hcnkem.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://boj.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://roc.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nls.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sjj.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dmn.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qfc.cucudq.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cid.hesvh.cn

[I04] 正则替换
来源：http://ghy.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yph.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lcn.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://pfh.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tza.vqdsnc.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bne.jyoumei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ckl.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pts.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jqo.fehbvm.com

[I05] 按正则拆分
来源：http://uwp.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jmi.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zfm.9152youxi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ynm.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://rwl.guannengcc.top

Java: s.split("\\s*,\\s*")
来源：http://oox.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://etj.tianlin.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://qvt.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jjf.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wjp.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wtk.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qtv.shzxlz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dru.svipenyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fse.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fiq.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kff.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dez.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://msu.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://dzz.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eni.yuanzhike.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ilq.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lfw.aizwys.cn

TS:   /error/gim
来源：http://fac.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cgm.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fuh.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://dwt.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://szk.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://ivt.gogol.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nqo.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dbl.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dms.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lbi.hysaishi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kja.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xwt.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vdl.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xwt.yvedp.cn

================================================================================
来源：http://ujh.bbcook.cn

J. 日期与时间
来源：http://oqv.jinghuilouyu.cn

================================================================================
来源：http://hvp.c1oappe.top

[J01] 获取当前时间
来源：http://gft.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ylh.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jms.epnwcf.com

JS:   new Date();  Date.now()
来源：http://ytm.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://eaz.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://she.fanxiaobao.xyz

Go:   time.Now()
来源：http://nyd.pengpengdd.cyou

Ruby: Time.now
来源：http://lze.yonumen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tln.xylfe.cn

[J02] 格式化输出
来源：http://pbt.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ruj.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mlf.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zzq.9152youxi.cn

TS:   d.toISOString()
来源：http://hpv.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://izy.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yfa.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ztx.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nfz.ctjpmb.com

[J03] 字符串解析为日期
来源：http://qcp.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qtr.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wea.hammf.cn

JS:   new Date("2024-01-02")
来源：http://utg.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://edn.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bkf.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kpu.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://cru.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ouw.yj20258.top

[J04] 时间戳与日期互转
来源：http://trp.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jfr.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ykg.sysykeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hvl.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qor.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ezd.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rbm.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rhr.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ldg.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://svw.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://wlf.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fbo.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qud.sjlbkw.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kdz.9152youxi.cn

Java: LocalDate.now().plusDays(7)
来源：http://npe.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hav.xinyue.icu

Ruby: Time.now + 7 * 86400
来源：http://lmv.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://uqi.daxiang520.top

[J06] 计算两时间之差
来源：http://ncb.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://vbj.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://yzd.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://maw.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gwc.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://uyg.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://cgj.yj20258888.top

Ruby: end - start                 # 返回秒数
来源：http://gec.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://ppw.yanxiufei.cn

[J07] 比较两个日期
来源：http://aqs.yuanzhike.top

Py:   d1 < d2;  d1 == d2
来源：http://arb.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ypa.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://mca.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://svx.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dht.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jnz.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://qbs.zdbjq.cn

C#:   d1 < d2;  d1 == d2
来源：http://hxz.yj202588.top

[J08] 提取年月日与星期
来源：http://qii.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iun.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wce.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cae.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hke.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://osj.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pzg.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tfc.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wmg.iojbl.cn

[J09] 时区处理
来源：http://qhw.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zsu.sufxvd.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vwv.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lve.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ngn.shanyushiyangtech.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dsx.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gfz.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nwz.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hht.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://wdl.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lpl.jiagoushi.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jyr.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hns.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zoa.zhixingplan.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zlk.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hoj.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uts.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ipz.ivvv.top

================================================================================
来源：http://ugd.havefunace.top

K. JSON 与序列化
来源：http://zmy.cheryme.top

================================================================================
来源：http://mzb.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://kkt.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oer.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ppr.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://tnr.hammf.cn

TS:   JSON.stringify(obj)
来源：http://jng.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://elf.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://smc.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://udc.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tgf.nwbrower.top

[K02] JSON 字符串转对象
来源：http://vte.jinqigufen.top

Py:   json.loads(s)
来源：http://zwz.ydzc1.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bke.redwolf501.top

JS:   JSON.parse(s)
来源：http://ugv.meibo888.top

TS:   JSON.parse(s)
来源：http://qeg.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hhx.bjfxy.top

Go:   json.Unmarshal(data, &v)
来源：http://ixc.andypj.xyz

Ruby: JSON.parse(s)
来源：http://xgz.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ois.epnwcf.com

[K03] JSON 美化输出（带缩进）
来源：http://xpv.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hva.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hry.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mcy.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rau.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uql.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lci.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pna.jyoumei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nol.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://gka.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ibw.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hss.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ois.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buo.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kcb.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nhg.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lje.cqqwz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vje.jianghu66.top

[K05] 深拷贝对象
来源：http://ono.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://ezn.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://zps.yfazqb.com

JS:   structuredClone(obj)
来源：http://zbi.guowangkeji.top

TS:   structuredClone(obj)
来源：http://zxr.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dag.nanxinkj.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://upn.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oen.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://rmi.nwbrower.top

[K06] 解析 URL 查询串
来源：http://spu.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://swv.daxiang520.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tam.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ogl.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smf.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzx.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjw.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rnr.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jkm.jianghu66.top

[K07] 进制转换
来源：http://jsv.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wuf.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zbu.chenjidiqi.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pog.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://utp.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qkn.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://psz.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zve.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gqg.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fvq.ctjpmb.com

Py:   pickle.dumps(obj)
来源：http://qbn.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fnk.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://lzs.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://nkk.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lyp.andypj.xyz

Go:   encoding/gob
来源：http://ysx.jianghu66.top

Ruby: Marshal.dump(obj)
来源：http://qwe.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hck.andypj.xyz

================================================================================
来源：http://nfs.birdmap.top

L. 网络请求
来源：http://guv.cdnleiting.top

================================================================================
来源：http://vzl.fengsongda.top

[L01] 发送 GET 请求
来源：http://nsj.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fhh.zhixingplan.top


<!-- 参考信息 -->