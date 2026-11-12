代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://vtk.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://gth.zhijiandao.cn

[H05] 捕获特定类型
来源：http://wiy.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://ocl.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zlq.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://shw.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://eyw.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://pgx.yangfankeji.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pze.ivvv.top

Ruby: rescue ArgumentError => e
来源：http://rab.iojbl.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ikd.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://ctk.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://fiz.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://soc.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fqy.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://wcd.dianchejie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yzv.jinyuanbaomall.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nfz.ctjpmb.com

Ruby: d&.dig(:a, :b)
来源：http://gqh.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://wrz.yanxiufei.cn

[H07] 断言
来源：http://qmi.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://nif.feifeiyinyue.top

PHP:  assert($x > 0);
来源：http://ung.yueranfly.top

JS:   console.assert(x > 0);
来源：http://mii.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://olo.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://wuk.guowangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yot.aibaodan.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mov.fanxiaobao.xyz

C#:   Debug.Assert(x > 0);
来源：http://dqh.chenjidiqi.icu

[H08] 获取错误信息与堆栈
来源：http://eok.birdmap.top

Py:   str(e);  traceback.format_exc()
来源：http://mjp.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://swa.gzhubu.top

JS:   e.message;  e.stack
来源：http://bbw.chenlongwang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hxc.tianlin.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://khp.jinqigfzy.top

Go:   err.Error()
来源：http://kew.xuetiantiany.cn

Ruby: e.message;  e.backtrace
来源：http://vxr.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://pnn.vqdsnc.cn

[H09] 带错误码的异常
来源：http://cqo.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kes.xuetiantiany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jei.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cae.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://faw.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdq.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wnf.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://izz.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://fwj.kuanghao11.cn

[H10] 资源自动释放
来源：http://wca.sxryk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wvf.jyoumei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dwz.smart0.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qrp.yangfankeji.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lth.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sig.chenjidiqi.icu

Go:   defer f.Close()
来源：http://exd.hywenlv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gqr.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zuc.52xcode.cn

================================================================================
来源：http://zhn.cqqwz.cn

I. 正则表达式
来源：http://niy.hongshengwenyu.top

================================================================================
来源：http://mzl.jianghu66.top

[I01] 判断是否匹配
来源：http://uoe.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kme.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://obh.316326.xyz

JS:   /\d+/.test(s)
来源：http://gzl.316326.xyz

TS:   /\d+/.test(s)
来源：http://qrc.sjlbkw.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ktw.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ppz.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://hyy.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dbz.ybcxt.top

[I02] 提取所有匹配
来源：http://mcg.hnqzz.top

Py:   re.findall(r"\d+", s)
来源：http://xry.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jfm.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ibb.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://yfz.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aqh.hysaishi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://luy.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://qca.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xlz.tian-w.cn

[I03] 提取捕获分组
来源：http://rsq.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://grt.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mvl.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oxn.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dfx.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wgx.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jjb.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hix.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igv.dianchejie.cn

[I04] 正则替换
来源：http://gol.sjlbkw.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fpb.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xaj.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://zvs.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://vub.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://edu.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wld.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://idq.zdqjudy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vcl.ehwqpu.com

[I05] 按正则拆分
来源：http://dyb.jinyuanbaomall.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://odb.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kwe.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://cab.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://oyk.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://unu.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ihw.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://zda.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mty.yanxiufei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vnx.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xyf.guannengcc.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ahm.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://svf.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ucn.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fgs.tarul.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cpi.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://flz.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oie.dashuyun.cn

[I07] 忽略大小写与多行模式
来源：http://rsm.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://voj.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gry.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eyz.zdbjq.cn

TS:   /error/gim
来源：http://mxy.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gbm.zhixingplan.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hfk.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://vxg.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cot.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://ekp.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gvq.hongshengwenyu.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wkd.yvedp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://set.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jmn.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://mki.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dkk.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mzw.zdbjq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tbd.yueranfly.top

================================================================================
来源：http://pki.xinyue.icu

J. 日期与时间
来源：http://isr.yj20258888.top

================================================================================
来源：http://cns.yvedp.cn

[J01] 获取当前时间
来源：http://wbd.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qjv.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dfl.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://goa.yj20258.top

TS:   new Date();  Date.now()
来源：http://zlt.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sja.zdqjudy.top

Go:   time.Now()
来源：http://hpq.zdqjudy.top

Ruby: Time.now
来源：http://nba.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jqa.daria6918.cn

[J02] 格式化输出
来源：http://ulv.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oow.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boo.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tfg.yj202588.top

TS:   d.toISOString()
来源：http://qmh.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mro.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ojd.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjs.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dsj.jqgfzy.top

[J03] 字符串解析为日期
来源：http://qhp.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://axa.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nkp.yongpay.top

JS:   new Date("2024-01-02")
来源：http://wcu.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://suk.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://dam.shuidangran.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://elo.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://omv.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hjp.yangfankeji.com

[J04] 时间戳与日期互转
来源：http://nlq.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xeq.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vry.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iou.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qdy.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bbo.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tgd.hnxiangtu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jaj.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iet.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://vba.cqqwz.cn

Py:   now + timedelta(days=7)
来源：http://ixx.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://jmw.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mbw.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://auu.jlsjyb.cn

Java: LocalDate.now().plusDays(7)
来源：http://agu.zdbjq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ihs.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://cym.vqdsnc.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lgf.jianghu66.top

[J06] 计算两时间之差
来源：http://krf.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://yxs.jlsjyb.cn

PHP:  $end->diff($start)->days;
来源：http://wsz.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hgm.cdnleiting.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ynn.zhoulong.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://jnv.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://qtj.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://por.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://muo.cheryme.top

[J07] 比较两个日期
来源：http://qam.hnqzz.top

Py:   d1 < d2;  d1 == d2
来源：http://hrb.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzx.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://vph.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://pub.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ekb.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wnj.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://ttt.dianchejie.cn

C#:   d1 < d2;  d1 == d2
来源：http://paw.zhengqikj.top

[J08] 提取年月日与星期
来源：http://inw.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nev.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://auk.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yyq.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gry.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txs.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://usd.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mxt.zhongyouzk.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pfs.shuidangran.top

[J09] 时区处理
来源：http://fvy.guowangkeji.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zkh.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tpl.iojbl.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://asu.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdd.shuidangran.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pcn.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yfv.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ann.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nqs.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://moh.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gbd.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fhb.guowangkeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://twj.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kte.zycfv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://izf.fanxiaobao.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://elk.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://idj.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfp.cqqwz.cn

================================================================================
来源：http://anm.zdqjudy.top

K. JSON 与序列化
来源：http://ufm.tianlin.xyz

================================================================================
来源：http://zxy.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://uwk.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ies.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mum.birdmap.top

JS:   JSON.stringify(obj)
来源：http://rav.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://rod.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gyp.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://wws.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://qsw.hesvh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pmq.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://sjb.ehwqpu.com

Py:   json.loads(s)
来源：http://mqr.hnqzz.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vis.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://jei.fktsv.cn

TS:   JSON.parse(s)
来源：http://ktn.sweek.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wan.sweek.top

Go:   json.Unmarshal(data, &v)
来源：http://nie.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://gwu.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://obq.feifeiyinyue.top

[K03] JSON 美化输出（带缩进）
来源：http://pee.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fml.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://adw.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vfv.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://dwb.sysykeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rpw.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://our.iojbl.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zlw.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ctg.redwolf501.top

[K04] 读取 JSON 文件
来源：http://jdj.ybcxt.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ata.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xeo.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cet.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rea.hesvh.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvj.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iha.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rjo.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mpn.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://jrx.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://ybz.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://kak.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://xez.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://ubv.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vmn.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mlu.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yas.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://uuv.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://bwl.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xgy.zhiwuduotai.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gib.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yeu.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ege.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hzo.aibaodan.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://myh.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://icv.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cuf.zdbjq.cn

[K07] 进制转换
来源：http://ntj.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sim.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://czh.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hop.hnxiangtu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://afn.ywan-chungtsiang.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pfz.jinghuilouyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qcy.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lgb.ppjwa.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hie.snrcjt.cn

[K08] 二进制序列化（非 JSON）
来源：http://zai.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://sqc.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rgw.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://cgn.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://zut.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jbj.fktsv.cn

Go:   encoding/gob
来源：http://xnr.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://jfe.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://adm.tianlin.xyz

================================================================================
来源：http://kmo.zhoulong.xyz


<!-- 参考信息 -->