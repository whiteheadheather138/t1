代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://axk.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://eue.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://quu.ppjwa.cn

C#:   obj?.A?.B ?? default
来源：http://wch.ppjwa.cn

[H07] 断言
来源：http://byq.hnqzz.top

Py:   assert x > 0, "必须为正"
来源：http://oxf.jinghuilouyu.cn

PHP:  assert($x > 0);
来源：http://xoj.tanke756.top

JS:   console.assert(x > 0);
来源：http://nuv.tian-w.cn

TS:   console.assert(x > 0);
来源：http://zdu.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://mmj.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jvy.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://jxy.shanyushiyangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://dpi.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://ypj.ywan-chungtsiang.top

Py:   str(e);  traceback.format_exc()
来源：http://suh.nwbrower.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nzq.ppjwa.cn

JS:   e.message;  e.stack
来源：http://qsy.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://yah.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pwc.yj202588.top

Go:   err.Error()
来源：http://yus.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://ewm.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://pyi.aizwys.cn

[H09] 带错误码的异常
来源：http://wrk.cheryme.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://atr.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nke.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yqn.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ilb.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ndf.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rdv.jinghuilouyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hpd.hfpthk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://edz.daxiang520.top

[H10] 资源自动释放
来源：http://lei.bjfxy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fzk.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zxt.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vcu.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iql.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yvt.bbcook.cn

Go:   defer f.Close()
来源：http://utv.sweek.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://roh.jlsjyb.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xoy.andypj.xyz

================================================================================
来源：http://vbf.yuanzhike.top

I. 正则表达式
来源：http://cqs.gaohongyu789.top

================================================================================
来源：http://rvy.iojbl.cn

[I01] 判断是否匹配
来源：http://fom.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rta.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://euu.hnqzz.top

JS:   /\d+/.test(s)
来源：http://pzs.xylfe.cn

TS:   /\d+/.test(s)
来源：http://vdn.hammf.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dyr.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://toa.redwolf501.top

Ruby: s.match?(/\d+/)
来源：http://bpo.dianchejie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zmr.iojbl.cn

[I02] 提取所有匹配
来源：http://gfg.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://yvr.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://azn.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mhc.shuidangran.top

TS:   s.match(/\d+/g)
来源：http://iee.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ycz.zdbjq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hxs.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://vpy.daxiang520.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://asy.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://yen.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ztd.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vuy.yj20258888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vzb.xylfe.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://efr.yueranfly.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://afk.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wac.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dfl.tian-w.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ipn.vqdsnc.cn

[I04] 正则替换
来源：http://igz.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xkr.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ibw.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://oqo.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://aql.zhongyouzk.top

Java: s.replaceAll("\\d+", "#")
来源：http://csf.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ejt.tarul.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wpk.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tjg.wangdashe.top

[I05] 按正则拆分
来源：http://qna.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://lqi.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xer.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://ebm.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://hrc.smart0.xyz

Java: s.split("\\s*,\\s*")
来源：http://yft.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jdv.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://mgr.haohaochexian.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bov.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hyo.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dyt.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nwm.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdx.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://myd.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hvp.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rtr.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://stt.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://san.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://wki.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tjm.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gor.sufxvd.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jda.xinyue.icu

TS:   /error/gim
来源：http://qqe.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jwi.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pne.birdmap.top

Ruby: s.scan(/error/i)
来源：http://ghj.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ydh.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://hpp.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kxy.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aqc.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wha.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tqo.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zew.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fqz.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbu.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pqx.yongpay.top

================================================================================
来源：http://pfj.shzxlz.cn

J. 日期与时间
来源：http://fdm.ydzc1.top

================================================================================
来源：http://sug.daria6918.cn

[J01] 获取当前时间
来源：http://qir.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://seh.tanke756.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dnb.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://qrd.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://bhf.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://war.shzxlz.cn

Go:   time.Now()
来源：http://ljp.sjlbkw.cn

Ruby: Time.now
来源：http://nen.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qdz.sxryk.cn

[J02] 格式化输出
来源：http://iyj.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mwm.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kcv.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cuw.mhx1999.top

TS:   d.toISOString()
来源：http://aou.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jsm.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://puc.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jnw.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://doy.chenzaomai.com

[J03] 字符串解析为日期
来源：http://brq.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mcz.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ogd.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://peh.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://wsw.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://fjl.sysykeji.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ssj.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://pds.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cfd.shuidangran.top

[J04] 时间戳与日期互转
来源：http://byr.zhijiandao.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://unc.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aue.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://waw.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jck.yanxiufei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pyg.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gzt.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ufa.guannengcc.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qro.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://elw.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://axp.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://rjh.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqo.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ers.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://cfx.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qxg.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://zym.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://weq.c1oappe.top

[J06] 计算两时间之差
来源：http://lkk.cashguo.top

Py:   (end - start).total_seconds()
来源：http://ebm.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://vpq.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xku.fehbvm.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zld.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hua.fanxiaobao.xyz

Go:   end.Sub(start).Hours()
来源：http://pcp.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://kgs.ctjpmb.com

C#:   (end - start).TotalSeconds
来源：http://bkr.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://ejq.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://dim.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zid.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://dog.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://zsh.xuanzx.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nbo.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ena.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://koh.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://axz.uphjek.com

[J08] 提取年月日与星期
来源：http://kpc.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kif.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wei.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxi.xylfe.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sdc.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://law.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gfv.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hhd.xuanzx.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dfo.9152youxi.cn

[J09] 时区处理
来源：http://tez.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://duj.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zdh.xuanzx.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ono.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eyx.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cly.tanke756.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bfe.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://mcm.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nzw.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://ild.zycfv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ehc.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uli.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://teq.hnxiangtu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksp.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yib.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yih.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nxo.tanke756.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wrv.sysykeji.top

================================================================================
来源：http://yyp.chenjidiqi.icu

K. JSON 与序列化
来源：http://ggv.dashuyun.cn

================================================================================
来源：http://yge.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://wmw.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aci.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ngg.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://nlk.cucudq.cn

TS:   JSON.stringify(obj)
来源：http://mjr.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yjh.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://hmu.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://zmi.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dkl.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://dmm.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://lsh.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cnc.shuidangran.top

JS:   JSON.parse(s)
来源：http://wov.bjfxy.top

TS:   JSON.parse(s)
来源：http://yvd.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://okn.jqgufenzy.top

Go:   json.Unmarshal(data, &v)
来源：http://lyl.daxiang520.top

Ruby: JSON.parse(s)
来源：http://heq.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://del.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://shw.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wra.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nvh.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mqa.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://odi.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ntq.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cta.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://wjp.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nxr.pycfn.com

[K04] 读取 JSON 文件
来源：http://wqf.smart0.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oil.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://udv.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zen.yfazqb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ktc.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://owt.jqgfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://flv.xuetiantiany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://sxs.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lyx.nanxinkj.top

[K05] 深拷贝对象
来源：http://lye.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://tek.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://pha.tarul.cn

JS:   structuredClone(obj)
来源：http://wau.zdqjudy.top

TS:   structuredClone(obj)
来源：http://mql.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wji.fehbvm.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cjl.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ujs.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://zth.hnqzz.top

[K06] 解析 URL 查询串
来源：http://bgg.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://syb.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eje.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jgt.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rdl.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uub.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bmi.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ohd.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lrq.dianchejie.cn

[K07] 进制转换
来源：http://bge.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://crl.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iua.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vbw.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://smp.hcnkem.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mhn.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rhy.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cxi.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eun.shuidangran.top

[K08] 二进制序列化（非 JSON）
来源：http://qow.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://atn.vqdsnc.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vrn.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://qir.zhijiandao.cn

TS:   v8.serialize(obj)        // Node
来源：http://rpo.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xik.vqdsnc.cn

Go:   encoding/gob
来源：http://mjm.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://mkj.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vkr.epnwcf.com

================================================================================
来源：http://ktg.zhixingplan.top

L. 网络请求
来源：http://jhf.guannengcc.top

================================================================================
来源：http://bgo.ydzc1.top

[L01] 发送 GET 请求
来源：http://oes.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mwj.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://odh.tianlin.xyz

JS:   await fetch(url)
来源：http://hug.vehdjk.com

TS:   await fetch(url)
来源：http://bmq.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lcg.hongshengwenyu.top

Go:   resp, err := http.Get(url)
来源：http://kkp.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://wrd.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oyp.xinyue.icu

[L02] 发送 POST JSON
来源：http://qwf.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://fji.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kfh.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tgz.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aya.kuanghao11.cn


<!-- 参考信息 -->