代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://bpi.52xcode.cn

C#:   class MyException : Exception {}
来源：http://xop.jqgufenzy.top

[H05] 捕获特定类型
来源：http://kor.daxiang520.top

Py:   except ValueError as e:
来源：http://nui.ybcxt.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tjq.epnwcf.com

JS:   if (e instanceof TypeError) {}
来源：http://nte.hammf.cn

TS:   if (e instanceof TypeError) {}
来源：http://fia.smart0.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nhu.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pfc.chenlongwang.top

Ruby: rescue ArgumentError => e
来源：http://nmp.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tko.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://bzm.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://afz.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vjq.jiagoushi.top

JS:   obj?.a?.b;  d ?? default
来源：http://ozo.yj20258888.top

TS:   obj?.a?.b;  d ?? default
来源：http://xqx.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yrm.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ekb.jlsjyb.cn

Ruby: d&.dig(:a, :b)
来源：http://hzr.chenlongwang.top

C#:   obj?.A?.B ?? default
来源：http://eyx.aibaodan.cn

[H07] 断言
来源：http://avt.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://epq.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://jzp.guowangkeji.top

JS:   console.assert(x > 0);
来源：http://oxf.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://fqn.mhx1999.top

Java: assert x > 0 : "必须为正";
来源：http://has.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://adt.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dlu.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://kon.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://fbd.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://vut.jianghu66.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gry.jianghu66.top

JS:   e.message;  e.stack
来源：http://pgj.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pte.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://asv.snrcjt.cn

Go:   err.Error()
来源：http://oyb.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://thu.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://coc.daria6918.cn

[H09] 带错误码的异常
来源：http://ihl.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rqd.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://mis.jqgfzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://khr.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eqk.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rjq.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hjz.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://dra.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jgx.zdbjq.cn

[H10] 资源自动释放
来源：http://tlx.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://djw.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hdh.bbcook.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fxm.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yaa.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://prl.nanxuanxn.top

Go:   defer f.Close()
来源：http://dou.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rzl.ywan-chungtsiang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qsd.zdqjudy.top

================================================================================
来源：http://bgv.cqqwz.cn

I. 正则表达式
来源：http://nzs.guannengcc.top

================================================================================
来源：http://zif.pycfn.com

[I01] 判断是否匹配
来源：http://wyk.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fgg.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://dnu.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://kjv.bbcook.cn

TS:   /\d+/.test(s)
来源：http://zay.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mhz.tanke756.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pou.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://jvh.pengpengdd.cyou

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdy.svipenyu.cn

[I02] 提取所有匹配
来源：http://zph.cqqwz.cn

Py:   re.findall(r"\d+", s)
来源：http://dbq.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rsd.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zha.yanxiufei.cn

TS:   s.match(/\d+/g)
来源：http://boy.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hja.haohaochexian.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bak.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://dfx.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ryg.cqqwz.cn

[I03] 提取捕获分组
来源：http://rsx.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://arm.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tol.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyc.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xfs.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vng.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iyq.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cyf.iojbl.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gsg.andypj.xyz

[I04] 正则替换
来源：http://ser.vehdjk.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ibg.316326.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mdw.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://swd.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://zqt.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://unh.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ptr.yongpay.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bfe.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://avc.andypj.xyz

[I05] 按正则拆分
来源：http://dna.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://smo.yj202588.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ehq.jinghuilouyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nvj.tianlin.xyz

TS:   s.split(/\s*,\s*/)
来源：http://cdg.shangyingyoupin.top

Java: s.split("\\s*,\\s*")
来源：http://uqy.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://plu.cheryme.top

Ruby: s.split(/\s*,\s*/)
来源：http://vmx.hesvh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qpv.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qqg.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://djg.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vrs.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vql.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://onc.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ogy.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mwf.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uxx.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qjt.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://der.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://erv.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://asd.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eel.hywenlv.cn

TS:   /error/gim
来源：http://gsr.yongpay.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oth.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mmu.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://sys.tianlin.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://obn.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://ome.0kj1m.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oqy.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sjr.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://woy.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jib.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://crt.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gix.gzhubu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hyn.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yit.pycfn.com

================================================================================
来源：http://cjy.yueranfly.top

J. 日期与时间
来源：http://xtg.hammf.cn

================================================================================
来源：http://cms.svipenyu.cn

[J01] 获取当前时间
来源：http://tmt.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ejq.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cle.c1oappe.top

JS:   new Date();  Date.now()
来源：http://zbb.tian-w.cn

TS:   new Date();  Date.now()
来源：http://orq.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://obx.zdbjq.cn

Go:   time.Now()
来源：http://cgf.ywan-chungtsiang.top

Ruby: Time.now
来源：http://pgb.sxryk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xcs.fehbvm.com

[J02] 格式化输出
来源：http://ybo.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bdt.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvf.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wte.hongshengwenyu.top

TS:   d.toISOString()
来源：http://bkb.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xcd.sysykeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ggh.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kgp.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sle.sweek.top

[J03] 字符串解析为日期
来源：http://phn.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zgx.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mkh.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://sht.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://vys.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yjj.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hqx.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://jye.jqgufenzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ezz.sufxvd.cn

[J04] 时间戳与日期互转
来源：http://emy.chenjidiqi.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hka.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jdl.aibaodan.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oqu.yonumen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fty.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hok.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wym.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nfe.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cme.yvedp.cn

[J05] 时间加减（加 7 天）
来源：http://mmn.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://myy.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://vfh.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vcz.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aka.gogol.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://dsk.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fff.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://vca.zdbjq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wdf.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://uvx.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://zbn.zdqjudy.top

PHP:  $end->diff($start)->days;
来源：http://kol.epnwcf.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wzy.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vcj.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ltc.sysykeji.top

Go:   end.Sub(start).Hours()
来源：http://qdn.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://kbl.zhaomingkeji.xyz

C#:   (end - start).TotalSeconds
来源：http://whc.zycfv.cn

[J07] 比较两个日期
来源：http://xli.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://vbw.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eeu.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://gnb.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://obp.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tiq.yanxiufei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ktd.9152youxi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://upd.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://czw.yuanzhike.top

[J08] 提取年月日与星期
来源：http://ttw.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nub.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fcj.guannengcc.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wjs.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbf.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ktm.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jyp.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xwx.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qpc.chenlongwang.top

[J09] 时区处理
来源：http://hgy.ywan-chungtsiang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wzz.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lip.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvl.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kra.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ydo.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xsk.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://agl.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bgt.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://ugp.zhiwuduotai.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wff.c1oappe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cip.xinyue.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yqt.9152youxi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://khy.jinqigufen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ryu.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://avm.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bng.nanxinkj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cld.svipenyu.cn

================================================================================
来源：http://mui.zycfv.cn

K. JSON 与序列化
来源：http://blz.sjlbkw.cn

================================================================================
来源：http://iji.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://yrf.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fec.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lst.yuanzhike.top

JS:   JSON.stringify(obj)
来源：http://ees.316326.xyz

TS:   JSON.stringify(obj)
来源：http://mbs.ivvv.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dpk.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://ccd.xingfuxueyuan.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://rxu.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qgt.yj20258888.top

[K02] JSON 字符串转对象
来源：http://wfh.shangyingyoupin.top

Py:   json.loads(s)
来源：http://vth.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sdm.ybcxt.top

JS:   JSON.parse(s)
来源：http://jvb.hammf.cn

TS:   JSON.parse(s)
来源：http://djo.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://esx.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://bmb.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://wob.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qnr.yj20258888.top

[K03] JSON 美化输出（带缩进）
来源：http://lsa.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://chl.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ugr.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jkm.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jih.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://btd.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://imy.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://yqz.yuxming.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://bqs.cheryme.top

[K04] 读取 JSON 文件
来源：http://nfv.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://phn.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysg.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wii.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxo.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xbx.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://twa.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mas.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vdu.ydzc1.top

[K05] 深拷贝对象
来源：http://bec.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://hox.zhaomingkeji.xyz

PHP:  unserialize(serialize($obj));
来源：http://uqf.yj20258.top

JS:   structuredClone(obj)
来源：http://oqj.hammf.cn

TS:   structuredClone(obj)
来源：http://fdz.jinghuilouyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pqu.daria6918.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qpc.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dfu.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hoi.tian-w.cn

[K06] 解析 URL 查询串
来源：http://poh.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://juy.hcnkem.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kzf.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vtz.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rte.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://izl.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hlf.hammf.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://knq.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uqy.316326.xyz

[K07] 进制转换
来源：http://ttw.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://itt.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://itj.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oqs.shanyushiyangtech.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qqp.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxw.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ifd.ywan-chungtsiang.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pre.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://otu.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://rjw.ivvv.top

Py:   pickle.dumps(obj)
来源：http://fwl.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://yzs.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://qnw.fanxiaobao.xyz

TS:   v8.serialize(obj)        // Node
来源：http://clv.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nef.bbcook.cn

Go:   encoding/gob
来源：http://jtq.jinyuanbaomall.cn

Ruby: Marshal.dump(obj)
来源：http://mxo.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mnj.zhiwuduotai.top

================================================================================
来源：http://wze.shanyushiyangtech.top


<!-- 参考信息 -->