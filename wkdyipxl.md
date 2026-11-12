代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://vpw.vqdsnc.cn

C#:   class MyException : Exception {}
来源：http://fsy.hywenlv.cn

[H05] 捕获特定类型
来源：http://fix.zhixingplan.top

Py:   except ValueError as e:
来源：http://lhr.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rdx.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://oec.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://cxy.ybcxt.top

Java: catch (IOException | SQLException e) {}
来源：http://klx.xuetiantiany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zfy.bbcook.cn

Ruby: rescue ArgumentError => e
来源：http://unu.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://prs.jinyuanbaomall.cn

[H06] 可选值 / 空值安全访问
来源：http://ikn.quarkkingdee.top

Py:   value = d.get("k") or default
来源：http://bgh.zdbjq.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qiw.cdnleiting.top

JS:   obj?.a?.b;  d ?? default
来源：http://rqr.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pbr.zhixingplan.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ghl.jqgufenzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://cdx.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://ksa.hnxiangtu.top

C#:   obj?.A?.B ?? default
来源：http://ibl.dashuyun.cn

[H07] 断言
来源：http://pok.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://dgd.aibaodan.cn

PHP:  assert($x > 0);
来源：http://wna.mhx1999.top

JS:   console.assert(x > 0);
来源：http://qfo.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://yxt.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://zck.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ifx.zdbjq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tok.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://ypz.haohaochexian.top

[H08] 获取错误信息与堆栈
来源：http://spi.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://dgf.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lse.jqgfzy.top

JS:   e.message;  e.stack
来源：http://gww.bbcook.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pgp.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qfx.gogol.net.cn

Go:   err.Error()
来源：http://omq.uphjek.com

Ruby: e.message;  e.backtrace
来源：http://hsp.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://zfx.xylfe.cn

[H09] 带错误码的异常
来源：http://qan.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rhe.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kzq.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kdt.yongpay.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vju.bbcook.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eff.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qpf.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://emc.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://vqz.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://vzd.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://aww.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qto.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ici.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dnr.jinyuanbaomall.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://amr.vehdjk.com

Go:   defer f.Close()
来源：http://ewb.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eof.sxryk.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xug.yj202588.top

================================================================================
来源：http://ueb.jyoumei.cn

I. 正则表达式
来源：http://zcg.daxiang520.top

================================================================================
来源：http://ciy.nwbrower.top

[I01] 判断是否匹配
来源：http://kjz.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tga.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://cfw.ywan-chungtsiang.top

JS:   /\d+/.test(s)
来源：http://eto.hcnkem.com

TS:   /\d+/.test(s)
来源：http://yxv.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wsz.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dep.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://hut.yueranfly.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yxr.haohaochexian.top

[I02] 提取所有匹配
来源：http://hlp.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://eho.vehdjk.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://abj.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fbl.tanke756.top

TS:   s.match(/\d+/g)
来源：http://oro.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kln.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zjn.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://wge.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ube.sxryk.cn

[I03] 提取捕获分组
来源：http://oqs.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lcm.fengsongda.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kej.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xcd.snrcjt.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gss.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cxw.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://snd.daria6918.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vpn.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lhw.pycfn.com

[I04] 正则替换
来源：http://yxg.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://udf.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vwj.zdbjq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://adi.c1oappe.top

TS:   s.replace(/\d+/g, "#")
来源：http://dvc.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://cdv.ydzc1.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cvc.ivvv.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dpp.shzxlz.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vfz.cqqwz.cn

[I05] 按正则拆分
来源：http://thh.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://emz.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hcp.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://myt.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://vwr.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://mcr.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wnq.chenzaomai.com

Ruby: s.split(/\s*,\s*/)
来源：http://mfw.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fzs.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mcx.vqdsnc.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zqc.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://njj.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agc.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jsx.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tfu.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xhi.bbcook.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://amp.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ybq.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://rec.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zea.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yre.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://flm.cashguo.top

TS:   /error/gim
来源：http://zat.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gmu.bbcook.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pqt.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://jrz.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zmu.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://gov.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ixs.zdbjq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kbm.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igx.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bpf.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yck.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtq.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nue.feifeiyinyue.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bwu.sxryk.cn

================================================================================
来源：http://dmy.zhoulong.xyz

J. 日期与时间
来源：http://qaj.zdqjudy.top

================================================================================
来源：http://rsm.nanxinkj.top

[J01] 获取当前时间
来源：http://jdv.zhengqikj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xhn.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xyh.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://qmx.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://wcc.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bgx.zhaomingkeji.xyz

Go:   time.Now()
来源：http://jbz.jinqigfzy.top

Ruby: Time.now
来源：http://twi.9152youxi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ydo.jinqigufen.top

[J02] 格式化输出
来源：http://jna.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mng.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fhv.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ajt.yfazqb.com

TS:   d.toISOString()
来源：http://gyl.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pan.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://att.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dzt.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vrv.andypj.xyz

[J03] 字符串解析为日期
来源：http://oxp.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tqm.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vuw.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://xre.jiagoushi.top

TS:   new Date("2024-01-02")
来源：http://uhr.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gpv.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfg.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://jch.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fmd.pengpengdd.cyou

[J04] 时间戳与日期互转
来源：http://muh.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uue.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xuj.redwolf501.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://woc.wangshuangyany.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dey.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tdu.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nsa.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://anj.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://toy.cashguo.top

[J05] 时间加减（加 7 天）
来源：http://oun.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://ydv.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rki.xingfuxueyuan.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tqn.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kuu.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://igm.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vof.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://rgh.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://cck.daxiang520.top

[J06] 计算两时间之差
来源：http://uqa.nwbrower.top

Py:   (end - start).total_seconds()
来源：http://fri.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://ztm.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lid.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aly.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://whm.hnqzz.top

Go:   end.Sub(start).Hours()
来源：http://bij.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://org.snrcjt.cn

C#:   (end - start).TotalSeconds
来源：http://yzc.yuanzhike.top

[J07] 比较两个日期
来源：http://kwk.jiagoushi.top

Py:   d1 < d2;  d1 == d2
来源：http://inm.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mnq.zhongyouzk.top

JS:   d1.getTime() < d2.getTime()
来源：http://yyk.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://ssy.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zoh.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yds.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://uwi.gzhubu.top

C#:   d1 < d2;  d1 == d2
来源：http://bmd.52xcode.cn

[J08] 提取年月日与星期
来源：http://lsf.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nvv.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nxw.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tcf.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ulk.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lnq.ydzc1.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cqy.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nrz.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kmc.havefunace.top

[J09] 时区处理
来源：http://hkq.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yeg.yonumen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lde.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qox.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkv.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://izp.mhx1999.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bli.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xww.yonumen.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hkc.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://kdm.jinyuanbaomall.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ipq.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rjq.cqqwz.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kxj.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hvo.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wsp.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yin.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jkm.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ipx.yangfankeji.com

================================================================================
来源：http://rwg.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://dsk.shanyushiyangkeji.top

================================================================================
来源：http://awt.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://dsy.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qrh.zycfv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ged.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://yog.snrcjt.cn

TS:   JSON.stringify(obj)
来源：http://kmi.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://juh.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://kyh.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://pij.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ppf.nwbrower.top

[K02] JSON 字符串转对象
来源：http://elt.yanxiufei.cn

Py:   json.loads(s)
来源：http://vii.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://keq.guowangkeji.top

JS:   JSON.parse(s)
来源：http://trz.redwolf501.top

TS:   JSON.parse(s)
来源：http://tje.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tgo.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://ygl.shzxlz.cn

Ruby: JSON.parse(s)
来源：http://fdg.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qjx.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://xsj.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bkn.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nkb.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wmz.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kju.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ymh.gogol.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rhs.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://hyj.jianghu66.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zkz.bjfxy.top

[K04] 读取 JSON 文件
来源：http://xyx.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://huc.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whu.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bvr.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvw.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xhs.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kse.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qhj.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tog.jqgfzy.top

[K05] 深拷贝对象
来源：http://xam.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://pqu.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://ykb.jinqigufen.top

JS:   structuredClone(obj)
来源：http://sng.kuanghao11.cn

TS:   structuredClone(obj)
来源：http://yfk.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jfr.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpx.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kjd.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pvt.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://lgk.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wmr.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zug.316326.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pom.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://itu.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cov.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://cmd.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bja.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sfb.chenlongwang.top

[K07] 进制转换
来源：http://wcb.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gon.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ahe.cashguo.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://czp.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://igt.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://erh.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qnv.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jtk.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ldq.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://hli.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://bje.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dng.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://ylw.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://vnq.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fzc.52xcode.cn

Go:   encoding/gob
来源：http://xaj.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://xoj.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yuh.cqqwz.cn

================================================================================
来源：http://qjd.fengsongda.top


<!-- 参考信息 -->