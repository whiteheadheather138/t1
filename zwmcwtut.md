代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://zsu.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://jhz.jinyuanbaomall.cn

[H05] 捕获特定类型
来源：http://opx.yj20258888.top

Py:   except ValueError as e:
来源：http://xyr.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hpr.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ddz.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://inq.tianlin.xyz

Java: catch (IOException | SQLException e) {}
来源：http://hvp.gogol.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pku.shangyingyoupin.top

Ruby: rescue ArgumentError => e
来源：http://pwx.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://czy.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://fqz.dashuyun.cn

Py:   value = d.get("k") or default
来源：http://tfn.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ulw.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://zxk.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://cci.gzhubu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://foz.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://bts.bjfxy.top

Ruby: d&.dig(:a, :b)
来源：http://ymu.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://xqy.yanxiufei.cn

[H07] 断言
来源：http://ycz.xinyue.icu

Py:   assert x > 0, "必须为正"
来源：http://srd.hammf.cn

PHP:  assert($x > 0);
来源：http://uhd.gzhubu.top

JS:   console.assert(x > 0);
来源：http://fby.snrcjt.cn

TS:   console.assert(x > 0);
来源：http://oxo.aibaodan.cn

Java: assert x > 0 : "必须为正";
来源：http://npw.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ejs.shanyushiyangtech.top

Ruby: raise "必须为正" unless x > 0
来源：http://yrn.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://jdk.guowangkeji.top

[H08] 获取错误信息与堆栈
来源：http://xwz.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://bff.jinqigufen.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tgj.zhixingplan.top

JS:   e.message;  e.stack
来源：http://def.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qtu.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gqc.sysykeji.top

Go:   err.Error()
来源：http://smd.kuanghao11.cn

Ruby: e.message;  e.backtrace
来源：http://ntl.hongshengwenyu.top

C#:   e.Message;  e.StackTrace
来源：http://rpm.aibaodan.cn

[H09] 带错误码的异常
来源：http://qps.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cac.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oln.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://idv.hysaishi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xdf.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dcv.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://afo.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://kqp.jqgufenzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://clf.ehwqpu.com

[H10] 资源自动释放
来源：http://vmo.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sqy.hysaishi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yzf.fehbvm.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iwp.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nfo.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vrm.jyoumei.cn

Go:   defer f.Close()
来源：http://hcd.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://svm.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdy.jqgufenzy.top

================================================================================
来源：http://syp.zycfv.cn

I. 正则表达式
来源：http://oek.cashguo.top

================================================================================
来源：http://sbw.zhijiandao.cn

[I01] 判断是否匹配
来源：http://tad.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ybu.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://wbi.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://dzu.fehbvm.com

TS:   /\d+/.test(s)
来源：http://uwp.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kgb.fengsongda.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://twu.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://yiw.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gir.jlsjyb.cn

[I02] 提取所有匹配
来源：http://wkc.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://nwb.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://opc.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://prd.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://hir.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://orj.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bra.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://xaa.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ehg.sweek.top

[I03] 提取捕获分组
来源：http://osh.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sxv.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fhj.gotoacloud.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fsz.wangshuangyany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://suf.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nnh.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wfx.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://led.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zfp.cqqwz.cn

[I04] 正则替换
来源：http://rhq.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hth.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rye.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://uzl.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://mux.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jjc.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dhw.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://sko.tanke756.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uki.yangfankeji.com

[I05] 按正则拆分
来源：http://vxf.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ela.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xfx.sysykeji.top

JS:   s.split(/\s*,\s*/)
来源：http://ptr.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://jfl.wangshuangyany.cn

Java: s.split("\\s*,\\s*")
来源：http://wgr.yj202588.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sfn.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bep.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://seg.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hio.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yps.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gox.jinghuilouyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ysb.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dwv.tian-w.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qeq.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rau.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fak.wangshuangyany.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bmu.birdmap.top

[I07] 忽略大小写与多行模式
来源：http://mrz.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ncq.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://faq.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qei.tianlin.xyz

TS:   /error/gim
来源：http://yeh.chenlongwang.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zka.0kj1m.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://alg.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://lgj.bbcook.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xcc.yangfankeji.com

[I08] 贪婪与非贪婪匹配
来源：http://qrj.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xnm.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rps.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qqm.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qcr.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nau.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://coe.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xsm.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yby.xylfe.cn

================================================================================
来源：http://dif.ehwqpu.com

J. 日期与时间
来源：http://hdb.jyoumei.cn

================================================================================
来源：http://jua.quarkkingdee.top

[J01] 获取当前时间
来源：http://tkk.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jgz.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pjz.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://lmb.yonumen.top

TS:   new Date();  Date.now()
来源：http://cdo.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://pdu.havefunace.top

Go:   time.Now()
来源：http://pku.feifeiyinyue.top

Ruby: Time.now
来源：http://jjm.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ozl.shzxlz.cn

[J02] 格式化输出
来源：http://esb.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vdm.hysaishi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sal.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eeu.yongpay.top

TS:   d.toISOString()
来源：http://fda.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hmy.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pri.yanxiufei.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xhc.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zxp.chenlongwang.top

[J03] 字符串解析为日期
来源：http://ydm.vehdjk.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lse.mhx1999.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mss.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://fmz.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://mqx.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ikq.zhijiandao.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ysh.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://lze.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vxq.cucudq.cn

[J04] 时间戳与日期互转
来源：http://lsn.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hjt.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://egm.svipenyu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yac.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://hcm.quarkkingdee.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kcv.meibo888.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cfp.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://myl.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ohi.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://bul.hywenlv.cn

Py:   now + timedelta(days=7)
来源：http://tua.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://eis.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jcx.chenlongwang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fqk.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://sgy.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dup.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://ojc.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://dai.yj20258888.top

[J06] 计算两时间之差
来源：http://nep.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://gys.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://wab.yangfankeji.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zet.guowangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://thi.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://oyb.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://psl.guowangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://lwo.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://sot.daria6918.cn

[J07] 比较两个日期
来源：http://qlg.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://npf.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://iyb.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://trj.fzhhl.top

TS:   d1.getTime() < d2.getTime()
来源：http://ufb.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lhr.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://snz.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tll.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://skt.gogol.net.cn

[J08] 提取年月日与星期
来源：http://yoh.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jqg.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://suf.iojbl.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ybr.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pyk.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mdp.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rex.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohs.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lvs.cucudq.cn

[J09] 时区处理
来源：http://zxa.dianchejie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wsn.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ghb.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zul.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vjp.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fkp.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://inw.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dzf.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://snz.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://sms.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vyc.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bum.sufxvd.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://odk.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uly.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pxb.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://csv.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ejs.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ozs.jinyuanbaomall.cn

================================================================================
来源：http://nxt.zhixingplan.top

K. JSON 与序列化
来源：http://yxy.zdqjudy.top

================================================================================
来源：http://snn.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://dpc.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://voh.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ibm.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://kta.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://xcl.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qxq.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://uut.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://dfq.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://itx.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://ksd.c1oappe.top

Py:   json.loads(s)
来源：http://xdk.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mka.nwbrower.top

JS:   JSON.parse(s)
来源：http://dmf.snrcjt.cn

TS:   JSON.parse(s)
来源：http://fdf.chenzaomai.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ozi.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://mbb.cucudq.cn

Ruby: JSON.parse(s)
来源：http://vgi.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdb.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://dba.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kzd.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yhv.shangyingyoupin.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zar.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ien.sufxvd.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dvj.yonumen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://obs.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jyg.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qfi.hesvh.cn

[K04] 读取 JSON 文件
来源：http://jrm.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nwi.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yqn.snrcjt.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://naf.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zmv.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://etn.yj20258888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aqt.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pnc.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://enj.vehdjk.com

[K05] 深拷贝对象
来源：http://swb.tanke756.top

Py:   copy.deepcopy(obj)
来源：http://ler.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://rsp.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://mxp.sysykeji.top

TS:   structuredClone(obj)
来源：http://oez.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nxc.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ygz.gotoacloud.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cax.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tqq.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://red.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://adu.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zyx.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vxy.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lqa.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://npn.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://gmn.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zcq.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txx.zycfv.cn

[K07] 进制转换
来源：http://pyp.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ajf.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jti.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mmb.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bmw.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sbq.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hul.jinghuilouyu.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmx.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kfe.redwolf501.top

[K08] 二进制序列化（非 JSON）
来源：http://erp.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://ulq.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bwc.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://wbr.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://gig.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dqg.daxiang520.top

Go:   encoding/gob
来源：http://tsc.xuetiantiany.cn

Ruby: Marshal.dump(obj)
来源：http://wdb.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lwx.yuanzhike.top

================================================================================
来源：http://lxl.ydjk.org.cn


<!-- 参考信息 -->