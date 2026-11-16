代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://scu.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://fau.jinqigufen.top

[H05] 捕获特定类型
来源：http://thb.zdbjq.cn

Py:   except ValueError as e:
来源：http://uwt.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wti.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://ghn.sjlbkw.cn

TS:   if (e instanceof TypeError) {}
来源：http://sub.cqqwz.cn

Java: catch (IOException | SQLException e) {}
来源：http://ayk.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vig.fanxiaobao.xyz

Ruby: rescue ArgumentError => e
来源：http://uoi.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qkr.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://bey.jinyuanbaomall.cn

Py:   value = d.get("k") or default
来源：http://bfw.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://qnz.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://suj.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mdt.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://shp.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ham.jyoumei.cn

Ruby: d&.dig(:a, :b)
来源：http://bis.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://syb.zhongyouzk.top

[H07] 断言
来源：http://zoq.iojbl.cn

Py:   assert x > 0, "必须为正"
来源：http://xkz.vqdsnc.cn

PHP:  assert($x > 0);
来源：http://klo.sjlbkw.cn

JS:   console.assert(x > 0);
来源：http://nsp.pengpengdd.cyou

TS:   console.assert(x > 0);
来源：http://wrv.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://qfv.hammf.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mlo.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://gvl.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://wqw.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://rsq.xingfuxueyuan.xyz

Py:   str(e);  traceback.format_exc()
来源：http://mae.snrcjt.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bxc.fzhhl.top

JS:   e.message;  e.stack
来源：http://mxq.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bku.hfpthk.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fyl.guannengcc.top

Go:   err.Error()
来源：http://cie.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://iny.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://ipx.cdnleiting.top

[H09] 带错误码的异常
来源：http://qqy.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zkz.xuanzx.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://txe.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://umm.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lfr.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kkw.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jnw.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://sqj.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jwv.jyoumei.cn

[H10] 资源自动释放
来源：http://lad.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ytl.cheryme.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://enu.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gru.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sug.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ymx.shanyushiyangkeji.top

Go:   defer f.Close()
来源：http://jlk.gaohongyu789.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://emp.vehdjk.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://acg.hnxiangtu.top

================================================================================
来源：http://qpu.jqgfzy.top

I. 正则表达式
来源：http://kcy.hammf.cn

================================================================================
来源：http://wbi.jlsjyb.cn

[I01] 判断是否匹配
来源：http://tip.shangyingyoupin.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://drj.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jcf.gzhubu.top

JS:   /\d+/.test(s)
来源：http://swj.yj202588.top

TS:   /\d+/.test(s)
来源：http://pmj.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uhu.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rsu.xuetiantiany.cn

Ruby: s.match?(/\d+/)
来源：http://pxq.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mfr.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://cyx.zhiwuduotai.top

Py:   re.findall(r"\d+", s)
来源：http://nxl.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bwj.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgg.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://ode.jinqigfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hoy.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xbj.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://dza.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wtr.xuanzx.com

[I03] 提取捕获分组
来源：http://evo.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cfc.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nsc.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mto.yongpay.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yvq.hesvh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fmi.yj202588.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hch.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yvc.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhm.zhoulong.xyz

[I04] 正则替换
来源：http://thd.zhaomingkeji.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://ams.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://htv.hcnkem.com

JS:   s.replace(/\d+/g, "#")
来源：http://wli.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xeg.yonumen.top

Java: s.replaceAll("\\d+", "#")
来源：http://ngt.fktsv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yzr.shzxlz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://agh.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aoi.hammf.cn

[I05] 按正则拆分
来源：http://bpc.wangshuangyany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qdx.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ofx.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://oio.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://ahh.fzhhl.top

Java: s.split("\\s*,\\s*")
来源：http://hdo.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aze.ctjpmb.com

Ruby: s.split(/\s*,\s*/)
来源：http://jqa.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://znr.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yqa.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://naz.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jny.aizwys.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jvg.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lqv.jlsjyb.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dfc.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://izy.52xcode.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jns.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bza.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://pyw.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wkh.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wby.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tqv.zhoulong.xyz

TS:   /error/gim
来源：http://njj.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lre.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://iui.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://jic.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lct.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://bij.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dlt.sjlbkw.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pma.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oev.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cum.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mcj.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://trc.316326.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zzo.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zhj.sysykeji.top

================================================================================
来源：http://aom.gzhubu.top

J. 日期与时间
来源：http://wql.hesvh.cn

================================================================================
来源：http://waw.aizwys.cn

[J01] 获取当前时间
来源：http://gfw.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ozj.vehdjk.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://edz.ydzc1.top

JS:   new Date();  Date.now()
来源：http://iph.kuanghao11.cn

TS:   new Date();  Date.now()
来源：http://efp.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mep.tianlin.xyz

Go:   time.Now()
来源：http://dtv.yongpay.top

Ruby: Time.now
来源：http://edv.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oxy.yfazqb.com

[J02] 格式化输出
来源：http://ici.pengpengdd.cyou

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jmg.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rob.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xgb.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://oam.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fin.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://euv.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xic.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://szv.yueranfly.top

[J03] 字符串解析为日期
来源：http://hwo.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yvd.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://arg.hywenlv.cn

JS:   new Date("2024-01-02")
来源：http://wfg.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://qzm.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://thg.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wds.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://uth.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gtz.yfazqb.com

[J04] 时间戳与日期互转
来源：http://zmc.feifeiyinyue.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kib.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fva.uphjek.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wyi.yongpay.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xlk.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ruh.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bxp.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xyz.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mzn.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://jkh.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://fpq.gotoacloud.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kel.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpb.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://csq.ywan-chungtsiang.top

Java: LocalDate.now().plusDays(7)
来源：http://jsi.zhongyouzk.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://itt.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://nnc.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://faj.shanyushiyangkeji.top

[J06] 计算两时间之差
来源：http://kug.haohaochexian.top

Py:   (end - start).total_seconds()
来源：http://xcp.yangfankeji.com

PHP:  $end->diff($start)->days;
来源：http://obb.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jxt.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pgu.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bhp.xuanzx.com

Go:   end.Sub(start).Hours()
来源：http://lrc.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://gyf.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://mra.shzxlz.cn

[J07] 比较两个日期
来源：http://reb.jinqigufen.top

Py:   d1 < d2;  d1 == d2
来源：http://uej.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rek.epnwcf.com

JS:   d1.getTime() < d2.getTime()
来源：http://hdj.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://mqs.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mue.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hkw.guannengcc.top

Ruby: d1 < d2;  d1 == d2
来源：http://alp.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://usy.svipenyu.cn

[J08] 提取年月日与星期
来源：http://tdf.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rkl.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ofu.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qxb.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ozv.xuetiantiany.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hud.andypj.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bev.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mut.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lnf.snrcjt.cn

[J09] 时区处理
来源：http://aih.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lqm.shzxlz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dgz.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://paq.redwolf501.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fev.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rjr.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wyt.gogol.net.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wpv.fehbvm.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zgg.chenlongwang.top

[J10] 取今天 / 本月第一天
来源：http://rkp.nanxinkj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wgz.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uff.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pzo.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ojy.hesvh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hdy.hnxiangtu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nvq.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wtd.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rhk.sxryk.cn

================================================================================
来源：http://ooh.ydzc1.top

K. JSON 与序列化
来源：http://rno.gotoacloud.top

================================================================================
来源：http://fuu.bbcook.cn

[K01] 对象转 JSON 字符串
来源：http://mks.52xcode.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ncn.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ytr.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://ylx.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://aux.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wtv.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://ire.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://roj.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://srr.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://qqx.yfazqb.com

Py:   json.loads(s)
来源：http://wuw.smart0.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ycb.andypj.xyz

JS:   JSON.parse(s)
来源：http://hzm.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://tgt.fktsv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://npr.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://bnt.xuanzx.com

Ruby: JSON.parse(s)
来源：http://ttp.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bnd.tianlin.xyz

[K03] JSON 美化输出（带缩进）
来源：http://afa.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gtt.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rmk.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ppy.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://blj.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tzx.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xiy.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://mew.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rew.sxryk.cn

[K04] 读取 JSON 文件
来源：http://ljx.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffo.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://etn.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kno.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cen.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ule.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wnn.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://cys.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zds.tanke756.top

[K05] 深拷贝对象
来源：http://xhp.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://cjz.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://ocg.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://pqq.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://csy.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://prw.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ksn.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxw.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://pem.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://kzp.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://slt.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwn.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sik.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uug.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sah.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://sku.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fvu.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://smb.zycfv.cn

[K07] 进制转换
来源：http://kxu.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://eob.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lcv.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ecx.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bxb.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ygr.ctjpmb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mzx.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qks.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zbm.jiagoushi.top

[K08] 二进制序列化（非 JSON）
来源：http://koc.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://trt.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://xiu.jinqigfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://ddj.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://ngv.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxc.haohaochexian.top

Go:   encoding/gob
来源：http://yyd.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://azj.guowangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ofj.yj20258888.top

================================================================================
来源：http://gia.sufxvd.cn


<!-- 参考信息 -->