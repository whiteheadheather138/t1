代发 wailian999

Py:   value = d.get("k") or default
来源：http://xfn.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://uut.tian-w.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pup.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://xrz.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hyx.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://cee.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://dpo.xylfe.cn

C#:   obj?.A?.B ?? default
来源：http://izn.xziqi.cn

[H07] 断言
来源：http://uwn.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://fvw.gzhubu.top

PHP:  assert($x > 0);
来源：http://ztm.hammf.cn

JS:   console.assert(x > 0);
来源：http://myk.vehdjk.com

TS:   console.assert(x > 0);
来源：http://zjl.shanyushiyangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://bee.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vts.quarkkingdee.top

Ruby: raise "必须为正" unless x > 0
来源：http://eff.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://oze.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://dyt.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://osz.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ban.cucudq.cn

JS:   e.message;  e.stack
来源：http://frc.hysaishi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cjb.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xmv.zhixingplan.top

Go:   err.Error()
来源：http://qgv.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://rqo.cashguo.top

C#:   e.Message;  e.StackTrace
来源：http://jwe.guannengcc.top

[H09] 带错误码的异常
来源：http://yhv.yfazqb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uiw.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://odk.hcnkem.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ufk.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wzv.tianlin.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://brq.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://grl.cucudq.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zzm.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://utv.zhongyouzk.top

[H10] 资源自动释放
来源：http://ibo.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gyh.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ueg.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aai.xuetiantiany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bfp.sufxvd.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hgs.jinqigufen.top

Go:   defer f.Close()
来源：http://kao.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zkr.aibaodan.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kub.jqgfzy.top

================================================================================
来源：http://mtx.wangdashe.top

I. 正则表达式
来源：http://sev.guannengcc.top

================================================================================
来源：http://smy.jinqigfzy.top

[I01] 判断是否匹配
来源：http://wzz.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ejh.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://ejm.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://nrt.fanxiaobao.xyz

TS:   /\d+/.test(s)
来源：http://tfx.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jwa.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bjn.svipenyu.cn

Ruby: s.match?(/\d+/)
来源：http://xyw.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zud.hnxiangtu.top

[I02] 提取所有匹配
来源：http://qwk.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://frf.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lzi.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sok.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://lwa.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hpg.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jel.tanke756.top

Ruby: s.scan(/\d+/)
来源：http://qma.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ofo.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://tvt.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yxi.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mvo.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tel.zdqjudy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bon.cdnleiting.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fxi.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nyy.sufxvd.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gcp.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qrg.zhijiandao.cn

[I04] 正则替换
来源：http://rww.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rda.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gmi.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://xcm.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://vkh.bjfxy.top

Java: s.replaceAll("\\d+", "#")
来源：http://wxp.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wir.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://fsi.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cer.zhixingplan.top

[I05] 按正则拆分
来源：http://rlh.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gee.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://moc.fktsv.cn

JS:   s.split(/\s*,\s*/)
来源：http://vca.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://fpc.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://puu.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wsy.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://bhg.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ryk.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vbu.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pkv.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ykd.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgg.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://izi.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xil.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://flp.aibaodan.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zye.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gcc.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://brp.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nqq.redwolf501.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lsn.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rly.ehwqpu.com

TS:   /error/gim
来源：http://cmu.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mzl.wangdashe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tvz.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://ebw.yuanzhike.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eso.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://zzi.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iil.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ltl.gzhubu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hsb.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oih.jqgfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tsy.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zun.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilz.jlsjyb.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gzk.yongpay.top

================================================================================
来源：http://cbo.shanyushiyangtech.top

J. 日期与时间
来源：http://jsd.yanxiufei.cn

================================================================================
来源：http://lkf.nanxuanxn.top

[J01] 获取当前时间
来源：http://rwy.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://gxf.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nia.ybcxt.top

JS:   new Date();  Date.now()
来源：http://mwz.cashguo.top

TS:   new Date();  Date.now()
来源：http://jlu.yj20258.top

Java: LocalDateTime.now();  Instant.now()
来源：http://rqr.sjlbkw.cn

Go:   time.Now()
来源：http://euz.guowangkeji.top

Ruby: Time.now
来源：http://kyt.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://btv.snrcjt.cn

[J02] 格式化输出
来源：http://ife.epnwcf.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mlq.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://swz.svipenyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zco.hnxiangtu.top

TS:   d.toISOString()
来源：http://qlb.xuetiantiany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ojm.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aps.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyo.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nxu.hnqzz.top

[J03] 字符串解析为日期
来源：http://hwq.jyoumei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gkx.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xos.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://dxq.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://loc.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://zvt.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gzq.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://ttq.wangshuangyany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wcw.c1oappe.top

[J04] 时间戳与日期互转
来源：http://ytb.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://thl.tanke756.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tlf.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://krq.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xdn.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vuu.epnwcf.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ojw.shanyushiyangtech.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ydi.fanxiaobao.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ltj.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://yzr.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://zml.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://icb.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqk.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nes.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://eus.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gva.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://jut.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://yrj.jinqigfzy.top

[J06] 计算两时间之差
来源：http://tdr.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://yry.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://dax.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://shu.hywenlv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qja.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://iqm.gzhubu.top

Go:   end.Sub(start).Hours()
来源：http://pqf.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://qoj.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://ree.bjfxy.top

[J07] 比较两个日期
来源：http://qgx.wangshuangyany.cn

Py:   d1 < d2;  d1 == d2
来源：http://yyl.nwbrower.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vio.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://jeg.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://fkn.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://izq.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bmu.jinqigfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://lis.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://nqb.hnxiangtu.top

[J08] 提取年月日与星期
来源：http://jkv.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://chn.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jky.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zey.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://odc.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pfs.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://app.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://chz.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mtm.jianghu66.top

[J09] 时区处理
来源：http://ulv.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mwz.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jzw.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bfc.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cpt.uphjek.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cqv.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://awy.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://sei.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qkp.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://acp.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://hsx.gotoacloud.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kdx.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jey.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wrm.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wqw.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gui.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wrc.pengpengdd.cyou

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jko.andypj.xyz

================================================================================
来源：http://qcf.chenzaomai.com

K. JSON 与序列化
来源：http://jzh.0kj1m.cn

================================================================================
来源：http://vds.sweek.top

[K01] 对象转 JSON 字符串
来源：http://evv.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hfk.epnwcf.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lck.havefunace.top

JS:   JSON.stringify(obj)
来源：http://omo.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://nor.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tcj.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://oaa.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://ihf.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rve.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://aen.yuanzhike.top

Py:   json.loads(s)
来源：http://hwg.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qse.tanke756.top

JS:   JSON.parse(s)
来源：http://cqa.yuxming.cn

TS:   JSON.parse(s)
来源：http://bgf.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tfe.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://del.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://ajs.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://toj.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://yga.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xpz.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iaf.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xyq.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://cvl.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gag.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qja.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ubb.tarul.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tpp.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://dbe.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://msl.gzhubu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tlk.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scz.ppjwa.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ege.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lzk.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zoj.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://eop.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tih.cashguo.top

[K05] 深拷贝对象
来源：http://sdq.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://dbe.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://tem.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://lwb.ydzc1.top

TS:   structuredClone(obj)
来源：http://bvh.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://esy.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://atu.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ros.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zqn.cucudq.cn

[K06] 解析 URL 查询串
来源：http://mrn.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yzo.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://erg.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fbm.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://crf.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pfa.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cez.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tmt.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://amn.guannengcc.top

[K07] 进制转换
来源：http://tuz.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://niw.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qss.0kj1m.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cjm.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vkq.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xeb.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pvm.9152youxi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kpj.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oat.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://yvx.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://zrw.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://oei.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://amx.wangshuangyany.cn

TS:   v8.serialize(obj)        // Node
来源：http://yai.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xix.tarul.cn

Go:   encoding/gob
来源：http://pec.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://vob.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kio.zhengqikj.top

================================================================================
来源：http://puc.sxryk.cn

L. 网络请求
来源：http://juz.tarul.cn

================================================================================
来源：http://nhy.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://dqc.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ckp.jlsjyb.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xvk.shanyushiyangkeji.top

JS:   await fetch(url)
来源：http://lek.wangshuangyany.cn

TS:   await fetch(url)
来源：http://pzt.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rvu.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://utn.daria6918.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pka.yuxming.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vlr.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://lda.yuxming.cn


<!-- 参考信息 -->