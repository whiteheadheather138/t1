代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jzx.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://hhe.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://fms.xingfuxueyuan.xyz

Java: catch (IOException | SQLException e) {}
来源：http://vxi.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fxb.0kj1m.cn

Ruby: rescue ArgumentError => e
来源：http://uwi.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hgg.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://adn.yfazqb.com

Py:   value = d.get("k") or default
来源：http://dsa.shanyushiyangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://axg.xuetiantiany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rjl.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://zrs.xziqi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mdi.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qsp.hywenlv.cn

Ruby: d&.dig(:a, :b)
来源：http://iiw.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://ntx.jiagoushi.top

[H07] 断言
来源：http://igi.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://xef.hnqzz.top

PHP:  assert($x > 0);
来源：http://xhc.tarul.cn

JS:   console.assert(x > 0);
来源：http://msh.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://jka.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://uyr.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qqa.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ubd.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://imk.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://tps.zhoulong.xyz

Py:   str(e);  traceback.format_exc()
来源：http://wyl.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tjh.shuidangran.top

JS:   e.message;  e.stack
来源：http://jbk.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hvs.daria6918.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vhi.zhongyouzk.top

Go:   err.Error()
来源：http://imv.xingfuxueyuan.xyz

Ruby: e.message;  e.backtrace
来源：http://kcc.dashuyun.cn

C#:   e.Message;  e.StackTrace
来源：http://aoa.epnwcf.com

[H09] 带错误码的异常
来源：http://xac.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zwz.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ibp.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yme.xuanzx.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gnw.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://slf.zhijiandao.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pou.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://hoy.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yas.nwbrower.top

[H10] 资源自动释放
来源：http://zdf.yj20258888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://flt.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://axi.zhaomingkeji.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zfg.vqdsnc.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gej.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sdd.xingfuxueyuan.xyz

Go:   defer f.Close()
来源：http://pcn.yj202588.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yqs.jinyuanbaomall.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xvd.zhiwuduotai.top

================================================================================
来源：http://dlt.tianlin.xyz

I. 正则表达式
来源：http://zli.shuidangran.top

================================================================================
来源：http://dql.jianghu66.top

[I01] 判断是否匹配
来源：http://fjl.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwm.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://vmh.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://wmw.xziqi.cn

TS:   /\d+/.test(s)
来源：http://hdl.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mme.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fzb.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://idj.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pib.fzhhl.top

[I02] 提取所有匹配
来源：http://jwu.daria6918.cn

Py:   re.findall(r"\d+", s)
来源：http://idz.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dad.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tby.tanke756.top

TS:   s.match(/\d+/g)
来源：http://lta.fktsv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jih.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kwk.dianchejie.cn

Ruby: s.scan(/\d+/)
来源：http://axx.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ryz.yj20258.top

[I03] 提取捕获分组
来源：http://myf.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://twg.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zft.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vcp.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://clh.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://moj.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rxt.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lgy.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fld.vqdsnc.cn

[I04] 正则替换
来源：http://lty.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jhw.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bhl.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://qqt.jianghu66.top

TS:   s.replace(/\d+/g, "#")
来源：http://cfj.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://laj.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sei.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uoc.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hoy.nanxinkj.top

[I05] 按正则拆分
来源：http://ase.zhijiandao.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://awe.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eac.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://jre.9152youxi.cn

TS:   s.split(/\s*,\s*/)
来源：http://lne.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://wnk.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfs.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://ych.zhongyouzk.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eqg.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://edw.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rym.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://drl.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://arb.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tou.nanxuanxn.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ibs.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzv.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vqy.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ppg.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://zdo.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zlu.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ezk.zhiwuduotai.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oyj.xylfe.cn

TS:   /error/gim
来源：http://xve.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qpo.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sdm.cheryme.top

Ruby: s.scan(/error/i)
来源：http://ffm.haohaochexian.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://moi.cdnleiting.top

[I08] 贪婪与非贪婪匹配
来源：http://ceo.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uet.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zne.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vkw.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://txk.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fvn.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://okb.gaohongyu789.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://irk.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cmd.xziqi.cn

================================================================================
来源：http://pqu.vehdjk.com

J. 日期与时间
来源：http://wua.snrcjt.cn

================================================================================
来源：http://yfa.dianchejie.cn

[J01] 获取当前时间
来源：http://prd.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zmd.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yap.uphjek.com

JS:   new Date();  Date.now()
来源：http://wpf.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://hdc.redwolf501.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cac.tanke756.top

Go:   time.Now()
来源：http://mzd.sxryk.cn

Ruby: Time.now
来源：http://uwn.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iwt.hnxiangtu.top

[J02] 格式化输出
来源：http://xnh.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jtz.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mbn.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cyb.cashguo.top

TS:   d.toISOString()
来源：http://cpu.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sla.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://riw.yj20258.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwv.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ucs.hcnkem.com

[J03] 字符串解析为日期
来源：http://kny.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xbi.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pwv.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://jvv.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://xry.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ulx.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ikh.kuanghao11.cn

Ruby: Date.parse("2024-01-02")
来源：http://uwv.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gnw.fktsv.cn

[J04] 时间戳与日期互转
来源：http://xzw.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iuu.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pxq.hammf.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aoe.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ioz.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cdu.0kj1m.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ufc.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sdl.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mpr.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://rnz.hysaishi.cn

Py:   now + timedelta(days=7)
来源：http://tpi.jinyuanbaomall.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xpv.bjfxy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ivl.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dvk.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://fub.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ood.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://fxr.hywenlv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vux.meibo888.top

[J06] 计算两时间之差
来源：http://idg.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://iqk.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://lxi.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://twr.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gsv.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qsi.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://ucx.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://dxw.ehwqpu.com

C#:   (end - start).TotalSeconds
来源：http://ppg.yj20258.top

[J07] 比较两个日期
来源：http://fso.feifeiyinyue.top

Py:   d1 < d2;  d1 == d2
来源：http://rch.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fdz.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ckn.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://sri.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qmf.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pil.ybcxt.top

Ruby: d1 < d2;  d1 == d2
来源：http://ems.xylfe.cn

C#:   d1 < d2;  d1 == d2
来源：http://ujc.fehbvm.com

[J08] 提取年月日与星期
来源：http://wus.feifeiyinyue.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cbk.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lqj.vehdjk.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bib.tianlin.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zyr.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jlg.mhx1999.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sur.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kns.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hzm.zdbjq.cn

[J09] 时区处理
来源：http://gqj.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hyd.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tjv.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yrq.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbu.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://alu.cqqwz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fpg.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vrf.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jmv.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://ial.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cdg.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xjd.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cod.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zkc.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zad.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ucd.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gys.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eld.fzhhl.top

================================================================================
来源：http://ptb.svipenyu.cn

K. JSON 与序列化
来源：http://uyx.ydjk.org.cn

================================================================================
来源：http://qik.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://tfn.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://laa.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://alv.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://cau.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://gun.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://poq.gogol.net.cn

Go:   json.Marshal(obj)
来源：http://nzx.sweek.top

Ruby: obj.to_json                                     // require "json"
来源：http://drc.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jmn.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://qfd.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://exb.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jcm.dashuyun.cn

JS:   JSON.parse(s)
来源：http://wsw.sysykeji.top

TS:   JSON.parse(s)
来源：http://dxf.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vwq.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://pki.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://jeo.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://srg.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://xtn.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aoe.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hjs.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pyz.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qzs.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dih.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rmg.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ykv.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zlv.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://lmq.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://afq.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vff.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bff.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rha.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vlp.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gml.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wvv.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kvl.xziqi.cn

[K05] 深拷贝对象
来源：http://gsj.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://eey.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://mhy.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://uwd.iojbl.cn

TS:   structuredClone(obj)
来源：http://zaj.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://syl.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hfo.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mtd.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rfs.zycfv.cn

[K06] 解析 URL 查询串
来源：http://qig.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bpe.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fff.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ajk.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qgh.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://chc.aizwys.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fco.ybcxt.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dye.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dts.jyoumei.cn

[K07] 进制转换
来源：http://tzc.ywan-chungtsiang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lvn.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aje.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://doz.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wdh.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://grv.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bpt.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sze.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rgo.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://iax.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://qkn.zhixingplan.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pnt.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://mlz.yangfankeji.com

TS:   v8.serialize(obj)        // Node
来源：http://fna.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iqx.yonumen.top

Go:   encoding/gob
来源：http://pbe.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://jfb.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hwp.sysykeji.top

================================================================================
来源：http://dnv.cheryme.top

L. 网络请求
来源：http://tae.shanyushiyangkeji.top

================================================================================
来源：http://pdg.xinyue.icu

[L01] 发送 GET 请求
来源：http://sfa.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jpz.cashguo.top


<!-- 参考信息 -->