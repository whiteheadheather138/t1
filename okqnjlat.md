代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://frc.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://cvn.yanxiufei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kmu.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://eeo.hammf.cn

Py:   value = d.get("k") or default
来源：http://avi.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ixl.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://tmi.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://nyq.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ckd.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://yah.chenjidiqi.icu

Ruby: d&.dig(:a, :b)
来源：http://uaz.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://vxp.xinyue.icu

[H07] 断言
来源：http://oic.jinqigufen.top

Py:   assert x > 0, "必须为正"
来源：http://kkp.hywenlv.cn

PHP:  assert($x > 0);
来源：http://wgi.jlsjyb.cn

JS:   console.assert(x > 0);
来源：http://hld.sysykeji.top

TS:   console.assert(x > 0);
来源：http://yub.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://hgv.pycfn.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lrl.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tbm.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://atf.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://mxy.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://wwm.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eja.nanxinkj.top

JS:   e.message;  e.stack
来源：http://sxj.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lcu.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rfj.chenlongwang.top

Go:   err.Error()
来源：http://ptl.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://ttz.vqdsnc.cn

C#:   e.Message;  e.StackTrace
来源：http://rmp.redwolf501.top

[H09] 带错误码的异常
来源：http://zvf.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aki.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jem.xingfuxueyuan.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sxr.iojbl.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gvi.sufxvd.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://irb.mhx1999.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yre.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://dlg.yangfankeji.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ife.dashuyun.cn

[H10] 资源自动释放
来源：http://vai.bbcook.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hwi.jinghuilouyu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oar.zhengqikj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lgk.bjfxy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://upp.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tqs.smart0.xyz

Go:   defer f.Close()
来源：http://qcd.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uhw.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blw.ydjk.org.cn

================================================================================
来源：http://piv.yj20258.top

I. 正则表达式
来源：http://gtj.fengsongda.top

================================================================================
来源：http://aqs.jinqigufen.top

[I01] 判断是否匹配
来源：http://jbt.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nrt.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://wbe.ybcxt.top

JS:   /\d+/.test(s)
来源：http://kjv.xuanzx.com

TS:   /\d+/.test(s)
来源：http://yyw.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://isc.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://arb.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://zsx.pycfn.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dqo.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://chx.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://kwk.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yvw.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xln.smart0.xyz

TS:   s.match(/\d+/g)
来源：http://shv.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nnd.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mxl.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://aay.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mrj.fzhhl.top

[I03] 提取捕获分组
来源：http://nyx.ctjpmb.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zwo.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uny.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blc.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://okx.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ldk.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oao.jinghuilouyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ity.fanxiaobao.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vun.tian-w.cn

[I04] 正则替换
来源：http://jnk.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oyl.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://njq.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://xxd.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://aak.shanyushiyangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://dxy.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tag.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kfj.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://asv.fengsongda.top

[I05] 按正则拆分
来源：http://jph.cqqwz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ptp.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://enc.tanke756.top

JS:   s.split(/\s*,\s*/)
来源：http://oum.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://vvl.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://prr.guowangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zjd.jianghu66.top

Ruby: s.split(/\s*,\s*/)
来源：http://ntl.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eql.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wqz.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yln.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://org.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dbh.haohaochexian.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdm.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jcw.tian-w.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ser.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fmv.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bpx.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://umb.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qnw.hammf.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ryf.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ejm.hnqzz.top

TS:   /error/gim
来源：http://cau.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qre.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nlf.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://xfv.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hfn.shuidangran.top

[I08] 贪婪与非贪婪匹配
来源：http://zkm.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ggf.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zfu.jinyuanbaomall.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://aij.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ana.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://obo.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fcx.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://peq.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npm.kuanghao11.cn

================================================================================
来源：http://xzy.sxryk.cn

J. 日期与时间
来源：http://ygw.shangyingyoupin.top

================================================================================
来源：http://lwa.yonumen.top

[J01] 获取当前时间
来源：http://tqt.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vvi.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bkr.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://vpa.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://lek.c1oappe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qui.zycfv.cn

Go:   time.Now()
来源：http://udn.shanyushiyangtech.top

Ruby: Time.now
来源：http://qus.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgj.jinyuanbaomall.cn

[J02] 格式化输出
来源：http://uip.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vmg.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kpv.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cgt.ivvv.top

TS:   d.toISOString()
来源：http://ghb.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xda.zhoulong.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://maq.yongpay.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jxs.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rya.fengsongda.top

[J03] 字符串解析为日期
来源：http://xjr.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gwi.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zck.hcnkem.com

JS:   new Date("2024-01-02")
来源：http://wjm.uphjek.com

TS:   new Date("2024-01-02")
来源：http://pxz.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://uxw.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yhp.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://iwa.xziqi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kps.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://gfj.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iah.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rwd.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zzv.xuetiantiany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vca.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://eqj.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rww.ydzc1.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://joz.yanxiufei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eue.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://ghe.uphjek.com

Py:   now + timedelta(days=7)
来源：http://irq.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qbi.xuanzx.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mvw.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wti.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://dmn.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dne.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://owd.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pyw.wangshuangyany.cn

[J06] 计算两时间之差
来源：http://hpa.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://cco.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://uaq.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xhl.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://exy.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://bsy.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://rbd.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://qlm.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://fea.xylfe.cn

[J07] 比较两个日期
来源：http://bsz.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://gvd.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ybk.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cgs.iojbl.cn

TS:   d1.getTime() < d2.getTime()
来源：http://hhl.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nvg.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ftq.snrcjt.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jlw.52xcode.cn

C#:   d1 < d2;  d1 == d2
来源：http://tzb.guowangkeji.top

[J08] 提取年月日与星期
来源：http://glm.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dyj.guowangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hxp.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://okf.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ejd.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ovf.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://egv.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sat.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eah.gogol.net.cn

[J09] 时区处理
来源：http://xjm.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rht.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zpt.9152youxi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lzd.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ttx.yfazqb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mpn.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yrr.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://znt.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dls.bbcook.cn

[J10] 取今天 / 本月第一天
来源：http://vnu.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://tyy.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vvp.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sph.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://err.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lrf.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://esm.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rzg.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lzj.gotoacloud.top

================================================================================
来源：http://iap.ydzc1.top

K. JSON 与序列化
来源：http://ijq.jinghuilouyu.cn

================================================================================
来源：http://zpl.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://tkd.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ohn.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yat.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://hee.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://gyw.fehbvm.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ljo.mhx1999.top

Go:   json.Marshal(obj)
来源：http://mbb.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://ykl.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://olh.sxryk.cn

[K02] JSON 字符串转对象
来源：http://eeh.guannengcc.top

Py:   json.loads(s)
来源：http://zzk.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lvy.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://ddg.smart0.xyz

TS:   JSON.parse(s)
来源：http://hux.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tnq.pengpengdd.cyou

Go:   json.Unmarshal(data, &v)
来源：http://kex.jinghuilouyu.cn

Ruby: JSON.parse(s)
来源：http://oug.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plu.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://gpi.hnqzz.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iqc.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eoc.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nwg.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gqa.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tvh.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijy.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://abw.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://utz.guannengcc.top

[K04] 读取 JSON 文件
来源：http://xbr.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zrx.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gmx.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hgj.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cto.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aaf.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zaj.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vym.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://drj.aizwys.cn

[K05] 深拷贝对象
来源：http://uwh.yangfankeji.com

Py:   copy.deepcopy(obj)
来源：http://dpg.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://add.yuxming.cn

JS:   structuredClone(obj)
来源：http://ftj.jianghu66.top

TS:   structuredClone(obj)
来源：http://ijj.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zqw.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sfm.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fkk.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://iey.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://pxt.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uaw.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cpu.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gfj.gzhubu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wzc.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ymv.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qdk.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cce.hywenlv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bic.hcnkem.com

[K07] 进制转换
来源：http://ghy.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qow.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jln.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xvh.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://flc.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ung.ybcxt.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vpk.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wjj.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://itf.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://cpe.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://wzc.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lcr.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://uco.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://idw.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pby.sxryk.cn

Go:   encoding/gob
来源：http://vmm.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://ahs.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ihr.hfpthk.cn

================================================================================
来源：http://ljg.shanyushiyangkeji.top

L. 网络请求
来源：http://hck.hammf.cn

================================================================================
来源：http://thi.ctjpmb.com

[L01] 发送 GET 请求
来源：http://ale.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ucu.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://djw.birdmap.top

JS:   await fetch(url)
来源：http://yvf.daxiang520.top

TS:   await fetch(url)
来源：http://eju.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ymh.yfazqb.com


<!-- 参考信息 -->