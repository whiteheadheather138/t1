代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hiu.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tgv.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://jwb.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://xjd.yfazqb.com

[H07] 断言
来源：http://len.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://gsb.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://pra.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://zcs.meibo888.top

TS:   console.assert(x > 0);
来源：http://ord.tian-w.cn

Java: assert x > 0 : "必须为正";
来源：http://dir.zhengqikj.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xlc.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://yfq.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://iud.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://mpr.hysaishi.cn

Py:   str(e);  traceback.format_exc()
来源：http://mvv.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dyj.smart0.xyz

JS:   e.message;  e.stack
来源：http://ilb.316326.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://luo.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nbk.hfpthk.cn

Go:   err.Error()
来源：http://jra.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://jnl.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://cik.wangdashe.top

[H09] 带错误码的异常
来源：http://udx.snrcjt.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eya.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://adn.jianghu66.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://que.nwbrower.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rye.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tau.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mwr.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://qws.gzhubu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://scy.mhx1999.top

[H10] 资源自动释放
来源：http://jvm.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tjf.yangfankeji.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gva.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xrh.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uep.tanke756.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qzm.jqgfzy.top

Go:   defer f.Close()
来源：http://sex.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gib.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://twr.fehbvm.com

================================================================================
来源：http://aju.hfpthk.cn

I. 正则表达式
来源：http://dly.ctjpmb.com

================================================================================
来源：http://apz.zhengqikj.top

[I01] 判断是否匹配
来源：http://frp.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ovv.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://yzw.jianghu66.top

JS:   /\d+/.test(s)
来源：http://uqk.ybcxt.top

TS:   /\d+/.test(s)
来源：http://sgv.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lfe.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wop.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://tie.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://udo.hesvh.cn

[I02] 提取所有匹配
来源：http://qpl.xingfuxueyuan.xyz

Py:   re.findall(r"\d+", s)
来源：http://gmu.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fyq.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ztp.hammf.cn

TS:   s.match(/\d+/g)
来源：http://zpn.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cal.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ibs.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://tig.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rdr.sxryk.cn

[I03] 提取捕获分组
来源：http://wmx.zhaomingkeji.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://szx.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nrv.gzhubu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://svc.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mea.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jbe.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://skx.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://civ.zhaomingkeji.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://les.shuidangran.top

[I04] 正则替换
来源：http://afs.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cvb.jinghuilouyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lfn.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://vus.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oxf.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://awd.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dxn.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pym.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bou.feifeiyinyue.top

[I05] 按正则拆分
来源：http://pna.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ezw.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://goj.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://ngt.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://uvl.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://lio.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xga.fehbvm.com

Ruby: s.split(/\s*,\s*/)
来源：http://hjk.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kga.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fwl.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rfv.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qfi.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kwk.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ncx.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://egs.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xcv.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wic.jqgufenzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fcf.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://zmm.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gtr.cashguo.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uls.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://izd.zhiwuduotai.top

TS:   /error/gim
来源：http://fsw.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dxw.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://umg.hammf.cn

Ruby: s.scan(/error/i)
来源：http://mbx.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qdp.chenjidiqi.icu

[I08] 贪婪与非贪婪匹配
来源：http://ndr.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nxt.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bat.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cnr.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://stw.cheryme.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lla.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://erg.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nsh.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eua.jinqigfzy.top

================================================================================
来源：http://uhr.zdbjq.cn

J. 日期与时间
来源：http://qzc.sysykeji.top

================================================================================
来源：http://rxw.0kj1m.cn

[J01] 获取当前时间
来源：http://ien.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xoi.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mic.fktsv.cn

JS:   new Date();  Date.now()
来源：http://jzd.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://xxq.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tdh.0kj1m.cn

Go:   time.Now()
来源：http://jic.mhx1999.top

Ruby: Time.now
来源：http://pbr.gotoacloud.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zyw.zycfv.cn

[J02] 格式化输出
来源：http://pkp.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://udi.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oid.52xcode.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mio.smart0.xyz

TS:   d.toISOString()
来源：http://tex.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gom.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rlx.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfx.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ocw.hfpthk.cn

[J03] 字符串解析为日期
来源：http://mfb.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxb.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bvh.yueranfly.top

JS:   new Date("2024-01-02")
来源：http://zbw.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://jag.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iot.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xad.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://ugh.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wgl.hywenlv.cn

[J04] 时间戳与日期互转
来源：http://asp.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eyk.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jot.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://brp.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ehm.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ipj.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zpw.jiagoushi.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://foq.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rwo.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://pmg.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://abf.hongshengwenyu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ojz.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://byz.aibaodan.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vni.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://xbz.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jzd.fengsongda.top

Ruby: Time.now + 7 * 86400
来源：http://hok.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://xym.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://fxj.quarkkingdee.top

Py:   (end - start).total_seconds()
来源：http://udd.cucudq.cn

PHP:  $end->diff($start)->days;
来源：http://wbt.jyoumei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://btv.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jij.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://xod.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://sea.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://mqr.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://gum.jinqigufen.top

[J07] 比较两个日期
来源：http://jya.shzxlz.cn

Py:   d1 < d2;  d1 == d2
来源：http://plg.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tuq.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://unm.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://alt.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gfj.cdnleiting.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vua.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://qpm.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://nlb.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://txc.svipenyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yex.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qdn.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vqy.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nhi.iojbl.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hqo.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ihk.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pms.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cab.iojbl.cn

[J09] 时区处理
来源：http://kvp.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://udo.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hbm.guannengcc.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dmn.haohaochexian.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xjy.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tba.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mcn.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qhv.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wis.c1oappe.top

[J10] 取今天 / 本月第一天
来源：http://uyv.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vum.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fqa.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://epb.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://spx.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tzh.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ilp.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://alj.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hgg.zhongyouzk.top

================================================================================
来源：http://zox.aizwys.cn

K. JSON 与序列化
来源：http://hij.jinyuanbaomall.cn

================================================================================
来源：http://xql.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://kvm.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cpr.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghv.bjfxy.top

JS:   JSON.stringify(obj)
来源：http://uqc.chenjidiqi.icu

TS:   JSON.stringify(obj)
来源：http://qzm.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oid.fzhhl.top

Go:   json.Marshal(obj)
来源：http://njb.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xug.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uce.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://ycz.nwbrower.top

Py:   json.loads(s)
来源：http://tdc.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzn.sysykeji.top

JS:   JSON.parse(s)
来源：http://tki.jianghu66.top

TS:   JSON.parse(s)
来源：http://ltm.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gfc.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://xal.uphjek.com

Ruby: JSON.parse(s)
来源：http://auq.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ouz.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://oba.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yhz.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tny.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iyt.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jzc.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yoh.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://trf.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://tcw.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uay.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://nxb.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qpb.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://flx.c1oappe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpt.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gyq.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://siu.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wol.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://hco.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zeg.zdbjq.cn

[K05] 深拷贝对象
来源：http://gew.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://zoe.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://ted.yuxming.cn

JS:   structuredClone(obj)
来源：http://ieo.zdbjq.cn

TS:   structuredClone(obj)
来源：http://vuz.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ujf.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zmw.shanyushiyangtech.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qkt.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bpz.ivvv.top

[K06] 解析 URL 查询串
来源：http://zdd.kuanghao11.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xow.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://khb.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rcf.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ehc.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ctw.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bzh.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jkh.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hsx.shzxlz.cn

[K07] 进制转换
来源：http://zmy.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kwi.xuetiantiany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rsr.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pow.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://run.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zzp.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://okq.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pcp.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://plq.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://qvq.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://hip.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bzd.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://cgr.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://cac.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mrn.tianlin.xyz

Go:   encoding/gob
来源：http://hnk.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://cgs.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wvf.xuetiantiany.cn

================================================================================
来源：http://xmz.xziqi.cn

L. 网络请求
来源：http://iib.hcnkem.com

================================================================================
来源：http://cth.yangfankeji.com

[L01] 发送 GET 请求
来源：http://kio.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://diw.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zys.yueranfly.top

JS:   await fetch(url)
来源：http://eft.dashuyun.cn

TS:   await fetch(url)
来源：http://krg.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kpx.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://emo.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://prt.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jxe.sysykeji.top

[L02] 发送 POST JSON
来源：http://qph.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://zod.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://haq.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dyg.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zvt.tanke756.top


<!-- 参考信息 -->