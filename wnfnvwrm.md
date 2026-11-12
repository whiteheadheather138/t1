代发 wailian999

Py:   value = d.get("k") or default
来源：http://egy.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://yqr.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://cam.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://zvm.xylfe.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wkx.fktsv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qbk.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://lxg.zhoulong.xyz

C#:   obj?.A?.B ?? default
来源：http://xct.svipenyu.cn

[H07] 断言
来源：http://oab.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://jfi.yj202588.top

PHP:  assert($x > 0);
来源：http://jhs.shangyingyoupin.top

JS:   console.assert(x > 0);
来源：http://dzi.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://ili.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://rjo.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eud.jinyuanbaomall.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zou.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://lrb.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://stv.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://fte.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kqp.gotoacloud.top

JS:   e.message;  e.stack
来源：http://enm.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://dbv.zhaomingkeji.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ops.yonumen.top

Go:   err.Error()
来源：http://mik.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://who.hnxiangtu.top

C#:   e.Message;  e.StackTrace
来源：http://mxq.cdnleiting.top

[H09] 带错误码的异常
来源：http://qgb.hnxiangtu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://snr.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qeq.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ssg.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nyl.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://snd.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tya.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xsy.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://may.zycfv.cn

[H10] 资源自动释放
来源：http://xqv.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vhi.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zct.zhijiandao.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxe.jinyuanbaomall.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pwn.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lky.quarkkingdee.top

Go:   defer f.Close()
来源：http://kip.xylfe.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oql.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdq.sweek.top

================================================================================
来源：http://obi.mhx1999.top

I. 正则表达式
来源：http://jlb.jinqigufen.top

================================================================================
来源：http://mph.xziqi.cn

[I01] 判断是否匹配
来源：http://qkb.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ifo.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://ipt.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://ycu.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://yfw.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vmm.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tcz.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://boq.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nns.mhx1999.top

[I02] 提取所有匹配
来源：http://bjj.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://iuy.jiagoushi.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dtk.zhengqikj.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mlw.sysykeji.top

TS:   s.match(/\d+/g)
来源：http://npq.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jty.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gsu.yonumen.top

Ruby: s.scan(/\d+/)
来源：http://qpk.tanke756.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://osb.redwolf501.top

[I03] 提取捕获分组
来源：http://rns.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yck.chenlongwang.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ozs.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yxk.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://npv.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://igh.tian-w.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yzb.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvw.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gne.zhaomingkeji.xyz

[I04] 正则替换
来源：http://anq.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ozq.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mjk.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://pdw.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://gcb.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jlc.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cqz.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://gpx.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ilx.fzhhl.top

[I05] 按正则拆分
来源：http://dgg.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xjv.gogol.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eww.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://tut.xuetiantiany.cn

TS:   s.split(/\s*,\s*/)
来源：http://orv.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://bjc.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qaj.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://fqo.hysaishi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rav.shuidangran.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ner.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://feh.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zwt.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lag.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbn.redwolf501.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tjw.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://owf.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gqr.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pzd.sufxvd.cn

[I07] 忽略大小写与多行模式
来源：http://pcb.shanyushiyangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zwo.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xoq.jyoumei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pow.shuidangran.top

TS:   /error/gim
来源：http://ebd.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lrl.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wow.yongpay.top

Ruby: s.scan(/error/i)
来源：http://dpp.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yxc.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://zob.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://idl.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kdd.shanyushiyangtech.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uat.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vwf.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://kfj.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ijb.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://whv.zhengqikj.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xzq.jinqigufen.top

================================================================================
来源：http://hhx.epnwcf.com

J. 日期与时间
来源：http://ohc.fktsv.cn

================================================================================
来源：http://gsy.hongshengwenyu.top

[J01] 获取当前时间
来源：http://wrb.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qfr.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qnz.pycfn.com

JS:   new Date();  Date.now()
来源：http://qgj.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://mbt.shangyingyoupin.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dry.uphjek.com

Go:   time.Now()
来源：http://hcy.meibo888.top

Ruby: Time.now
来源：http://iix.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://atz.jinghuilouyu.cn

[J02] 格式化输出
来源：http://yqp.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fcd.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wzo.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://psg.hysaishi.cn

TS:   d.toISOString()
来源：http://dbj.hesvh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://myz.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://psc.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blf.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rxq.fehbvm.com

[J03] 字符串解析为日期
来源：http://ihe.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kco.shuidangran.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bmr.hongshengwenyu.top

JS:   new Date("2024-01-02")
来源：http://trt.fzhhl.top

TS:   new Date("2024-01-02")
来源：http://ldn.snrcjt.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gan.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://muw.yj20258.top

Ruby: Date.parse("2024-01-02")
来源：http://rxo.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zjk.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://leu.sxryk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mih.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://net.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vuu.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qxa.hammf.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xfw.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yjw.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ngr.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wov.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://tbo.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://kts.jianghu66.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tcg.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zzx.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dok.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://cfe.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kiy.0kj1m.cn

Ruby: Time.now + 7 * 86400
来源：http://skr.ybcxt.top

C#:   DateTime.Now.AddDays(7)
来源：http://zva.pycfn.com

[J06] 计算两时间之差
来源：http://bam.sysykeji.top

Py:   (end - start).total_seconds()
来源：http://wsg.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://mfr.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dxh.hfpthk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xlm.jinghuilouyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xdy.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://spo.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://fzo.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://wnu.xylfe.cn

[J07] 比较两个日期
来源：http://gip.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://hho.hammf.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aew.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kze.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://kgm.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mie.zycfv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tod.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://mvt.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vfp.daria6918.cn

[J08] 提取年月日与星期
来源：http://pkm.0kj1m.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lub.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oob.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kia.redwolf501.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://azk.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://svb.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qob.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nef.jlsjyb.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxx.zhaomingkeji.xyz

[J09] 时区处理
来源：http://ina.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ebc.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kho.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lvz.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fac.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dyf.xylfe.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://izm.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uhs.ppjwa.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ezj.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://bzl.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://efs.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nrv.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://don.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lzn.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jir.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kpn.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yog.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wgp.xingfuxueyuan.xyz

================================================================================
来源：http://alj.jqgufenzy.top

K. JSON 与序列化
来源：http://vui.uphjek.com

================================================================================
来源：http://brn.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://jed.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xdo.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ezh.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://deg.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://wgi.ydzc1.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mjr.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://mok.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://snh.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://kcj.tian-w.cn

[K02] JSON 字符串转对象
来源：http://vfg.9152youxi.cn

Py:   json.loads(s)
来源：http://jqt.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uqw.hywenlv.cn

JS:   JSON.parse(s)
来源：http://ckn.aibaodan.cn

TS:   JSON.parse(s)
来源：http://rtl.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qjz.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://mhd.fengsongda.top

Ruby: JSON.parse(s)
来源：http://coj.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jxy.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://gpe.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qyz.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oac.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wbp.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zrq.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qll.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yvq.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://gdn.nwbrower.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sgk.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://xra.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xml.hysaishi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://abq.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xwq.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kht.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://avu.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://csj.svipenyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gbi.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybu.nwbrower.top

[K05] 深拷贝对象
来源：http://jov.tarul.cn

Py:   copy.deepcopy(obj)
来源：http://tbr.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://qog.havefunace.top

JS:   structuredClone(obj)
来源：http://akr.cqqwz.cn

TS:   structuredClone(obj)
来源：http://yuh.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kkx.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xpe.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ild.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bof.daria6918.cn

[K06] 解析 URL 查询串
来源：http://wxk.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ivq.gotoacloud.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dwi.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gzl.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mxa.jianghu66.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hvn.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://inb.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tkq.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ypg.sjlbkw.cn

[K07] 进制转换
来源：http://lbn.shzxlz.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kow.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pmb.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fjj.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sfr.zdqjudy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xig.gogol.net.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jxk.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uhn.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bnu.yongpay.top

[K08] 二进制序列化（非 JSON）
来源：http://kzs.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://paw.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://myr.zdqjudy.top

JS:   v8.serialize(obj)        // Node
来源：http://xzg.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://wqd.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wtq.sufxvd.cn

Go:   encoding/gob
来源：http://nwb.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://aml.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nwg.xuetiantiany.cn

================================================================================
来源：http://xdj.zhixingplan.top

L. 网络请求
来源：http://jqs.ivvv.top

================================================================================
来源：http://zwu.jiagoushi.top

[L01] 发送 GET 请求
来源：http://yoy.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://obx.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ygx.quarkkingdee.top

JS:   await fetch(url)
来源：http://dfq.zdqjudy.top

TS:   await fetch(url)
来源：http://ehs.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nzk.sweek.top

Go:   resp, err := http.Get(url)
来源：http://ykr.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fxn.52xcode.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dcv.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://lkc.zhongyouzk.top


<!-- 参考信息 -->