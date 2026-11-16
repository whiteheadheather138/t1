代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://oyt.fzhhl.top

C#:   class MyException : Exception {}
来源：http://ojt.haohaochexian.top

[H05] 捕获特定类型
来源：http://onn.yongpay.top

Py:   except ValueError as e:
来源：http://imc.zhongyouzk.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://auq.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://hwl.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://dmk.zhaomingkeji.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fez.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zfz.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://uzf.uphjek.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xzz.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://iox.fktsv.cn

Py:   value = d.get("k") or default
来源：http://vwa.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://hnk.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://hwz.hongshengwenyu.top

TS:   obj?.a?.b;  d ?? default
来源：http://brh.zhengqikj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qvz.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://leb.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://dxz.chenzaomai.com

C#:   obj?.A?.B ?? default
来源：http://dwq.9152youxi.cn

[H07] 断言
来源：http://ueo.jiagoushi.top

Py:   assert x > 0, "必须为正"
来源：http://ehg.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://ljr.jinqigufen.top

JS:   console.assert(x > 0);
来源：http://xyp.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://ohr.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://qjq.jqgufenzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qfb.hysaishi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dtr.bjfxy.top

C#:   Debug.Assert(x > 0);
来源：http://zwf.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://cis.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://cpz.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://etj.fanxiaobao.xyz

JS:   e.message;  e.stack
来源：http://kgw.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://eny.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qch.yanxiufei.cn

Go:   err.Error()
来源：http://ulk.jqgufenzy.top

Ruby: e.message;  e.backtrace
来源：http://aje.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://arr.chenzaomai.com

[H09] 带错误码的异常
来源：http://bsy.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dsk.9152youxi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pzg.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gqx.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qmv.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rad.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nnv.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uom.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://daj.gotoacloud.top

[H10] 资源自动释放
来源：http://qil.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ucb.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://inb.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fwo.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pen.cucudq.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mxo.yongpay.top

Go:   defer f.Close()
来源：http://arl.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymg.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sru.gzhubu.top

================================================================================
来源：http://oml.wangshuangyany.cn

I. 正则表达式
来源：http://ygr.sxryk.cn

================================================================================
来源：http://lbs.gogol.net.cn

[I01] 判断是否匹配
来源：http://khl.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fls.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://qkr.fktsv.cn

JS:   /\d+/.test(s)
来源：http://qar.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://dxh.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qpa.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iio.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://zfw.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zjy.cqqwz.cn

[I02] 提取所有匹配
来源：http://xtr.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://qjy.zdbjq.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hjp.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ged.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://frg.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kbs.daxiang520.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xec.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://bzr.haohaochexian.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gxv.dashuyun.cn

[I03] 提取捕获分组
来源：http://col.zdqjudy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dff.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbn.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tqk.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yyt.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hmg.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hru.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://woc.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oyb.pycfn.com

[I04] 正则替换
来源：http://zeb.zhiwuduotai.top

Py:   re.sub(r"\d+", "#", s)
来源：http://odb.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zhg.xuetiantiany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uic.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dpr.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://iqj.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mde.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sbl.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://swa.aizwys.cn

[I05] 按正则拆分
来源：http://hgo.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://jae.fehbvm.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxd.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://xqt.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://rmz.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://rpi.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://txd.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://eph.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://txc.gotoacloud.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hsk.ehwqpu.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gpq.jinqigfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ekh.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vkb.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmb.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hfs.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://auy.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://klb.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://goo.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://ifd.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ozl.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sfr.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tvg.xuanzx.com

TS:   /error/gim
来源：http://lpn.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://afu.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://koz.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://tog.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jmo.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://skt.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kws.tarul.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mxs.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://abi.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://myb.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://kvc.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://res.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oih.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uub.fehbvm.com

================================================================================
来源：http://hdu.shuidangran.top

J. 日期与时间
来源：http://whb.sysykeji.top

================================================================================
来源：http://nvo.dashuyun.cn

[J01] 获取当前时间
来源：http://fde.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://fey.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://oyp.fehbvm.com

JS:   new Date();  Date.now()
来源：http://tcu.birdmap.top

TS:   new Date();  Date.now()
来源：http://qrw.pycfn.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tls.mhx1999.top

Go:   time.Now()
来源：http://zpx.haohaochexian.top

Ruby: Time.now
来源：http://aug.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zhv.kuanghao11.cn

[J02] 格式化输出
来源：http://iub.tanke756.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wsh.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pcl.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ziy.sxryk.cn

TS:   d.toISOString()
来源：http://fif.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zrd.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jbm.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qnm.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gcm.shuidangran.top

[J03] 字符串解析为日期
来源：http://ysu.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ocg.shzxlz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fnt.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://pcw.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://sjx.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://wqs.fktsv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://avy.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://nsx.zhoulong.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://naw.bjfxy.top

[J04] 时间戳与日期互转
来源：http://frr.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ygf.yonumen.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zyd.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tjw.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://mhq.shzxlz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vok.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xuv.gogol.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kqv.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://trk.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://oeb.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://qwv.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ytd.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wzz.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ube.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://elr.kuanghao11.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tvi.fehbvm.com

Ruby: Time.now + 7 * 86400
来源：http://cnp.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ljw.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://fjl.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://vdd.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://app.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fxe.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://txi.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://daz.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://iro.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://rxd.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://zwa.zhengqikj.top

[J07] 比较两个日期
来源：http://ejx.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://nav.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://izu.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://lkf.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ssa.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zni.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mah.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://wyn.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://wdb.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://gsw.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gov.fehbvm.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pmb.shangyingyoupin.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://biy.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://igq.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xer.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sgr.nanxuanxn.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wkn.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://klg.feifeiyinyue.top

[J09] 时区处理
来源：http://xbr.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nyw.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rke.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipe.hfpthk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rld.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lkq.sjlbkw.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ulb.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://nee.hnqzz.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wdw.fehbvm.com

[J10] 取今天 / 本月第一天
来源：http://gey.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wim.chenjidiqi.icu

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://plo.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsn.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lno.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xuq.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rax.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ili.sxryk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uun.hysaishi.cn

================================================================================
来源：http://dvw.feifeiyinyue.top

K. JSON 与序列化
来源：http://qaz.wangshuangyany.cn

================================================================================
来源：http://iyx.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://sub.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oqp.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ujo.fzhhl.top

JS:   JSON.stringify(obj)
来源：http://dpx.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://xlf.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vov.yuxming.cn

Go:   json.Marshal(obj)
来源：http://gxk.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://xtr.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vuz.gaohongyu789.top

[K02] JSON 字符串转对象
来源：http://xvq.hysaishi.cn

Py:   json.loads(s)
来源：http://hav.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kzm.pycfn.com

JS:   JSON.parse(s)
来源：http://wqf.fanxiaobao.xyz

TS:   JSON.parse(s)
来源：http://zvd.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xxz.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://syx.c1oappe.top

Ruby: JSON.parse(s)
来源：http://hri.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdc.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://pbl.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvq.ydzc1.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fge.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tin.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mia.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://paj.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avj.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://stt.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qsb.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://dep.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wed.iojbl.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ufe.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfq.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ttj.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://opl.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fal.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://zpj.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eta.ybcxt.top

[K05] 深拷贝对象
来源：http://bqz.jyoumei.cn

Py:   copy.deepcopy(obj)
来源：http://hgp.fanxiaobao.xyz

PHP:  unserialize(serialize($obj));
来源：http://kax.sjlbkw.cn

JS:   structuredClone(obj)
来源：http://lyf.shzxlz.cn

TS:   structuredClone(obj)
来源：http://swo.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uop.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://brb.epnwcf.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://opa.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xrv.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://dza.andypj.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ncl.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://olf.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://szo.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lwl.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xqn.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kss.xziqi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cpe.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qhh.zhixingplan.top

[K07] 进制转换
来源：http://jqp.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pwc.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kuf.xylfe.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bik.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xxp.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://emj.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wxn.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kxc.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ugs.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://vef.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://bay.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://vpo.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://lji.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://hsl.sufxvd.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qtd.dianchejie.cn

Go:   encoding/gob
来源：http://wzo.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://irt.jinqigfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ken.havefunace.top

================================================================================
来源：http://eij.xingfuxueyuan.xyz


<!-- 参考信息 -->