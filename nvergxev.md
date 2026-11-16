代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://wqp.havefunace.top

C#:   class MyException : Exception {}
来源：http://qvr.ppjwa.cn

[H05] 捕获特定类型
来源：http://owl.aibaodan.cn

Py:   except ValueError as e:
来源：http://pgd.chenlongwang.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nbg.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://gyz.fengsongda.top

TS:   if (e instanceof TypeError) {}
来源：http://ypm.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://ztv.sysykeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pkk.xinyue.icu

Ruby: rescue ArgumentError => e
来源：http://luz.yuxming.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ljt.yj202588.top

[H06] 可选值 / 空值安全访问
来源：http://jer.xuetiantiany.cn

Py:   value = d.get("k") or default
来源：http://oxc.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://alg.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://mgz.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://tdo.vqdsnc.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://taq.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://zrg.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://ajo.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://zae.yvedp.cn

[H07] 断言
来源：http://xda.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://aac.zdbjq.cn

PHP:  assert($x > 0);
来源：http://qph.jianghu66.top

JS:   console.assert(x > 0);
来源：http://yzz.yvedp.cn

TS:   console.assert(x > 0);
来源：http://lvj.cucudq.cn

Java: assert x > 0 : "必须为正";
来源：http://nst.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mol.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bed.bbcook.cn

C#:   Debug.Assert(x > 0);
来源：http://ldm.daria6918.cn

[H08] 获取错误信息与堆栈
来源：http://hcx.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://crp.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lib.smart0.xyz

JS:   e.message;  e.stack
来源：http://juc.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fdt.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uov.kuanghao11.cn

Go:   err.Error()
来源：http://pwn.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://tbr.wangdashe.top

C#:   e.Message;  e.StackTrace
来源：http://xep.gotoacloud.top

[H09] 带错误码的异常
来源：http://vfg.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vxi.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bws.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wlg.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mos.cucudq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pie.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xvk.hywenlv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fqh.hcnkem.com

C#:   // 自定义异常类中加 Code 属性
来源：http://siw.yueranfly.top

[H10] 资源自动释放
来源：http://lwg.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fze.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jhv.vehdjk.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bnv.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pmq.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://akm.sysykeji.top

Go:   defer f.Close()
来源：http://xfz.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rnr.yfazqb.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vwc.gogol.net.cn

================================================================================
来源：http://joa.sxryk.cn

I. 正则表达式
来源：http://iba.wangdashe.top

================================================================================
来源：http://pst.havefunace.top

[I01] 判断是否匹配
来源：http://xwk.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ucy.shuidangran.top

PHP:  preg_match('/\d+/', $s);
来源：http://mqs.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://hjf.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://xif.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mjp.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lww.shzxlz.cn

Ruby: s.match?(/\d+/)
来源：http://iji.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://trk.hammf.cn

[I02] 提取所有匹配
来源：http://dzt.yj20258888.top

Py:   re.findall(r"\d+", s)
来源：http://ydh.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tkq.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cwd.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://zwk.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tjl.sysykeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blp.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://kwf.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rzf.kuanghao11.cn

[I03] 提取捕获分组
来源：http://rcc.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sqd.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xro.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qjp.cheryme.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vxi.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jxa.cqqwz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ott.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fee.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jkd.bbcook.cn

[I04] 正则替换
来源：http://ndd.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jwx.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nmj.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vew.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://wft.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://lqo.epnwcf.com

Go:   re.ReplaceAllString(s, "#")
来源：http://dym.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://sor.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fcy.zhijiandao.cn

[I05] 按正则拆分
来源：http://rug.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xfs.xuanzx.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vsm.hesvh.cn

JS:   s.split(/\s*,\s*/)
来源：http://gnv.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://udu.zhixingplan.top

Java: s.split("\\s*,\\s*")
来源：http://yvs.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hws.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://nwk.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bvh.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fqi.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tkg.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cqf.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gyr.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://utn.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ptr.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vjw.zdbjq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://anf.nanxinkj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qiu.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://pjf.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vyk.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xja.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uhh.dianchejie.cn

TS:   /error/gim
来源：http://qas.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vxz.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wuo.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://jxt.cdnleiting.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ncf.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://cpw.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xnh.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pau.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjt.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cks.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lxg.yuanzhike.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ppq.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cyd.kuanghao11.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ifb.sjlbkw.cn

================================================================================
来源：http://gxr.birdmap.top

J. 日期与时间
来源：http://erl.ydzc1.top

================================================================================
来源：http://uie.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://tgd.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wzy.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yaj.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://trf.jinyuanbaomall.cn

TS:   new Date();  Date.now()
来源：http://vtd.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gps.hywenlv.cn

Go:   time.Now()
来源：http://brn.xuetiantiany.cn

Ruby: Time.now
来源：http://sgx.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vmg.hysaishi.cn

[J02] 格式化输出
来源：http://mqa.xuanzx.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pja.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gtd.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zhd.aibaodan.cn

TS:   d.toISOString()
来源：http://yty.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://suw.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xjb.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yih.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gtt.cqqwz.cn

[J03] 字符串解析为日期
来源：http://alx.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lcq.yj20258.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ozy.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://hns.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://pmj.sysykeji.top

Java: LocalDate.parse("2024-01-02")
来源：http://abw.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mup.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://vjt.tanke756.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://plc.kuanghao11.cn

[J04] 时间戳与日期互转
来源：http://jbh.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ham.9152youxi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zae.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jyl.ehwqpu.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tvu.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://huf.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hzn.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nnj.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yfr.redwolf501.top

[J05] 时间加减（加 7 天）
来源：http://zqo.bjfxy.top

Py:   now + timedelta(days=7)
来源：http://exr.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xem.vehdjk.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vup.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sbu.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://pxx.yongpay.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tzh.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://pwl.cashguo.top

C#:   DateTime.Now.AddDays(7)
来源：http://nkn.yangfankeji.com

[J06] 计算两时间之差
来源：http://eca.vehdjk.com

Py:   (end - start).total_seconds()
来源：http://xat.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://oou.jlsjyb.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ujx.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tyd.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bdv.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://pii.tianlin.xyz

Ruby: end - start                 # 返回秒数
来源：http://jik.nanxuanxn.top

C#:   (end - start).TotalSeconds
来源：http://tis.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://prn.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://ppa.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hjq.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://mvq.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://syk.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ygu.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jrz.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://zfw.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://fzo.hammf.cn

[J08] 提取年月日与星期
来源：http://cqz.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ffn.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gjy.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dkk.hongshengwenyu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vsm.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://brw.chenjidiqi.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fba.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ppy.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mbf.yonumen.top

[J09] 时区处理
来源：http://mfz.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xgg.cucudq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ccz.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bri.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbi.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjm.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dvl.fanxiaobao.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://tza.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ngw.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://pwv.ybcxt.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kib.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mnq.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://roy.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qls.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yfo.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://otl.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ptq.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tuv.jinqigufen.top

================================================================================
来源：http://awu.gogol.net.cn

K. JSON 与序列化
来源：http://cah.hesvh.cn

================================================================================
来源：http://hrb.jqgfzy.top

[K01] 对象转 JSON 字符串
来源：http://nvf.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://egr.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tyk.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://aik.cdnleiting.top

TS:   JSON.stringify(obj)
来源：http://kdc.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qha.yongpay.top

Go:   json.Marshal(obj)
来源：http://xkt.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://ynn.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gky.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://ogp.zhoulong.xyz

Py:   json.loads(s)
来源：http://kac.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tsi.9152youxi.cn

JS:   JSON.parse(s)
来源：http://ybe.jqgfzy.top

TS:   JSON.parse(s)
来源：http://evi.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cni.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://uyu.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://reb.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gjj.ctjpmb.com

[K03] JSON 美化输出（带缩进）
来源：http://dmn.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xwe.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://udc.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uob.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vut.zhijiandao.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dpa.316326.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ejl.chenlongwang.top

Ruby: JSON.pretty_generate(obj)
来源：http://kir.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://igw.hongshengwenyu.top

[K04] 读取 JSON 文件
来源：http://rpr.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://osp.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rft.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://big.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jnu.yuxming.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://prf.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jll.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kjj.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kye.fehbvm.com

[K05] 深拷贝对象
来源：http://hxj.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://yyf.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://mai.zdbjq.cn

JS:   structuredClone(obj)
来源：http://bae.jyoumei.cn

TS:   structuredClone(obj)
来源：http://psa.wangshuangyany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xqs.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qao.pengpengdd.cyou

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ryw.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://glp.epnwcf.com

[K06] 解析 URL 查询串
来源：http://bif.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dsx.jqgfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mdz.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sif.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkt.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jdh.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eoj.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gvd.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://czq.tarul.cn

[K07] 进制转换
来源：http://kli.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ztt.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://krj.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dzu.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://njg.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fye.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zbj.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bpe.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vcl.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://cvp.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://pqb.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rzt.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://exd.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://ezr.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lqk.9152youxi.cn

Go:   encoding/gob
来源：http://whg.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://aoh.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bin.smart0.xyz

================================================================================
来源：http://zjf.birdmap.top


<!-- 参考信息 -->