代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://ndq.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://piz.jyoumei.cn

[H05] 捕获特定类型
来源：http://dvn.nanxinkj.top

Py:   except ValueError as e:
来源：http://fcb.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://avh.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://auh.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://amf.zhongyouzk.top

Java: catch (IOException | SQLException e) {}
来源：http://ade.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://chx.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://sxl.9152youxi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://med.zdqjudy.top

[H06] 可选值 / 空值安全访问
来源：http://hha.jianghu66.top

Py:   value = d.get("k") or default
来源：http://nhs.hnqzz.top

PHP:  $v = $d["k"] ?? null;
来源：http://znh.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kdm.havefunace.top

TS:   obj?.a?.b;  d ?? default
来源：http://ote.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://haa.zhengqikj.top

Go:   if v, ok := m["k"]; ok { }
来源：http://kny.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://fpd.haohaochexian.top

C#:   obj?.A?.B ?? default
来源：http://dpz.cheryme.top

[H07] 断言
来源：http://ttw.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://fpr.316326.xyz

PHP:  assert($x > 0);
来源：http://fnf.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://vae.ydzc1.top

TS:   console.assert(x > 0);
来源：http://ahd.nanxuanxn.top

Java: assert x > 0 : "必须为正";
来源：http://nkz.hfpthk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mfi.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://xqh.zhongyouzk.top

C#:   Debug.Assert(x > 0);
来源：http://iqb.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://raw.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://mhy.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eyk.fehbvm.com

JS:   e.message;  e.stack
来源：http://tpj.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ghf.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lpt.aibaodan.cn

Go:   err.Error()
来源：http://yvx.snrcjt.cn

Ruby: e.message;  e.backtrace
来源：http://btl.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://gff.jinghuilouyu.cn

[H09] 带错误码的异常
来源：http://yff.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://frm.yfazqb.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://otz.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rbk.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ose.fzhhl.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tbr.cqqwz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gre.ppjwa.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qkg.shanyushiyangtech.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tgp.jqgfzy.top

[H10] 资源自动释放
来源：http://skr.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dho.zhiwuduotai.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ezq.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://irg.ctjpmb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gyg.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jjh.dashuyun.cn

Go:   defer f.Close()
来源：http://yda.sjlbkw.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qld.yvedp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ocj.jianghu66.top

================================================================================
来源：http://jbm.yj20258.top

I. 正则表达式
来源：http://aln.yonumen.top

================================================================================
来源：http://sxw.vehdjk.com

[I01] 判断是否匹配
来源：http://fyk.daria6918.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gjc.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ona.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://qpf.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://vfm.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kzf.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tzd.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://okg.sxryk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fxj.daxiang520.top

[I02] 提取所有匹配
来源：http://dbh.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://elj.zhijiandao.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vpd.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pbw.sweek.top

TS:   s.match(/\d+/g)
来源：http://knz.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xgu.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lwe.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://vau.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jxk.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://fhv.kuanghao11.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ngg.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cfk.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ezo.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgr.yuxming.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dyt.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lfd.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pnk.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xzs.daxiang520.top

[I04] 正则替换
来源：http://tlp.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lyc.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://flo.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://bkq.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://rib.redwolf501.top

Java: s.replaceAll("\\d+", "#")
来源：http://eee.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hyt.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ljj.hcnkem.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://isq.gzhubu.top

[I05] 按正则拆分
来源：http://pls.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://goe.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xhm.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://qyd.bbcook.cn

TS:   s.split(/\s*,\s*/)
来源：http://gos.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://koy.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vet.yj20258.top

Ruby: s.split(/\s*,\s*/)
来源：http://zkz.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://swx.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nci.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eii.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xyl.epnwcf.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqq.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lso.zhixingplan.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rah.kuanghao11.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mjg.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://shp.jlsjyb.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fvl.tanke756.top

[I07] 忽略大小写与多行模式
来源：http://xke.havefunace.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ufs.ydjk.org.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://onj.pengpengdd.cyou

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rcr.52xcode.cn

TS:   /error/gim
来源：http://gqu.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tns.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rea.ivvv.top

Ruby: s.scan(/error/i)
来源：http://buc.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qoi.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://hdz.shanyushiyangtech.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ost.vehdjk.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uxj.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://num.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ugi.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zmu.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vwh.shuidangran.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dgj.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kgy.quarkkingdee.top

================================================================================
来源：http://xlp.jlsjyb.cn

J. 日期与时间
来源：http://zgf.52xcode.cn

================================================================================
来源：http://wma.sjlbkw.cn

[J01] 获取当前时间
来源：http://mku.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kgh.daria6918.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bwq.fengsongda.top

JS:   new Date();  Date.now()
来源：http://jkv.cheryme.top

TS:   new Date();  Date.now()
来源：http://xzo.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cgk.birdmap.top

Go:   time.Now()
来源：http://dzo.hcnkem.com

Ruby: Time.now
来源：http://sri.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ikb.c1oappe.top

[J02] 格式化输出
来源：http://xma.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szq.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hdu.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://inl.zhijiandao.cn

TS:   d.toISOString()
来源：http://opp.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zze.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cxq.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://guq.haohaochexian.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://map.epnwcf.com

[J03] 字符串解析为日期
来源：http://amr.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bio.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kjm.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://tgj.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://zej.yanxiufei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zmd.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yvy.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://yvq.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://edw.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://qbr.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zqc.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wrb.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wkn.ybcxt.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vlt.ctjpmb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jph.316326.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aww.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://peo.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mrc.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://xev.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://iui.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yro.wangshuangyany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jlp.yj20258888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://khe.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://fgk.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zzt.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://bha.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ymr.yangfankeji.com

[J06] 计算两时间之差
来源：http://paz.ybcxt.top

Py:   (end - start).total_seconds()
来源：http://gan.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://ell.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ovw.yongpay.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://npf.nanxinkj.top

Java: Duration.between(start, end).toSeconds()
来源：http://zac.havefunace.top

Go:   end.Sub(start).Hours()
来源：http://fvb.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://mcc.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://nhx.jqgfzy.top

[J07] 比较两个日期
来源：http://owq.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://itq.vqdsnc.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nnu.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://jnt.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://vjh.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cgs.hfpthk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qzs.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wxf.zhengqikj.top

C#:   d1 < d2;  d1 == d2
来源：http://cor.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://jel.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ygc.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ttp.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://woz.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fgh.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bdv.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vra.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ynq.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pkg.gzhubu.top

[J09] 时区处理
来源：http://iku.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qiy.andypj.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oiz.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsv.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mnr.havefunace.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzs.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gvy.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ffk.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://net.zhaomingkeji.xyz

[J10] 取今天 / 本月第一天
来源：http://lry.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tmg.zhaomingkeji.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gpe.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://otm.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mqy.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vjy.jlsjyb.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://shp.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ize.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ilu.yonumen.top

================================================================================
来源：http://kmj.guowangkeji.top

K. JSON 与序列化
来源：http://fpg.tarul.cn

================================================================================
来源：http://oyi.zhaomingkeji.xyz

[K01] 对象转 JSON 字符串
来源：http://cyc.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ikd.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eox.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://swn.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://tyb.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xte.gzhubu.top

Go:   json.Marshal(obj)
来源：http://hgj.gogol.net.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jdr.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wdz.haohaochexian.top

[K02] JSON 字符串转对象
来源：http://laz.dashuyun.cn

Py:   json.loads(s)
来源：http://fyz.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tjd.zhixingplan.top

JS:   JSON.parse(s)
来源：http://kyv.316326.xyz

TS:   JSON.parse(s)
来源：http://bmi.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gve.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://isg.hammf.cn

Ruby: JSON.parse(s)
来源：http://njm.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jax.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://upu.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mlr.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jvq.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kld.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lyx.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uwp.jianghu66.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fkh.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fkb.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://odo.xuanzx.com

[K04] 读取 JSON 文件
来源：http://wvz.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nkc.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vby.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdh.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mly.gotoacloud.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wzm.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ysz.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://moa.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rxv.tanke756.top

[K05] 深拷贝对象
来源：http://apo.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://fvl.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://mew.epnwcf.com

JS:   structuredClone(obj)
来源：http://cbg.316326.xyz

TS:   structuredClone(obj)
来源：http://ipo.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pme.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://syu.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yjf.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qiu.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://cpd.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tiy.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eaq.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://usw.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pde.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xjd.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aoe.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vbp.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zll.vehdjk.com

[K07] 进制转换
来源：http://hpg.9152youxi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vlv.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jcj.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fdd.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blp.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fbo.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://llh.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afc.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xxi.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://rvu.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://tsg.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bdc.gotoacloud.top

JS:   v8.serialize(obj)        // Node
来源：http://thh.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://fry.cheryme.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eor.sufxvd.cn

Go:   encoding/gob
来源：http://trn.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://lsj.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xfh.yangfankeji.com

================================================================================
来源：http://ttv.xinyue.icu


<!-- 参考信息 -->