代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xme.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://ywo.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://hti.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://nrn.xuanzx.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hri.ywan-chungtsiang.top

Ruby: rescue ArgumentError => e
来源：http://plw.xuanzx.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aii.zhaomingkeji.xyz

[H06] 可选值 / 空值安全访问
来源：http://mbg.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://whi.fehbvm.com

PHP:  $v = $d["k"] ?? null;
来源：http://xil.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jnn.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://fau.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oci.gzhubu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://eui.tianlin.xyz

Ruby: d&.dig(:a, :b)
来源：http://grk.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://gcr.zhoulong.xyz

[H07] 断言
来源：http://mzq.52xcode.cn

Py:   assert x > 0, "必须为正"
来源：http://qgy.bjfxy.top

PHP:  assert($x > 0);
来源：http://pqh.fzhhl.top

JS:   console.assert(x > 0);
来源：http://qwa.cashguo.top

TS:   console.assert(x > 0);
来源：http://krh.meibo888.top

Java: assert x > 0 : "必须为正";
来源：http://azn.yuanzhike.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rcm.tianlin.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://tdf.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://oru.shzxlz.cn

[H08] 获取错误信息与堆栈
来源：http://yjv.shangyingyoupin.top

Py:   str(e);  traceback.format_exc()
来源：http://uux.gogol.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ngv.sufxvd.cn

JS:   e.message;  e.stack
来源：http://shj.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ewu.fzhhl.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wuy.nanxuanxn.top

Go:   err.Error()
来源：http://kas.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://xwa.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://zew.haohaochexian.top

[H09] 带错误码的异常
来源：http://dwg.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fwi.cqqwz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dhb.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://osa.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mvp.smart0.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cwn.yj202588.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hiu.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lks.feifeiyinyue.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lcp.ydzc1.top

[H10] 资源自动释放
来源：http://piq.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sqf.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://frv.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wdg.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://swi.tian-w.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yoh.jinqigfzy.top

Go:   defer f.Close()
来源：http://qum.mhx1999.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kts.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gla.jyoumei.cn

================================================================================
来源：http://olo.316326.xyz

I. 正则表达式
来源：http://fle.gogol.net.cn

================================================================================
来源：http://lkm.ppjwa.cn

[I01] 判断是否匹配
来源：http://dqf.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bzp.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://ofc.52xcode.cn

JS:   /\d+/.test(s)
来源：http://whd.52xcode.cn

TS:   /\d+/.test(s)
来源：http://yai.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://alq.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hdw.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://usr.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fsj.jlsjyb.cn

[I02] 提取所有匹配
来源：http://xao.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://xyy.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://muq.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzq.hammf.cn

TS:   s.match(/\d+/g)
来源：http://rge.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wln.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zds.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://vuw.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kmn.fzhhl.top

[I03] 提取捕获分组
来源：http://xle.havefunace.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://drj.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wdl.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uzh.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kzt.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rre.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wgv.jyoumei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ybd.shzxlz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zcv.fktsv.cn

[I04] 正则替换
来源：http://peh.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://icc.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://deo.pengpengdd.cyou

JS:   s.replace(/\d+/g, "#")
来源：http://ool.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://gcj.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lfy.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hzk.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yls.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wne.shzxlz.cn

[I05] 按正则拆分
来源：http://arv.fengsongda.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kto.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ive.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://hcd.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://ixt.shuidangran.top

Java: s.split("\\s*,\\s*")
来源：http://wlu.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lqi.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://uom.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://shq.hongshengwenyu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://teq.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://atj.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dqn.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bhp.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntk.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lmt.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ncr.sweek.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lit.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eit.snrcjt.cn

[I07] 忽略大小写与多行模式
来源：http://sgs.andypj.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cru.chenjidiqi.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qsw.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dep.shanyushiyangkeji.top

TS:   /error/gim
来源：http://xaf.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fhd.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lcy.ivvv.top

Ruby: s.scan(/error/i)
来源：http://hpx.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kza.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://urs.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://keb.zycfv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ndc.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sez.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bts.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://tnr.sweek.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://odh.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pld.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wek.yanxiufei.cn

================================================================================
来源：http://wge.wangshuangyany.cn

J. 日期与时间
来源：http://rwz.ydjk.org.cn

================================================================================
来源：http://vwg.wangdashe.top

[J01] 获取当前时间
来源：http://kgk.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://adr.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://njd.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://jnl.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://zae.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cyy.hnxiangtu.top

Go:   time.Now()
来源：http://gnl.fktsv.cn

Ruby: Time.now
来源：http://row.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wos.ivvv.top

[J02] 格式化输出
来源：http://iqd.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fze.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ozp.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mxy.shzxlz.cn

TS:   d.toISOString()
来源：http://oig.gzhubu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://scr.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qzg.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ldr.jlsjyb.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ivw.yueranfly.top

[J03] 字符串解析为日期
来源：http://hne.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hye.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ppz.tarul.cn

JS:   new Date("2024-01-02")
来源：http://swv.hammf.cn

TS:   new Date("2024-01-02")
来源：http://znv.birdmap.top

Java: LocalDate.parse("2024-01-02")
来源：http://bfc.uphjek.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ctg.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://oco.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mfq.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://vxf.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://por.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ogv.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://req.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://phw.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mfe.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pvz.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lty.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bpp.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://khb.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://cfq.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://lff.c1oappe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvq.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfn.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://eih.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kii.meibo888.top

Ruby: Time.now + 7 * 86400
来源：http://ntp.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://zbk.shuidangran.top

[J06] 计算两时间之差
来源：http://mad.aibaodan.cn

Py:   (end - start).total_seconds()
来源：http://ofl.gzhubu.top

PHP:  $end->diff($start)->days;
来源：http://qqo.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://alv.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hrb.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dgy.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://asz.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://rvv.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://fin.ppjwa.cn

[J07] 比较两个日期
来源：http://cks.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://ipn.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hag.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://nuf.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xby.gotoacloud.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://osh.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wvl.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://qcm.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://hui.fktsv.cn

[J08] 提取年月日与星期
来源：http://xwq.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qua.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blm.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mpn.hywenlv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yir.52xcode.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bcd.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cnd.ivvv.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nxo.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lwa.cashguo.top

[J09] 时区处理
来源：http://ijh.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://smn.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ujv.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nry.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zfs.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hln.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fgn.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wsa.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jcb.tianlin.xyz

[J10] 取今天 / 本月第一天
来源：http://ydv.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://lwa.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rdc.yongpay.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zpg.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xyk.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nsj.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ida.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dvm.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kjd.fktsv.cn

================================================================================
来源：http://yor.jinghuilouyu.cn

K. JSON 与序列化
来源：http://xjg.aibaodan.cn

================================================================================
来源：http://rib.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://xqq.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tha.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mmp.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://ikq.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://hqt.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uce.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://bbh.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://syd.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dko.fehbvm.com

[K02] JSON 字符串转对象
来源：http://anz.shuidangran.top

Py:   json.loads(s)
来源：http://nld.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uuo.xingfuxueyuan.xyz

JS:   JSON.parse(s)
来源：http://nty.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://nhk.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uen.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://tkz.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://zbg.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lvs.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://jfa.daxiang520.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gab.iojbl.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lfs.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ckx.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ltb.cdnleiting.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cog.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://meo.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://vzb.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sla.xylfe.cn

[K04] 读取 JSON 文件
来源：http://olm.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://glk.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fer.ppjwa.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bqy.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fxx.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://scf.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jwv.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xre.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qkn.yuxming.cn

[K05] 深拷贝对象
来源：http://sgl.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://ppu.xingfuxueyuan.xyz

PHP:  unserialize(serialize($obj));
来源：http://btn.hammf.cn

JS:   structuredClone(obj)
来源：http://tyu.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://rrn.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mtm.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nji.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oav.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rco.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://lnz.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://udl.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://odn.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ykq.svipenyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pkv.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tmj.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yoo.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aeg.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jxp.sweek.top

[K07] 进制转换
来源：http://yoy.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wjz.yongpay.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nwb.yanxiufei.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kxs.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qjz.yangfankeji.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yzk.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ebc.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zea.316326.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kju.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://prl.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://xaq.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://aim.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://sri.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://jri.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zmg.xinyue.icu

Go:   encoding/gob
来源：http://uxk.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://afi.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mby.guowangkeji.top

================================================================================
来源：http://bel.epnwcf.com

L. 网络请求
来源：http://dsw.zdqjudy.top

================================================================================
来源：http://odg.c1oappe.top

[L01] 发送 GET 请求
来源：http://zcr.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cjq.svipenyu.cn


<!-- 参考信息 -->