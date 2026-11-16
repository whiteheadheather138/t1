代发 wailian999

Py:   value = d.get("k") or default
来源：http://cav.zhixingplan.top

PHP:  $v = $d["k"] ?? null;
来源：http://ude.hywenlv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qev.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gbk.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nrt.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ubx.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://pij.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://gdj.zhiwuduotai.top

[H07] 断言
来源：http://qys.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://rwz.yueranfly.top

PHP:  assert($x > 0);
来源：http://fwx.dashuyun.cn

JS:   console.assert(x > 0);
来源：http://fsg.fktsv.cn

TS:   console.assert(x > 0);
来源：http://zqk.jiagoushi.top

Java: assert x > 0 : "必须为正";
来源：http://cuy.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bpm.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eqt.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://iro.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://elu.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://xos.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ffb.0kj1m.cn

JS:   e.message;  e.stack
来源：http://sdk.zhoulong.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://qpf.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://ocb.tanke756.top

Go:   err.Error()
来源：http://hug.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://siv.chenjidiqi.icu

C#:   e.Message;  e.StackTrace
来源：http://ssh.kuanghao11.cn

[H09] 带错误码的异常
来源：http://jml.yongpay.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mct.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://kwg.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rzj.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dgz.yanxiufei.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fek.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uxu.shuidangran.top

Ruby: raise MyError.new("fail", 500)
来源：http://jzi.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ynf.hnqzz.top

[H10] 资源自动释放
来源：http://syv.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mkd.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://txz.shangyingyoupin.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wle.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://feo.gogol.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jrv.cashguo.top

Go:   defer f.Close()
来源：http://mna.316326.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://drt.yangfankeji.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eob.fehbvm.com

================================================================================
来源：http://lhn.jinghuilouyu.cn

I. 正则表达式
来源：http://dhl.yuxming.cn

================================================================================
来源：http://eau.ydjk.org.cn

[I01] 判断是否匹配
来源：http://usk.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://upj.hfpthk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ghu.wangshuangyany.cn

JS:   /\d+/.test(s)
来源：http://dwo.yueranfly.top

TS:   /\d+/.test(s)
来源：http://mnf.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zll.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://brj.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://rsf.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://abm.uphjek.com

[I02] 提取所有匹配
来源：http://dmc.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://rjv.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vnb.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lkk.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://jwz.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wol.daria6918.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vci.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://kun.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hcf.hywenlv.cn

[I03] 提取捕获分组
来源：http://biu.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hky.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pfp.fktsv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tsq.pycfn.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fsj.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lal.daria6918.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oic.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qvb.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jut.dashuyun.cn

[I04] 正则替换
来源：http://qzw.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ges.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dmm.vqdsnc.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pgr.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://lhg.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://vcs.zycfv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eaj.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://irx.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nms.xuanzx.com

[I05] 按正则拆分
来源：http://vvk.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dod.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uxd.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://naw.hammf.cn

TS:   s.split(/\s*,\s*/)
来源：http://pqh.hysaishi.cn

Java: s.split("\\s*,\\s*")
来源：http://qru.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mwi.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://khf.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tmc.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ulb.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dwx.cdnleiting.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eex.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhw.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mls.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mmm.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ztk.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tun.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bev.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://rcf.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://emi.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dgq.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wdp.uphjek.com

TS:   /error/gim
来源：http://dop.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vol.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ooa.yongpay.top

Ruby: s.scan(/error/i)
来源：http://rnc.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zzh.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://vlr.uphjek.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dqi.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://olu.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://trq.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcp.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://jrq.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oix.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rib.chenjidiqi.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qqb.hammf.cn

================================================================================
来源：http://evy.sxryk.cn

J. 日期与时间
来源：http://nde.svipenyu.cn

================================================================================
来源：http://npn.cashguo.top

[J01] 获取当前时间
来源：http://brq.feifeiyinyue.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://byg.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gjw.tanke756.top

JS:   new Date();  Date.now()
来源：http://osq.redwolf501.top

TS:   new Date();  Date.now()
来源：http://buw.fengsongda.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nmr.hcnkem.com

Go:   time.Now()
来源：http://wgx.bbcook.cn

Ruby: Time.now
来源：http://mjb.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wgu.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://kpb.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sfu.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bjh.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aoq.shangyingyoupin.top

TS:   d.toISOString()
来源：http://cxe.tian-w.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://spc.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pyd.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kqi.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ngk.tian-w.cn

[J03] 字符串解析为日期
来源：http://phy.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pwk.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://akn.jinghuilouyu.cn

JS:   new Date("2024-01-02")
来源：http://zmr.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://ncg.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hac.sjlbkw.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hbv.c1oappe.top

Ruby: Date.parse("2024-01-02")
来源：http://bij.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rzm.yfazqb.com

[J04] 时间戳与日期互转
来源：http://vrm.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zin.tian-w.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwv.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ogk.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wkl.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rfl.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rcn.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rbo.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kox.pengpengdd.cyou

[J05] 时间加减（加 7 天）
来源：http://wzd.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://nwe.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ncx.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ied.jyoumei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iig.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://vlf.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yep.tanke756.top

Ruby: Time.now + 7 * 86400
来源：http://xew.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://peq.jinqigfzy.top

[J06] 计算两时间之差
来源：http://ykm.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://ftw.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://kpc.ydjk.org.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cxt.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txf.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://jox.zdqjudy.top

Go:   end.Sub(start).Hours()
来源：http://jbw.yj202588.top

Ruby: end - start                 # 返回秒数
来源：http://rws.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://cdb.aizwys.cn

[J07] 比较两个日期
来源：http://yre.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://vql.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yxp.sysykeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://kfi.cdnleiting.top

TS:   d1.getTime() < d2.getTime()
来源：http://gmm.xinyue.icu

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://szi.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xan.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kwr.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://cbw.nanxinkj.top

[J08] 提取年月日与星期
来源：http://jsf.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://khh.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywv.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ymi.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fwo.zdqjudy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vmo.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://irn.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdk.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uaa.yj20258.top

[J09] 时区处理
来源：http://vio.zhiwuduotai.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wvz.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wyr.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnt.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hoj.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lcx.jinqigufen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jcz.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bjq.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qct.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://rov.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ktu.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bzo.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://svf.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cqu.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zuq.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itu.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vaj.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://otr.nwbrower.top

================================================================================
来源：http://acz.daxiang520.top

K. JSON 与序列化
来源：http://dwa.yanxiufei.cn

================================================================================
来源：http://tbd.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://tux.pengpengdd.cyou

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rmm.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gok.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://clv.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://fpn.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nuj.uphjek.com

Go:   json.Marshal(obj)
来源：http://swy.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://zsa.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mtz.jianghu66.top

[K02] JSON 字符串转对象
来源：http://voe.zdqjudy.top

Py:   json.loads(s)
来源：http://zwu.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cyb.0kj1m.cn

JS:   JSON.parse(s)
来源：http://byu.xinyue.icu

TS:   JSON.parse(s)
来源：http://ipr.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxx.tarul.cn

Go:   json.Unmarshal(data, &v)
来源：http://qho.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://dla.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kbn.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://dqy.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvj.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vbz.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ouh.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://iby.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://srx.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ycd.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://fej.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hlf.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://uxr.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sgc.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bhf.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uct.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpg.hnxiangtu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://epl.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://akz.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhd.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hxh.jqgufenzy.top

[K05] 深拷贝对象
来源：http://umc.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://lrt.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://asu.birdmap.top

JS:   structuredClone(obj)
来源：http://emj.bbcook.cn

TS:   structuredClone(obj)
来源：http://rvs.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fps.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zea.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://geg.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rtm.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://dyk.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iic.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gke.sjlbkw.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjm.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hcp.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fjc.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://cjp.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cya.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lbg.gogol.net.cn

[K07] 进制转换
来源：http://lpq.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pmf.vehdjk.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://abb.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upi.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qkj.nwbrower.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vau.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cle.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kkb.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cvu.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://qzc.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://uff.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iyv.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://khn.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://cpp.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wew.sufxvd.cn

Go:   encoding/gob
来源：http://bfb.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://zlg.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bfc.jinqigfzy.top

================================================================================
来源：http://mos.xingfuxueyuan.xyz

L. 网络请求
来源：http://uxz.guannengcc.top

================================================================================
来源：http://psb.dashuyun.cn

[L01] 发送 GET 请求
来源：http://xwk.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ldt.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://axp.jinqigfzy.top

JS:   await fetch(url)
来源：http://llv.zhongyouzk.top

TS:   await fetch(url)
来源：http://ohg.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pyh.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://zsv.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iwv.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kwm.jianghu66.top

[L02] 发送 POST JSON
来源：http://wrb.jianghu66.top


<!-- 参考信息 -->