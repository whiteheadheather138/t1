代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mii.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://mrz.hnqzz.top

TS:   if (e instanceof TypeError) {}
来源：http://lgs.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://dzc.shzxlz.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eyj.jinghuilouyu.cn

Ruby: rescue ArgumentError => e
来源：http://ozs.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bkx.uphjek.com

[H06] 可选值 / 空值安全访问
来源：http://bqb.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://syx.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://lag.sysykeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://vsw.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://wgi.aizwys.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xff.ywan-chungtsiang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ajp.jinqigufen.top

Ruby: d&.dig(:a, :b)
来源：http://ose.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://qax.guannengcc.top

[H07] 断言
来源：http://gpj.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://dzi.andypj.xyz

PHP:  assert($x > 0);
来源：http://pdx.cheryme.top

JS:   console.assert(x > 0);
来源：http://ssj.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://cvp.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://vpb.jinqigfzy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lpj.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://vfd.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://plr.gotoacloud.top

[H08] 获取错误信息与堆栈
来源：http://dju.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://cyv.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gha.jiagoushi.top

JS:   e.message;  e.stack
来源：http://fst.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eop.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://izw.bbcook.cn

Go:   err.Error()
来源：http://ezo.xinyue.icu

Ruby: e.message;  e.backtrace
来源：http://vcl.havefunace.top

C#:   e.Message;  e.StackTrace
来源：http://uxb.chenjidiqi.icu

[H09] 带错误码的异常
来源：http://bbh.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wld.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ytl.chenzaomai.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sno.ywan-chungtsiang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ueh.pengpengdd.cyou

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xmw.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://scu.yueranfly.top

Ruby: raise MyError.new("fail", 500)
来源：http://jhe.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://asi.zhixingplan.top

[H10] 资源自动释放
来源：http://gmt.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vsm.hnqzz.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hvc.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ver.zhaomingkeji.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uqv.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vht.kuanghao11.cn

Go:   defer f.Close()
来源：http://szy.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jwj.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pka.jiagoushi.top

================================================================================
来源：http://wmt.shanyushiyangtech.top

I. 正则表达式
来源：http://ksv.snrcjt.cn

================================================================================
来源：http://yyw.gogol.net.cn

[I01] 判断是否匹配
来源：http://qqj.gzhubu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ssu.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://tco.hesvh.cn

JS:   /\d+/.test(s)
来源：http://pws.birdmap.top

TS:   /\d+/.test(s)
来源：http://piz.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oyb.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qjl.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://jfc.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nfk.pycfn.com

[I02] 提取所有匹配
来源：http://lnk.ivvv.top

Py:   re.findall(r"\d+", s)
来源：http://agi.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://out.hnxiangtu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fmy.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://lit.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lts.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zoe.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://gtz.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iod.yvedp.cn

[I03] 提取捕获分组
来源：http://jzg.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wky.nanxinkj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tzt.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lft.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sej.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ivc.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zzw.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://phw.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://auf.yangfankeji.com

[I04] 正则替换
来源：http://eij.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mni.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rjh.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ith.jlsjyb.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xtc.jinqigfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://zyb.hnqzz.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cbm.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ign.jinghuilouyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pbx.cdnleiting.top

[I05] 按正则拆分
来源：http://ugc.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://kjt.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hwj.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://spt.hysaishi.cn

TS:   s.split(/\s*,\s*/)
来源：http://avw.bjfxy.top

Java: s.split("\\s*,\\s*")
来源：http://wiv.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xfb.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xol.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pps.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xld.shangyingyoupin.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rxb.yangfankeji.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fck.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://njm.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wlr.jinqigufen.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rgj.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qig.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://toq.nwbrower.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lin.iojbl.cn

[I07] 忽略大小写与多行模式
来源：http://yik.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tdv.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyg.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://coo.wangdashe.top

TS:   /error/gim
来源：http://vof.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ibb.shzxlz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iqj.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://mpm.birdmap.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vkz.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://mbf.svipenyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gni.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aqv.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wql.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tpe.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qdh.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nlm.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwm.zhijiandao.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rxd.zdbjq.cn

================================================================================
来源：http://iaf.ivvv.top

J. 日期与时间
来源：http://quc.jqgfzy.top

================================================================================
来源：http://wpo.vqdsnc.cn

[J01] 获取当前时间
来源：http://rih.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://jkp.fanxiaobao.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rac.kuanghao11.cn

JS:   new Date();  Date.now()
来源：http://msf.ehwqpu.com

TS:   new Date();  Date.now()
来源：http://xsx.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://sac.hcnkem.com

Go:   time.Now()
来源：http://yhn.sweek.top

Ruby: Time.now
来源：http://mjt.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hap.xuanzx.com

[J02] 格式化输出
来源：http://pdu.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dkv.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hoo.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ddy.gzhubu.top

TS:   d.toISOString()
来源：http://rvv.hnqzz.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qwa.ctjpmb.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pyg.hysaishi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oia.feifeiyinyue.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uyr.yvedp.cn

[J03] 字符串解析为日期
来源：http://als.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://soc.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jgp.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://qcj.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://jol.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://oun.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bod.jiagoushi.top

Ruby: Date.parse("2024-01-02")
来源：http://oku.shuidangran.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dus.fzhhl.top

[J04] 时间戳与日期互转
来源：http://tco.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nqb.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wrb.52xcode.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tdr.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pgf.zycfv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zyh.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gsy.gzhubu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aqh.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hcv.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://cvo.fanxiaobao.xyz

Py:   now + timedelta(days=7)
来源：http://dmf.52xcode.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wju.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vwb.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcu.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://mtd.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qsq.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://nny.guowangkeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://pyz.redwolf501.top

[J06] 计算两时间之差
来源：http://odb.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://tyl.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://fej.havefunace.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cmm.quarkkingdee.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gqq.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://xvs.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://odm.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://tjb.jqgufenzy.top

C#:   (end - start).TotalSeconds
来源：http://wgy.andypj.xyz

[J07] 比较两个日期
来源：http://hvg.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://vfd.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ksd.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fop.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://aoa.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sjp.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxc.vqdsnc.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lln.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://oeq.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://ndn.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cfm.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://myx.jinyuanbaomall.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ztk.pengpengdd.cyou

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zzg.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hlr.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qgx.gogol.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dzf.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hhd.ctjpmb.com

[J09] 时区处理
来源：http://qhm.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mgt.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://guo.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ifz.ywan-chungtsiang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zkl.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nej.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kbt.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dqa.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mku.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://dpv.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wvn.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uan.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylb.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kjp.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wtn.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ydq.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uzv.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lyq.zhijiandao.cn

================================================================================
来源：http://lft.yfazqb.com

K. JSON 与序列化
来源：http://ogq.yj202588.top

================================================================================
来源：http://ofn.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://hgs.tianlin.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qmn.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nvc.sweek.top

JS:   JSON.stringify(obj)
来源：http://ceb.cheryme.top

TS:   JSON.stringify(obj)
来源：http://fer.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yeg.vehdjk.com

Go:   json.Marshal(obj)
来源：http://ssy.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ast.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://csd.epnwcf.com

[K02] JSON 字符串转对象
来源：http://eph.ctjpmb.com

Py:   json.loads(s)
来源：http://nqk.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dpl.gogol.net.cn

JS:   JSON.parse(s)
来源：http://vej.yj20258.top

TS:   JSON.parse(s)
来源：http://clk.bbcook.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ooz.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://ibe.daxiang520.top

Ruby: JSON.parse(s)
来源：http://fjk.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pfl.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://ttd.yuanzhike.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://woq.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qgu.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dva.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kpp.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sck.jyoumei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jfz.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jct.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ixf.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://rgq.tianlin.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://woh.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xiq.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jgv.yuxming.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xne.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gwx.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qae.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mew.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://drx.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://bqf.fengsongda.top

Py:   copy.deepcopy(obj)
来源：http://nlx.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://ayl.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://iyc.sysykeji.top

TS:   structuredClone(obj)
来源：http://hbm.nanxuanxn.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lcu.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xtv.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cma.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xge.xuanzx.com

[K06] 解析 URL 查询串
来源：http://zjb.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lho.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uvy.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qut.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izi.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bbt.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hfp.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://boo.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gam.fzhhl.top

[K07] 进制转换
来源：http://ygg.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kbv.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xvl.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rfr.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zfz.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ejd.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gyd.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ilt.c1oappe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jzn.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://xzv.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://qgf.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://tdp.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://saj.ydjk.org.cn

TS:   v8.serialize(obj)        // Node
来源：http://ocp.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://itt.yj202588.top

Go:   encoding/gob
来源：http://svu.xylfe.cn

Ruby: Marshal.dump(obj)
来源：http://feb.xinyue.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bvd.dashuyun.cn

================================================================================
来源：http://exr.chenjidiqi.icu

L. 网络请求
来源：http://jhl.cucudq.cn

================================================================================
来源：http://qra.cqqwz.cn

[L01] 发送 GET 请求
来源：http://fmp.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bnh.shanyushiyangtech.top


<!-- 参考信息 -->