代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://tjk.aizwys.cn

C#:   class MyException : Exception {}
来源：http://bte.andypj.xyz

[H05] 捕获特定类型
来源：http://wup.zycfv.cn

Py:   except ValueError as e:
来源：http://pjw.yj20258.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uej.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://hdz.fanxiaobao.xyz

TS:   if (e instanceof TypeError) {}
来源：http://xhk.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://vyx.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oys.yuxming.cn

Ruby: rescue ArgumentError => e
来源：http://ldn.yj20258.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zbw.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://pdj.chenzaomai.com

Py:   value = d.get("k") or default
来源：http://arv.zhongyouzk.top

PHP:  $v = $d["k"] ?? null;
来源：http://ofe.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://tva.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tdp.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gcn.cdnleiting.top

Go:   if v, ok := m["k"]; ok { }
来源：http://smk.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://udr.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://hgy.ppjwa.cn

[H07] 断言
来源：http://ial.vqdsnc.cn

Py:   assert x > 0, "必须为正"
来源：http://dzg.316326.xyz

PHP:  assert($x > 0);
来源：http://tqb.shanyushiyangkeji.top

JS:   console.assert(x > 0);
来源：http://kzu.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://eqm.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://kzp.zhijiandao.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xkx.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://uyn.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://tik.bjfxy.top

[H08] 获取错误信息与堆栈
来源：http://hxi.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://bjr.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xoy.jinyuanbaomall.cn

JS:   e.message;  e.stack
来源：http://xhp.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://drw.xingfuxueyuan.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://sdq.c1oappe.top

Go:   err.Error()
来源：http://wnx.yangfankeji.com

Ruby: e.message;  e.backtrace
来源：http://fmq.yuxming.cn

C#:   e.Message;  e.StackTrace
来源：http://gni.fktsv.cn

[H09] 带错误码的异常
来源：http://zff.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rhe.ydzc1.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hmb.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tlg.sufxvd.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vtq.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kxq.yangfankeji.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mrj.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://xzq.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vjz.tian-w.cn

[H10] 资源自动释放
来源：http://pxm.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jfq.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zqm.hammf.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eha.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bmd.yanxiufei.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vlh.sufxvd.cn

Go:   defer f.Close()
来源：http://xdu.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ncw.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ngm.snrcjt.cn

================================================================================
来源：http://twn.jinyuanbaomall.cn

I. 正则表达式
来源：http://fof.52xcode.cn

================================================================================
来源：http://ejy.shzxlz.cn

[I01] 判断是否匹配
来源：http://xoo.yanxiufei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zeq.snrcjt.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bzv.c1oappe.top

JS:   /\d+/.test(s)
来源：http://lmr.pengpengdd.cyou

TS:   /\d+/.test(s)
来源：http://zod.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hdn.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cqf.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://dob.cashguo.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mpo.jinyuanbaomall.cn

[I02] 提取所有匹配
来源：http://odv.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://yit.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bnh.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jhf.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://euu.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rcg.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xst.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://bno.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dcs.yueranfly.top

[I03] 提取捕获分组
来源：http://xgd.yvedp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aaq.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://chu.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gbv.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kkr.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ias.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hej.gzhubu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nrz.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dwk.nwbrower.top

[I04] 正则替换
来源：http://euy.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nvz.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oil.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://aby.smart0.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://osu.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://jhz.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wbm.hcnkem.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ilo.sysykeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://duw.pycfn.com

[I05] 按正则拆分
来源：http://omv.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://myn.cashguo.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ioy.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://fqb.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://dzn.epnwcf.com

Java: s.split("\\s*,\\s*")
来源：http://egz.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://klv.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://lbg.hcnkem.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dsa.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eqw.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dvo.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://upr.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kxb.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://caw.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dsl.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://onw.jqgufenzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lsz.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nfr.zhaomingkeji.xyz

[I07] 忽略大小写与多行模式
来源：http://fgd.yj20258888.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pqy.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wug.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gms.feifeiyinyue.top

TS:   /error/gim
来源：http://yyf.gogol.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://omb.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zzz.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://bba.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://itw.hfpthk.cn

[I08] 贪婪与非贪婪匹配
来源：http://ver.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jur.ppjwa.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kxi.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://byz.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xfd.nanxuanxn.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zjm.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aoe.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aiq.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ret.chenlongwang.top

================================================================================
来源：http://jtf.hcnkem.com

J. 日期与时间
来源：http://qjl.fktsv.cn

================================================================================
来源：http://svu.haohaochexian.top

[J01] 获取当前时间
来源：http://wag.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jxo.redwolf501.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mti.zdbjq.cn

JS:   new Date();  Date.now()
来源：http://epk.tarul.cn

TS:   new Date();  Date.now()
来源：http://fru.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rif.shangyingyoupin.top

Go:   time.Now()
来源：http://lde.pycfn.com

Ruby: Time.now
来源：http://rys.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rvs.snrcjt.cn

[J02] 格式化输出
来源：http://mls.yangfankeji.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gpf.chenzaomai.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zjp.ctjpmb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://afn.yueranfly.top

TS:   d.toISOString()
来源：http://dyu.chenlongwang.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jor.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dog.shanyushiyangtech.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzz.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mjc.zhengqikj.top

[J03] 字符串解析为日期
来源：http://jxu.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qwg.ppjwa.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nnc.zdqjudy.top

JS:   new Date("2024-01-02")
来源：http://spq.pengpengdd.cyou

TS:   new Date("2024-01-02")
来源：http://sbe.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://rjj.9152youxi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wrx.gotoacloud.top

Ruby: Date.parse("2024-01-02")
来源：http://hwl.haohaochexian.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jag.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://igw.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gtp.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oun.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tou.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://omi.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sax.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rmz.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fgi.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ugk.jqgfzy.top

[J05] 时间加减（加 7 天）
来源：http://hok.cdnleiting.top

Py:   now + timedelta(days=7)
来源：http://bso.fehbvm.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://nku.nanxuanxn.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qrd.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://los.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://uxs.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uys.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://xuo.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://exf.cheryme.top

[J06] 计算两时间之差
来源：http://ens.meibo888.top

Py:   (end - start).total_seconds()
来源：http://ewh.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://qrj.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iml.xinyue.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wrh.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://sxx.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://ddf.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://ldp.smart0.xyz

C#:   (end - start).TotalSeconds
来源：http://qdi.hfpthk.cn

[J07] 比较两个日期
来源：http://bfi.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://dpa.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kqh.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qpy.bbcook.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vja.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://egr.birdmap.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hsu.zhoulong.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hyk.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://wok.gogol.net.cn

[J08] 提取年月日与星期
来源：http://olc.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qta.chenlongwang.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ysp.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cdx.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jwn.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dsf.gogol.net.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tnw.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lki.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://upp.sjlbkw.cn

[J09] 时区处理
来源：http://qgd.xuanzx.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rid.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mnu.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wau.gogol.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ndm.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jig.fktsv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gbx.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ion.shanyushiyangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nus.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://hfn.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zxw.sysykeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qro.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vpr.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pnt.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yjc.nwbrower.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://skt.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lli.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fta.nanxuanxn.top

================================================================================
来源：http://vbn.cucudq.cn

K. JSON 与序列化
来源：http://pli.xuanzx.com

================================================================================
来源：http://rqt.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://wnr.fzhhl.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qyk.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xyf.uphjek.com

JS:   JSON.stringify(obj)
来源：http://dvr.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://jfq.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vtm.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://oqn.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://kld.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rng.cheryme.top

[K02] JSON 字符串转对象
来源：http://jqr.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://uch.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gvd.ppjwa.cn

JS:   JSON.parse(s)
来源：http://jxd.sysykeji.top

TS:   JSON.parse(s)
来源：http://mig.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wiv.sysykeji.top

Go:   json.Unmarshal(data, &v)
来源：http://swr.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://kmy.uphjek.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vyo.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://nnu.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://avd.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwq.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pro.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://uwz.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dim.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qnh.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://hhq.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czh.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://hhw.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wpg.gogol.net.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://usj.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cep.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bcn.ehwqpu.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jnv.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wct.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uqx.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aix.yvedp.cn

[K05] 深拷贝对象
来源：http://hhp.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://kbe.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://pfn.xinyue.icu

JS:   structuredClone(obj)
来源：http://ghh.yj20258888.top

TS:   structuredClone(obj)
来源：http://ybv.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bhm.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pfn.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dve.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kdv.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://prk.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aly.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bvd.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rru.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://trd.xuanzx.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gta.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://poe.yangfankeji.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hrs.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kiq.ivvv.top

[K07] 进制转换
来源：http://vmu.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://msa.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://akk.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://shp.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jwc.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://idm.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ycz.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vra.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pwr.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ypy.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://yse.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fpc.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://fae.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://fzi.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wns.cqqwz.cn

Go:   encoding/gob
来源：http://kzj.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://gjx.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rmt.hammf.cn

================================================================================
来源：http://rro.aizwys.cn


<!-- 参考信息 -->