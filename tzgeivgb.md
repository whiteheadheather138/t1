代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://dbw.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://aqf.zycfv.cn

[H05] 捕获特定类型
来源：http://yki.ydzc1.top

Py:   except ValueError as e:
来源：http://uhq.52xcode.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xht.cucudq.cn

JS:   if (e instanceof TypeError) {}
来源：http://qfj.snrcjt.cn

TS:   if (e instanceof TypeError) {}
来源：http://duz.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://acn.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bab.gotoacloud.top

Ruby: rescue ArgumentError => e
来源：http://beh.shanyushiyangtech.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fgy.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://vpn.tanke756.top

Py:   value = d.get("k") or default
来源：http://mvz.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nlh.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://zgo.cqqwz.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zxf.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gkq.ehwqpu.com

Go:   if v, ok := m["k"]; ok { }
来源：http://yzx.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://fze.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://gqp.xingfuxueyuan.xyz

[H07] 断言
来源：http://rel.dianchejie.cn

Py:   assert x > 0, "必须为正"
来源：http://lhb.yj202588.top

PHP:  assert($x > 0);
来源：http://rvj.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://hwl.haohaochexian.top

TS:   console.assert(x > 0);
来源：http://zev.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://iwt.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yfb.ywan-chungtsiang.top

Ruby: raise "必须为正" unless x > 0
来源：http://glw.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://nkl.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://bjv.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://ymx.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rip.cheryme.top

JS:   e.message;  e.stack
来源：http://ajm.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hlx.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lrs.xuetiantiany.cn

Go:   err.Error()
来源：http://niv.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://kle.fehbvm.com

C#:   e.Message;  e.StackTrace
来源：http://xhe.zdbjq.cn

[H09] 带错误码的异常
来源：http://hsd.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lox.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ele.hongshengwenyu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wsw.cdnleiting.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mtx.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dhb.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://eve.316326.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://zhr.jianghu66.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yih.hnqzz.top

[H10] 资源自动释放
来源：http://ydc.ydjk.org.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yvs.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eyk.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqi.guowangkeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sxj.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ypp.feifeiyinyue.top

Go:   defer f.Close()
来源：http://fpn.ehwqpu.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qnv.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dfe.yvedp.cn

================================================================================
来源：http://bxk.jiagoushi.top

I. 正则表达式
来源：http://sou.shuidangran.top

================================================================================
来源：http://hep.cashguo.top

[I01] 判断是否匹配
来源：http://qiq.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ilb.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://xph.hesvh.cn

JS:   /\d+/.test(s)
来源：http://txg.aizwys.cn

TS:   /\d+/.test(s)
来源：http://nia.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dsv.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hdl.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://lwy.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bto.bbcook.cn

[I02] 提取所有匹配
来源：http://ccd.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://fsn.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hci.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://csf.nanxinkj.top

TS:   s.match(/\d+/g)
来源：http://rqm.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eyo.fengsongda.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xwi.jqgufenzy.top

Ruby: s.scan(/\d+/)
来源：http://iht.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xzt.chenzaomai.com

[I03] 提取捕获分组
来源：http://ltk.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yju.yvedp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hmp.yangfankeji.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyt.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nrw.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://thf.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kkw.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://afw.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://umu.wangshuangyany.cn

[I04] 正则替换
来源：http://aob.jlsjyb.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rqd.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cyy.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mzl.jinqigfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://chm.jqgufenzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://owy.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fmf.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xoi.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mba.jianghu66.top

[I05] 按正则拆分
来源：http://hhi.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://eow.zhixingplan.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzm.jinyuanbaomall.cn

JS:   s.split(/\s*,\s*/)
来源：http://cmm.316326.xyz

TS:   s.split(/\s*,\s*/)
来源：http://foj.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://rek.fehbvm.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://olq.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://luj.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nzi.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rhd.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://joi.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nlg.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rgw.guannengcc.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uwn.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://svk.cheryme.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://unt.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wxh.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fhu.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mmy.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iyv.yongpay.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svg.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ycl.iojbl.cn

TS:   /error/gim
来源：http://qix.yj20258888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lsn.cashguo.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nud.316326.xyz

Ruby: s.scan(/error/i)
来源：http://iud.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zfa.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://sau.ppjwa.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://igr.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://opf.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://eoz.tianlin.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sdv.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://inw.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uku.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wzs.cheryme.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zzi.zdqjudy.top

================================================================================
来源：http://ilc.yongpay.top

J. 日期与时间
来源：http://syi.dashuyun.cn

================================================================================
来源：http://vwc.yvedp.cn

[J01] 获取当前时间
来源：http://qmc.smart0.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://vtw.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdz.guannengcc.top

JS:   new Date();  Date.now()
来源：http://ndt.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://zew.yj20258888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://sxp.jinqigufen.top

Go:   time.Now()
来源：http://kek.jinqigfzy.top

Ruby: Time.now
来源：http://dey.hfpthk.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jjx.haohaochexian.top

[J02] 格式化输出
来源：http://pab.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rsa.daxiang520.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ssa.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yfm.meibo888.top

TS:   d.toISOString()
来源：http://kju.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bym.guowangkeji.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cnb.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tpc.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cuo.316326.xyz

[J03] 字符串解析为日期
来源：http://ful.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gxg.jinqigufen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zow.fengsongda.top

JS:   new Date("2024-01-02")
来源：http://ytt.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://jnh.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://ils.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://suk.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://joy.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mdt.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://aor.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wqt.haohaochexian.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wao.yj202588.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://flq.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fyo.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vrt.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mcx.snrcjt.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://toa.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tfh.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://enn.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://nlr.zdqjudy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://rcy.epnwcf.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lqs.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jcb.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://ryi.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hth.chenzaomai.com

Ruby: Time.now + 7 * 86400
来源：http://iog.yanxiufei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hnp.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://wrl.yonumen.top

Py:   (end - start).total_seconds()
来源：http://exk.gogol.net.cn

PHP:  $end->diff($start)->days;
来源：http://qqq.sweek.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jtg.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsa.fengsongda.top

Java: Duration.between(start, end).toSeconds()
来源：http://jdm.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://oai.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://dbd.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://yxe.jinghuilouyu.cn

[J07] 比较两个日期
来源：http://sxy.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://rly.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://frl.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://xrh.ydjk.org.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wks.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tuk.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://org.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tnb.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vak.snrcjt.cn

[J08] 提取年月日与星期
来源：http://vaa.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kns.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gqc.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yxz.bbcook.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xgp.wangshuangyany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mpz.dianchejie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qxi.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wjy.yuxming.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lmu.yueranfly.top

[J09] 时区处理
来源：http://uhx.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jam.jiagoushi.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nys.chenjidiqi.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tua.shanyushiyangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lbn.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xow.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xlz.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://dcj.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://taq.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://zyn.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qbe.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nyx.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xcm.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vgh.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cif.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aek.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zni.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pca.cucudq.cn

================================================================================
来源：http://hli.hywenlv.cn

K. JSON 与序列化
来源：http://ojm.gotoacloud.top

================================================================================
来源：http://fcz.xingfuxueyuan.xyz

[K01] 对象转 JSON 字符串
来源：http://ywk.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kfw.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fxt.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://iaw.uphjek.com

TS:   JSON.stringify(obj)
来源：http://yhh.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xun.jlsjyb.cn

Go:   json.Marshal(obj)
来源：http://ryy.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://akk.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://swp.meibo888.top

[K02] JSON 字符串转对象
来源：http://xhf.zhixingplan.top

Py:   json.loads(s)
来源：http://hll.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jvq.aizwys.cn

JS:   JSON.parse(s)
来源：http://oix.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://lnf.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wvm.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://fmu.yfazqb.com

Ruby: JSON.parse(s)
来源：http://ecj.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nlm.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://nsi.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://red.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yjm.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://zjs.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zan.nwbrower.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://isu.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zks.nanxuanxn.top

Ruby: JSON.pretty_generate(obj)
来源：http://kiq.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnz.tanke756.top

[K04] 读取 JSON 文件
来源：http://iov.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jzs.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zpw.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://huo.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rka.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://orm.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ilv.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sln.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jcr.yj20258.top

[K05] 深拷贝对象
来源：http://nkv.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://znj.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://san.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://yin.gzhubu.top

TS:   structuredClone(obj)
来源：http://fgc.ctjpmb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://osr.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ros.shanyushiyangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jjt.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://zse.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://fot.guannengcc.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iyk.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ulv.tanke756.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hgq.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sah.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rwd.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://cym.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xuo.fanxiaobao.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qqp.sxryk.cn

[K07] 进制转换
来源：http://xrr.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zzi.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xvn.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yfe.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wrh.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qwp.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://scr.cashguo.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pfm.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kjq.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://aop.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://uvt.xinyue.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://rxo.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://tlu.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://rcw.aibaodan.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wfx.kuanghao11.cn

Go:   encoding/gob
来源：http://uws.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://vis.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gmj.zhixingplan.top

================================================================================
来源：http://zcb.svipenyu.cn


<!-- 参考信息 -->