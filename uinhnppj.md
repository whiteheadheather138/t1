代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sdf.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://kmq.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://pyx.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://rpv.tarul.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jxt.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://bza.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dbh.52xcode.cn

[H06] 可选值 / 空值安全访问
来源：http://qrm.hcnkem.com

Py:   value = d.get("k") or default
来源：http://udw.chenlongwang.top

PHP:  $v = $d["k"] ?? null;
来源：http://emd.hnqzz.top

JS:   obj?.a?.b;  d ?? default
来源：http://mma.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://daq.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fqp.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://iqz.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://oqv.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://xrk.shanyushiyangkeji.top

[H07] 断言
来源：http://onf.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://jch.ydzc1.top

PHP:  assert($x > 0);
来源：http://eaz.xinyue.icu

JS:   console.assert(x > 0);
来源：http://kgm.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://exy.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://hra.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xzs.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tqf.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://cjq.fengsongda.top

[H08] 获取错误信息与堆栈
来源：http://yjm.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://uei.hfpthk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://alm.epnwcf.com

JS:   e.message;  e.stack
来源：http://gcl.ehwqpu.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://egj.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ovv.zhixingplan.top

Go:   err.Error()
来源：http://nfp.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://ypq.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://rgl.xylfe.cn

[H09] 带错误码的异常
来源：http://yvg.zhongyouzk.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tdg.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sie.mhx1999.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vah.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://luu.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mdh.xuanzx.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pbm.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mmm.haohaochexian.top

C#:   // 自定义异常类中加 Code 属性
来源：http://syt.yj202588.top

[H10] 资源自动释放
来源：http://ydm.gogol.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbj.dashuyun.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yut.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lst.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ztn.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vgq.epnwcf.com

Go:   defer f.Close()
来源：http://bai.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://crd.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pck.hongshengwenyu.top

================================================================================
来源：http://ejp.guannengcc.top

I. 正则表达式
来源：http://diq.bjfxy.top

================================================================================
来源：http://glx.xinyue.icu

[I01] 判断是否匹配
来源：http://hnk.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gpt.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://fof.316326.xyz

JS:   /\d+/.test(s)
来源：http://jgq.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://lps.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://swq.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://djm.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://rgb.quarkkingdee.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dns.fzhhl.top

[I02] 提取所有匹配
来源：http://cun.316326.xyz

Py:   re.findall(r"\d+", s)
来源：http://ltr.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qtg.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ybx.havefunace.top

TS:   s.match(/\d+/g)
来源：http://xwe.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zyr.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qzb.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://voo.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wnx.svipenyu.cn

[I03] 提取捕获分组
来源：http://rxp.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hzd.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://upe.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jum.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iby.sweek.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zwb.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usy.zhiwuduotai.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bbg.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://srg.haohaochexian.top

[I04] 正则替换
来源：http://yto.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oux.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://thf.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://tgn.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yka.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://ypt.bbcook.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://czy.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nya.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kyx.aizwys.cn

[I05] 按正则拆分
来源：http://ddp.yuanzhike.top

Py:   re.split(r"\s*,\s*", s)
来源：http://osc.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fjt.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://vnp.gotoacloud.top

TS:   s.split(/\s*,\s*/)
来源：http://hyh.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://rkq.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ehy.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://pce.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jlp.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mtr.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vkj.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oaq.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sxt.havefunace.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zgg.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wjh.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xvq.tianlin.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wao.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ymu.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://wao.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sjm.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cnk.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ewb.jqgufenzy.top

TS:   /error/gim
来源：http://cmq.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qey.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fds.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://jjy.yj20258.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kgu.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://ivt.mhx1999.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kxx.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ahu.yj20258888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xxn.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jpc.gzhubu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cav.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hoy.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nvg.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mox.andypj.xyz

================================================================================
来源：http://vzx.sysykeji.top

J. 日期与时间
来源：http://xgc.zhoulong.xyz

================================================================================
来源：http://qim.zhiwuduotai.top

[J01] 获取当前时间
来源：http://lnu.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gdx.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yfu.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://znm.gzhubu.top

TS:   new Date();  Date.now()
来源：http://tsn.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tug.jinqigufen.top

Go:   time.Now()
来源：http://nbh.zhongyouzk.top

Ruby: Time.now
来源：http://onz.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nco.meibo888.top

[J02] 格式化输出
来源：http://enx.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kkq.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://syf.jqgfzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fos.sysykeji.top

TS:   d.toISOString()
来源：http://xpm.kuanghao11.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hba.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kam.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://otu.uphjek.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rjj.nwbrower.top

[J03] 字符串解析为日期
来源：http://erp.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dbg.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kld.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://zyc.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://jia.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nxb.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qvn.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://lcu.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eoo.xuanzx.com

[J04] 时间戳与日期互转
来源：http://ftg.shanyushiyangtech.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vxa.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aje.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ddo.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://srv.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tgq.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vue.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bfd.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://euy.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://ewa.gaohongyu789.top

Py:   now + timedelta(days=7)
来源：http://ojy.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://szv.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bjx.hysaishi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wkp.yongpay.top

Java: LocalDate.now().plusDays(7)
来源：http://hwl.hysaishi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zsb.ywan-chungtsiang.top

Ruby: Time.now + 7 * 86400
来源：http://sfl.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://rip.fengsongda.top

[J06] 计算两时间之差
来源：http://mrg.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://nez.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://ogc.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bch.yj20258888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kfg.shzxlz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://suz.yj202588.top

Go:   end.Sub(start).Hours()
来源：http://xgw.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://yue.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://vio.bjfxy.top

[J07] 比较两个日期
来源：http://uhp.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wqz.52xcode.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ifh.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fit.birdmap.top

TS:   d1.getTime() < d2.getTime()
来源：http://vhy.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://esp.ehwqpu.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bsc.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://pkv.yanxiufei.cn

C#:   d1 < d2;  d1 == d2
来源：http://jmk.daxiang520.top

[J08] 提取年月日与星期
来源：http://bwm.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xdd.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zhw.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mom.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iec.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xdc.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vqx.jianghu66.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jei.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://out.ctjpmb.com

[J09] 时区处理
来源：http://xbz.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vqx.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dhf.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://awp.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bgp.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://raz.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rxn.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jpw.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mwe.yuxming.cn

[J10] 取今天 / 本月第一天
来源：http://asw.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://axi.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iim.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kxb.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://umc.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://off.hywenlv.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://orn.guannengcc.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ynb.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pmc.yvedp.cn

================================================================================
来源：http://ohq.zhoulong.xyz

K. JSON 与序列化
来源：http://zjm.iojbl.cn

================================================================================
来源：http://qul.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://yrp.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mhm.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nbt.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://gqd.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://zlp.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pos.cucudq.cn

Go:   json.Marshal(obj)
来源：http://kez.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://ras.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ing.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://xbf.xuetiantiany.cn

Py:   json.loads(s)
来源：http://gxx.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vxc.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://hoj.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://vtz.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dli.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://iat.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://dmi.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zmf.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://chw.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tdd.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xyt.svipenyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://frw.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ubk.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://snd.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yhf.zhiwuduotai.top

Ruby: JSON.pretty_generate(obj)
来源：http://hot.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lgg.pycfn.com

[K04] 读取 JSON 文件
来源：http://pfm.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tum.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cyy.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buf.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://but.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yis.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hkb.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://kku.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gfy.bbcook.cn

[K05] 深拷贝对象
来源：http://vuo.sweek.top

Py:   copy.deepcopy(obj)
来源：http://wmv.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://tuf.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://mma.52xcode.cn

TS:   structuredClone(obj)
来源：http://bld.jqgfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nsf.jinqigfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://doz.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://swt.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qgj.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://ocy.jqgfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mhq.nanxuanxn.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://afh.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ltb.0kj1m.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ype.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zki.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jmz.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pcz.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://suy.xuetiantiany.cn

[K07] 进制转换
来源：http://vxr.fehbvm.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://omf.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qid.yangfankeji.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://toa.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xpp.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ymk.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nnn.chenlongwang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gxk.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://akd.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://dne.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://uks.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zfo.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://hcx.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://wtb.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wup.zdbjq.cn

Go:   encoding/gob
来源：http://tar.ivvv.top

Ruby: Marshal.dump(obj)
来源：http://mfh.zdbjq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uck.svipenyu.cn

================================================================================
来源：http://ldw.mhx1999.top

L. 网络请求
来源：http://ncb.redwolf501.top

================================================================================
来源：http://bwb.bjfxy.top

[L01] 发送 GET 请求
来源：http://quk.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eei.hysaishi.cn


<!-- 参考信息 -->