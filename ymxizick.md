代发 wailian999

JS:   class MyError extends Error {}
来源：http://qwc.jianghu66.top

TS:   class MyError extends Error {}
来源：http://vco.hammf.cn

Java: class MyException extends RuntimeException {}
来源：http://iyh.fanxiaobao.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ajv.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://mhu.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://piq.mhx1999.top

[H05] 捕获特定类型
来源：http://zyd.redwolf501.top

Py:   except ValueError as e:
来源：http://djy.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xmn.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://tsh.jinqigufen.top

TS:   if (e instanceof TypeError) {}
来源：http://fxh.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://tam.daria6918.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hks.ydjk.org.cn

Ruby: rescue ArgumentError => e
来源：http://jzx.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qwy.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://bnd.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://sbi.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cxr.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://tgn.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://frr.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ksp.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://haa.hammf.cn

Ruby: d&.dig(:a, :b)
来源：http://nhn.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://kra.sxryk.cn

[H07] 断言
来源：http://lmo.tanke756.top

Py:   assert x > 0, "必须为正"
来源：http://ipq.jyoumei.cn

PHP:  assert($x > 0);
来源：http://hoz.cucudq.cn

JS:   console.assert(x > 0);
来源：http://zql.hnxiangtu.top

TS:   console.assert(x > 0);
来源：http://ofk.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://kgn.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://szq.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zmj.xinyue.icu

C#:   Debug.Assert(x > 0);
来源：http://uyb.vqdsnc.cn

[H08] 获取错误信息与堆栈
来源：http://zmr.iojbl.cn

Py:   str(e);  traceback.format_exc()
来源：http://gqi.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gme.nanxinkj.top

JS:   e.message;  e.stack
来源：http://mmt.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cst.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rda.fehbvm.com

Go:   err.Error()
来源：http://zyt.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://jsq.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://bcm.52xcode.cn

[H09] 带错误码的异常
来源：http://ref.jinqigufen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fvv.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://esz.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vum.xinyue.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tvg.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uff.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hhu.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eyy.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zfm.daria6918.cn

[H10] 资源自动释放
来源：http://byr.wangshuangyany.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nht.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hlr.tanke756.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jzk.gzhubu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cqv.chenlongwang.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kkl.shuidangran.top

Go:   defer f.Close()
来源：http://ton.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lxb.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yno.fengsongda.top

================================================================================
来源：http://oyt.hnqzz.top

I. 正则表达式
来源：http://scw.ydjk.org.cn

================================================================================
来源：http://wgc.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://muh.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qom.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://ytq.hnxiangtu.top

JS:   /\d+/.test(s)
来源：http://ewg.zdbjq.cn

TS:   /\d+/.test(s)
来源：http://klb.zdqjudy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uly.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uki.quarkkingdee.top

Ruby: s.match?(/\d+/)
来源：http://ktn.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vxz.havefunace.top

[I02] 提取所有匹配
来源：http://kok.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://nsg.tian-w.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rbe.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yeg.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://apg.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dal.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ymi.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://two.xinyue.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lgd.hcnkem.com

[I03] 提取捕获分组
来源：http://qgw.birdmap.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uqy.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fnm.shangyingyoupin.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aio.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://neo.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://peg.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://saf.ctjpmb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qpv.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://piz.sufxvd.cn

[I04] 正则替换
来源：http://ygb.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hho.dashuyun.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sin.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://ank.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zpg.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://krk.yangfankeji.com

Go:   re.ReplaceAllString(s, "#")
来源：http://gub.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fyu.zhiwuduotai.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://god.jyoumei.cn

[I05] 按正则拆分
来源：http://ant.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qay.zdbjq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wjz.zhiwuduotai.top

JS:   s.split(/\s*,\s*/)
来源：http://vrs.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://upn.shanyushiyangtech.top

Java: s.split("\\s*,\\s*")
来源：http://ztc.xinyue.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iik.cqqwz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fsi.jqgufenzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qun.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lxh.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ryo.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rqy.yonumen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://omt.zhengqikj.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vrj.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bif.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zkp.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cuy.svipenyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iqn.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://cpl.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dtf.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kcv.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ltx.xylfe.cn

TS:   /error/gim
来源：http://tvx.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tct.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aum.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://kpb.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://juu.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://tkm.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jcb.cashguo.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hxy.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ulj.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dmw.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xcc.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rab.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mvw.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://btm.zhongyouzk.top

================================================================================
来源：http://xbx.cucudq.cn

J. 日期与时间
来源：http://cnt.zhiwuduotai.top

================================================================================
来源：http://ltu.yuanzhike.top

[J01] 获取当前时间
来源：http://uex.snrcjt.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ltl.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ahg.aizwys.cn

JS:   new Date();  Date.now()
来源：http://zws.gaohongyu789.top

TS:   new Date();  Date.now()
来源：http://yok.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://tyg.pycfn.com

Go:   time.Now()
来源：http://fqa.daria6918.cn

Ruby: Time.now
来源：http://hjv.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mhh.birdmap.top

[J02] 格式化输出
来源：http://cbl.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lsi.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gdj.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iwq.zhengqikj.top

TS:   d.toISOString()
来源：http://nil.guowangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yki.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jas.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://deq.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vac.ydjk.org.cn

[J03] 字符串解析为日期
来源：http://lzz.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nls.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pdt.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://ucd.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://hvr.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ecq.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mby.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://amv.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rfz.ydzc1.top

[J04] 时间戳与日期互转
来源：http://cuv.jianghu66.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xkf.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zul.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ush.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://qzh.cdnleiting.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nch.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ode.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wgu.zdbjq.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qxl.wangdashe.top

[J05] 时间加减（加 7 天）
来源：http://enn.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://fxd.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hjw.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gny.cdnleiting.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dkk.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://qop.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://syd.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://fgc.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kdy.haohaochexian.top

[J06] 计算两时间之差
来源：http://tsc.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://gos.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://xgp.vqdsnc.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jgd.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lus.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://ibb.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://mer.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://nuh.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://wie.hesvh.cn

[J07] 比较两个日期
来源：http://puj.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://iix.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cju.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ecm.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iso.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qvq.nwbrower.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mbn.zhaomingkeji.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://xbj.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://jop.xingfuxueyuan.xyz

[J08] 提取年月日与星期
来源：http://izj.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lto.jinyuanbaomall.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oct.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://frb.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ygv.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hgz.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xyy.tianlin.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gaz.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rxq.hnqzz.top

[J09] 时区处理
来源：http://bkf.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hao.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vsc.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vjj.ivvv.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://efz.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://aln.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://unf.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lzl.yueranfly.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sof.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://jfx.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yci.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hfr.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qiy.zhongyouzk.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ahr.birdmap.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://alj.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ium.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mqd.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kin.jinghuilouyu.cn

================================================================================
来源：http://zaq.xuetiantiany.cn

K. JSON 与序列化
来源：http://qmb.fanxiaobao.xyz

================================================================================
来源：http://apk.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://ofh.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yvu.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hkd.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://wrp.chenzaomai.com

TS:   JSON.stringify(obj)
来源：http://sia.hywenlv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://twf.yfazqb.com

Go:   json.Marshal(obj)
来源：http://fuu.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bgf.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hon.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://dqh.vqdsnc.cn

Py:   json.loads(s)
来源：http://buu.daxiang520.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iyg.ehwqpu.com

JS:   JSON.parse(s)
来源：http://hze.aizwys.cn

TS:   JSON.parse(s)
来源：http://brz.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ljs.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://fnm.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://qld.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cli.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://qvo.smart0.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://awn.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hbd.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zzv.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fgw.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rca.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jnl.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://sxx.gaohongyu789.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://imn.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://tdh.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fbt.zdqjudy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://olr.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://moy.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bly.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://odl.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lzr.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nzz.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xmz.yfazqb.com

[K05] 深拷贝对象
来源：http://dnp.daxiang520.top

Py:   copy.deepcopy(obj)
来源：http://frk.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://zxj.smart0.xyz

JS:   structuredClone(obj)
来源：http://kqh.zdqjudy.top

TS:   structuredClone(obj)
来源：http://rwc.jyoumei.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jqm.mhx1999.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tjy.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xlx.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://jgr.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://eqr.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zpi.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tui.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lmd.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fae.jinqigfzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ztu.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tki.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kwc.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://okq.gzhubu.top

[K07] 进制转换
来源：http://qoo.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cbe.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lpj.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://crf.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://twl.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://azc.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dfw.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wnp.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tvl.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://jpq.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://cyt.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ltf.yj202588.top

JS:   v8.serialize(obj)        // Node
来源：http://tel.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://lhg.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wui.shanyushiyangkeji.top


<!-- 参考信息 -->