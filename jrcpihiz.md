代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rcm.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://gru.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mcm.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://skb.ybcxt.top

Py:   value = d.get("k") or default
来源：http://aor.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://vnb.hammf.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tso.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://juy.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nkb.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://zxa.hfpthk.cn

Ruby: d&.dig(:a, :b)
来源：http://mlr.tanke756.top

C#:   obj?.A?.B ?? default
来源：http://dib.fehbvm.com

[H07] 断言
来源：http://gkh.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://slt.guowangkeji.top

PHP:  assert($x > 0);
来源：http://dmz.yuxming.cn

JS:   console.assert(x > 0);
来源：http://aig.bjfxy.top

TS:   console.assert(x > 0);
来源：http://feh.sufxvd.cn

Java: assert x > 0 : "必须为正";
来源：http://kkv.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dnf.hesvh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dly.hnqzz.top

C#:   Debug.Assert(x > 0);
来源：http://ljr.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://ovz.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://wjz.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uqc.fengsongda.top

JS:   e.message;  e.stack
来源：http://xjd.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ffn.dianchejie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dow.c1oappe.top

Go:   err.Error()
来源：http://ufm.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://vvw.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://bkz.gogol.net.cn

[H09] 带错误码的异常
来源：http://vpy.tarul.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://luf.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vpw.fengsongda.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qmj.yj20258888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rrh.chenzaomai.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dsk.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tkx.chenzaomai.com

Ruby: raise MyError.new("fail", 500)
来源：http://lhr.sweek.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xpk.cashguo.top

[H10] 资源自动释放
来源：http://yqd.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqo.hywenlv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bvn.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://taw.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kkr.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ejz.yongpay.top

Go:   defer f.Close()
来源：http://yub.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qro.zhaomingkeji.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eih.yueranfly.top

================================================================================
来源：http://smd.wangshuangyany.cn

I. 正则表达式
来源：http://mht.jinyuanbaomall.cn

================================================================================
来源：http://gqq.meibo888.top

[I01] 判断是否匹配
来源：http://sqt.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvu.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kat.zdqjudy.top

JS:   /\d+/.test(s)
来源：http://oxe.jinghuilouyu.cn

TS:   /\d+/.test(s)
来源：http://fls.dashuyun.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aso.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lpz.nanxinkj.top

Ruby: s.match?(/\d+/)
来源：http://yev.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uut.yuxming.cn

[I02] 提取所有匹配
来源：http://xel.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://nbq.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kyb.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ivo.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://ris.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xkd.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dsj.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://jzd.bbcook.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://btn.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://lph.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xvz.9152youxi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ipu.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sva.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lbb.xinyue.icu

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rck.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vsc.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ped.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rzg.haohaochexian.top

[I04] 正则替换
来源：http://ikz.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://env.zhengqikj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pnh.9152youxi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tsq.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://dhn.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eay.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lcn.zhaomingkeji.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://vyl.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yma.cucudq.cn

[I05] 按正则拆分
来源：http://lbz.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://yrg.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nxr.nanxuanxn.top

JS:   s.split(/\s*,\s*/)
来源：http://egd.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://apv.ehwqpu.com

Java: s.split("\\s*,\\s*")
来源：http://fhg.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tyq.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://jqo.jianghu66.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tll.ctjpmb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aow.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lir.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vrd.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eah.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uvw.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hqx.chenzaomai.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzq.sufxvd.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uxn.yangfankeji.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nyg.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://pqm.quarkkingdee.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fgp.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kms.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cmn.daria6918.cn

TS:   /error/gim
来源：http://znd.hammf.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tlc.guowangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dip.chenlongwang.top

Ruby: s.scan(/error/i)
来源：http://ufk.hesvh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fpu.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://khk.tianlin.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qrg.jlsjyb.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://znc.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rca.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qmt.andypj.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://sab.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qhm.ywan-chungtsiang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://abj.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qyr.yj202588.top

================================================================================
来源：http://wob.yuxming.cn

J. 日期与时间
来源：http://xva.zhixingplan.top

================================================================================
来源：http://leb.sweek.top

[J01] 获取当前时间
来源：http://uzp.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://czg.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kdv.gzhubu.top

JS:   new Date();  Date.now()
来源：http://jec.316326.xyz

TS:   new Date();  Date.now()
来源：http://kdk.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ovr.ppjwa.cn

Go:   time.Now()
来源：http://qyb.gotoacloud.top

Ruby: Time.now
来源：http://evc.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ptz.guannengcc.top

[J02] 格式化输出
来源：http://wsy.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hrb.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vhb.pycfn.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mvb.yueranfly.top

TS:   d.toISOString()
来源：http://dou.ppjwa.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ogw.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gkp.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fpd.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fco.havefunace.top

[J03] 字符串解析为日期
来源：http://jzv.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jze.feifeiyinyue.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://poj.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://wdp.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://xtu.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://yki.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cdh.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://thu.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://doo.bbcook.cn

[J04] 时间戳与日期互转
来源：http://pcp.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nfp.yj20258888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mas.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dki.xylfe.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cew.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://npy.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jrb.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vjq.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ozk.yfazqb.com

[J05] 时间加减（加 7 天）
来源：http://bge.tian-w.cn

Py:   now + timedelta(days=7)
来源：http://rbu.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wnk.yangfankeji.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpq.316326.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fkv.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://xds.zhixingplan.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ywh.fzhhl.top

Ruby: Time.now + 7 * 86400
来源：http://ubb.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://hlc.iojbl.cn

[J06] 计算两时间之差
来源：http://ped.uphjek.com

Py:   (end - start).total_seconds()
来源：http://mut.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://ejv.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://llh.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eil.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uyg.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://auu.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://dtk.sjlbkw.cn

C#:   (end - start).TotalSeconds
来源：http://bno.yuanzhike.top

[J07] 比较两个日期
来源：http://wfz.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://leo.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://khd.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ptj.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://wqb.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lxm.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://alt.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://ndz.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://vhn.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://epa.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lfd.hammf.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jnr.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ruc.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jeu.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kfp.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qim.mhx1999.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://duo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gaf.fengsongda.top

[J09] 时区处理
来源：http://mek.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qmi.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hnr.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jkt.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://maq.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oeb.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aeq.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://efh.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://flq.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://pnm.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zux.daxiang520.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://odz.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uzj.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gpv.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lzw.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kjl.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gdh.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tjl.jinqigfzy.top

================================================================================
来源：http://yci.hfpthk.cn

K. JSON 与序列化
来源：http://egm.xinyue.icu

================================================================================
来源：http://mxp.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://vih.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rdg.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vph.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://aer.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://tft.hesvh.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ong.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://xay.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://zll.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jxj.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://rbt.daxiang520.top

Py:   json.loads(s)
来源：http://izc.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wfb.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://lcq.c1oappe.top

TS:   JSON.parse(s)
来源：http://jbx.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lox.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://boq.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://ebc.yj20258.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gja.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://fki.tanke756.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pbm.hnqzz.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wki.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uaf.hcnkem.com

TS:   JSON.stringify(obj, null, 2)
来源：http://iay.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://prf.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lda.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://sjr.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dvj.fktsv.cn

[K04] 读取 JSON 文件
来源：http://dxw.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ksb.zhixingplan.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qrc.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ero.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yfc.shanyushiyangtech.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xka.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ojx.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wbd.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://con.ehwqpu.com

[K05] 深拷贝对象
来源：http://bqb.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://jck.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://mck.svipenyu.cn

JS:   structuredClone(obj)
来源：http://fsd.chenlongwang.top

TS:   structuredClone(obj)
来源：http://tyy.shanyushiyangtech.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rqt.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uhs.cucudq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ssy.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ioh.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://fmj.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eot.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fep.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://azc.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgk.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://avn.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zwc.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zuw.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jbz.daria6918.cn

[K07] 进制转换
来源：http://kes.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://app.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rpg.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qjd.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://iur.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iya.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dsd.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bsl.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lyf.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://eta.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://png.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cbv.vehdjk.com

JS:   v8.serialize(obj)        // Node
来源：http://wqj.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://uwg.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ywo.cucudq.cn

Go:   encoding/gob
来源：http://glu.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://izw.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://urx.uphjek.com

================================================================================
来源：http://ceb.yangfankeji.com

L. 网络请求
来源：http://dfp.ydzc1.top

================================================================================
来源：http://izx.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://yav.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ers.ywan-chungtsiang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lpd.ctjpmb.com

JS:   await fetch(url)
来源：http://qyh.epnwcf.com

TS:   await fetch(url)
来源：http://esg.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mow.fengsongda.top


<!-- 参考信息 -->