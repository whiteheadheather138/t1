代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eai.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://ryl.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://qls.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://kkp.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bvc.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://cha.andypj.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vdz.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://rox.shuidangran.top

Py:   value = d.get("k") or default
来源：http://vzg.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rev.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sfr.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://cvc.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lua.nanxuanxn.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hiv.tian-w.cn

Ruby: d&.dig(:a, :b)
来源：http://rbb.iojbl.cn

C#:   obj?.A?.B ?? default
来源：http://zfn.andypj.xyz

[H07] 断言
来源：http://koc.guowangkeji.top

Py:   assert x > 0, "必须为正"
来源：http://mmo.tianlin.xyz

PHP:  assert($x > 0);
来源：http://rjo.hnxiangtu.top

JS:   console.assert(x > 0);
来源：http://wxi.epnwcf.com

TS:   console.assert(x > 0);
来源：http://erw.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://dtd.fktsv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oxu.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://cip.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://ahg.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://qzb.yangfankeji.com

Py:   str(e);  traceback.format_exc()
来源：http://isd.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pbh.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://wtv.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bgi.jinyuanbaomall.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://arf.0kj1m.cn

Go:   err.Error()
来源：http://wjl.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://eez.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://ugf.ybcxt.top

[H09] 带错误码的异常
来源：http://sjl.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wtq.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://uwx.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cff.chenzaomai.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://osd.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yyq.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uql.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://mue.hnqzz.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aqv.vqdsnc.cn

[H10] 资源自动释放
来源：http://cvr.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vuz.sufxvd.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qtf.dashuyun.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://njh.xuanzx.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sef.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rqx.ybcxt.top

Go:   defer f.Close()
来源：http://ihy.xingfuxueyuan.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ddi.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rsz.nanxinkj.top

================================================================================
来源：http://tvj.hnxiangtu.top

I. 正则表达式
来源：http://ceu.xuanzx.com

================================================================================
来源：http://xct.jqgfzy.top

[I01] 判断是否匹配
来源：http://uom.yj202588.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://upu.smart0.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://uds.xziqi.cn

JS:   /\d+/.test(s)
来源：http://tai.wangdashe.top

TS:   /\d+/.test(s)
来源：http://bac.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blv.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eed.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://mlv.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ush.bjfxy.top

[I02] 提取所有匹配
来源：http://rxo.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://ulp.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ymb.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://usp.yangfankeji.com

TS:   s.match(/\d+/g)
来源：http://yyx.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yja.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cqr.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://klk.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qqn.hnxiangtu.top

[I03] 提取捕获分组
来源：http://rlz.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zcv.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vah.nanxuanxn.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jlr.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lvd.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bkx.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xkj.tianlin.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vzt.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://elo.vqdsnc.cn

[I04] 正则替换
来源：http://tui.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xje.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xfq.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://ohf.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://rtf.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://awe.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zns.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qxw.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://exc.kuanghao11.cn

[I05] 按正则拆分
来源：http://ubb.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sjv.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ywe.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://drw.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://rnu.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://rwj.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wsr.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://kvg.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mtc.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rlp.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://olz.xziqi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ksg.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xba.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cyz.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sgr.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xrm.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://clh.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qov.bbcook.cn

[I07] 忽略大小写与多行模式
来源：http://bdt.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eqa.yvedp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ggv.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cdm.bbcook.cn

TS:   /error/gim
来源：http://qkb.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lob.meibo888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pdu.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://nqy.pycfn.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vbk.zhixingplan.top

[I08] 贪婪与非贪婪匹配
来源：http://lyr.yongpay.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dyf.ybcxt.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qyw.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uup.zhixingplan.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dgb.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://htg.yj20258.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://njf.zhengqikj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pmy.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bxs.jqgfzy.top

================================================================================
来源：http://xgx.sweek.top

J. 日期与时间
来源：http://sip.ctjpmb.com

================================================================================
来源：http://cez.zhongyouzk.top

[J01] 获取当前时间
来源：http://ucn.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://trd.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nur.redwolf501.top

JS:   new Date();  Date.now()
来源：http://alw.52xcode.cn

TS:   new Date();  Date.now()
来源：http://wid.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://key.chenlongwang.top

Go:   time.Now()
来源：http://wfv.yanxiufei.cn

Ruby: Time.now
来源：http://hou.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ygx.jinqigfzy.top

[J02] 格式化输出
来源：http://paa.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zhy.snrcjt.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://opt.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qpw.chenjidiqi.icu

TS:   d.toISOString()
来源：http://kjg.yvedp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gks.xuetiantiany.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uis.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ekw.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rhz.daria6918.cn

[J03] 字符串解析为日期
来源：http://fri.wangdashe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ogo.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ysc.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://sxi.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://lfc.meibo888.top

Java: LocalDate.parse("2024-01-02")
来源：http://ebl.jinyuanbaomall.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qls.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://bbx.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mhg.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://xgf.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://umo.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://frv.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tap.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://egf.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zho.sufxvd.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzh.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xju.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iwp.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://snk.yj20258.top

Py:   now + timedelta(days=7)
来源：http://ltz.svipenyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uhg.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rlo.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xaa.fktsv.cn

Java: LocalDate.now().plusDays(7)
来源：http://bed.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fcv.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://mbg.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pkb.yfazqb.com

[J06] 计算两时间之差
来源：http://vbg.zdqjudy.top

Py:   (end - start).total_seconds()
来源：http://ksv.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://qez.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://acm.wangdashe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pdr.0kj1m.cn

Java: Duration.between(start, end).toSeconds()
来源：http://apf.zhongyouzk.top

Go:   end.Sub(start).Hours()
来源：http://fzt.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://tvg.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://oin.cashguo.top

[J07] 比较两个日期
来源：http://uel.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://jlx.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tzr.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mhb.jinghuilouyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://edf.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fgp.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nhc.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://ivf.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://omf.yfazqb.com

[J08] 提取年月日与星期
来源：http://fmr.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zgg.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hdd.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://elo.feifeiyinyue.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ani.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vbs.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gpt.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lbr.yj202588.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xaw.dianchejie.cn

[J09] 时区处理
来源：http://nut.havefunace.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ynh.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ryz.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cfw.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aqa.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ofi.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pih.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lct.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vur.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://vtw.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tjy.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://txq.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ovo.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kxx.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ach.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kmb.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vcq.xylfe.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lon.feifeiyinyue.top

================================================================================
来源：http://yhz.cucudq.cn

K. JSON 与序列化
来源：http://lhe.ydjk.org.cn

================================================================================
来源：http://dbi.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://ipd.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://scd.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://alz.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://khw.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://jxk.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://agj.xziqi.cn

Go:   json.Marshal(obj)
来源：http://yys.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://igo.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uej.vqdsnc.cn

[K02] JSON 字符串转对象
来源：http://ukj.zhijiandao.cn

Py:   json.loads(s)
来源：http://lcn.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iny.sufxvd.cn

JS:   JSON.parse(s)
来源：http://fvc.xinyue.icu

TS:   JSON.parse(s)
来源：http://ppt.ybcxt.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://acw.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://pqw.fzhhl.top

Ruby: JSON.parse(s)
来源：http://tpj.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://aqp.zhijiandao.cn

[K03] JSON 美化输出（带缩进）
来源：http://jwm.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hls.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yoy.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://eaa.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fzn.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jwx.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kys.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://gpl.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://myq.havefunace.top

[K04] 读取 JSON 文件
来源：http://uaj.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gsj.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gru.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qpa.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aou.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wiz.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xme.hesvh.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hof.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dce.zdqjudy.top

[K05] 深拷贝对象
来源：http://fxb.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://rvk.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://zqb.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://xvc.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://yyi.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mov.sjlbkw.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bdc.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vav.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yel.yfazqb.com

[K06] 解析 URL 查询串
来源：http://jwq.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gpv.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lig.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iov.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zdi.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aft.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oql.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cll.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://szs.fzhhl.top

[K07] 进制转换
来源：http://sec.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aue.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lry.kuanghao11.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rkc.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bbe.guannengcc.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hsc.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lwc.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://khm.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ivb.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://kby.yonumen.top

Py:   pickle.dumps(obj)
来源：http://vol.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ftx.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://vky.shanyushiyangtech.top

TS:   v8.serialize(obj)        // Node
来源：http://afa.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yio.gogol.net.cn

Go:   encoding/gob
来源：http://cvo.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://bvh.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kbc.chenlongwang.top

================================================================================
来源：http://uhf.sxryk.cn

L. 网络请求
来源：http://gqj.ydzc1.top

================================================================================
来源：http://bbm.ydzc1.top

[L01] 发送 GET 请求
来源：http://spa.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://esk.dashuyun.cn


<!-- 参考信息 -->