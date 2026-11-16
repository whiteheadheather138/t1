代发 wailian999

Py:   value = d.get("k") or default
来源：http://cpm.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://nld.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://zdo.aizwys.cn

TS:   obj?.a?.b;  d ?? default
来源：http://frr.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zmw.uphjek.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qes.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://bfg.ydzc1.top

C#:   obj?.A?.B ?? default
来源：http://reh.yj20258.top

[H07] 断言
来源：http://byu.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://ckn.sxryk.cn

PHP:  assert($x > 0);
来源：http://zsm.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://atq.hammf.cn

TS:   console.assert(x > 0);
来源：http://scp.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://kcc.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vdw.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://axe.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://tfc.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://yin.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://xau.tanke756.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qpw.fengsongda.top

JS:   e.message;  e.stack
来源：http://kus.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://rzw.jqgfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qxq.cashguo.top

Go:   err.Error()
来源：http://xxc.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://gnr.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://rbl.fktsv.cn

[H09] 带错误码的异常
来源：http://uyj.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gda.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://mgx.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzh.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cxq.hysaishi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocl.jinghuilouyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zpr.gotoacloud.top

Ruby: raise MyError.new("fail", 500)
来源：http://whe.daxiang520.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gyv.zhaomingkeji.xyz

[H10] 资源自动释放
来源：http://zzh.zhijiandao.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pii.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rdl.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nhi.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bda.quarkkingdee.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wmn.9152youxi.cn

Go:   defer f.Close()
来源：http://bla.pengpengdd.cyou

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mat.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cbj.zhongyouzk.top

================================================================================
来源：http://kyi.0kj1m.cn

I. 正则表达式
来源：http://yxu.jqgfzy.top

================================================================================
来源：http://iwe.fehbvm.com

[I01] 判断是否匹配
来源：http://ijm.jlsjyb.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://noo.0kj1m.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oul.fzhhl.top

JS:   /\d+/.test(s)
来源：http://hsi.xuanzx.com

TS:   /\d+/.test(s)
来源：http://tmw.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mev.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bhc.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://afi.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://igt.daria6918.cn

[I02] 提取所有匹配
来源：http://zpl.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://adi.iojbl.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uqm.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ntz.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://fks.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://udj.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfu.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://pll.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cbp.daria6918.cn

[I03] 提取捕获分组
来源：http://uny.tarul.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cyh.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lko.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ccl.sysykeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://klx.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://coh.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cqy.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wza.birdmap.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sfv.mhx1999.top

[I04] 正则替换
来源：http://gqs.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://niq.yj20258.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ytr.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://oai.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ywc.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://xsh.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gbc.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://vzv.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dnl.ywan-chungtsiang.top

[I05] 按正则拆分
来源：http://oho.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hqo.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ytm.shangyingyoupin.top

JS:   s.split(/\s*,\s*/)
来源：http://yti.shuidangran.top

TS:   s.split(/\s*,\s*/)
来源：http://niu.xuetiantiany.cn

Java: s.split("\\s*,\\s*")
来源：http://nnv.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://riz.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://eeq.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bsw.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xqs.bbcook.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kmc.fehbvm.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nur.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cso.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qxy.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wsp.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://myn.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tel.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pzc.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://buh.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jzy.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://byp.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gwk.mhx1999.top

TS:   /error/gim
来源：http://icv.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tra.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxg.nwbrower.top

Ruby: s.scan(/error/i)
来源：http://ioc.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vxg.tanke756.top

[I08] 贪婪与非贪婪匹配
来源：http://muj.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zwg.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cix.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://utv.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vcv.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rdl.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://raf.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rsr.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ifu.bbcook.cn

================================================================================
来源：http://wiv.sxryk.cn

J. 日期与时间
来源：http://zie.316326.xyz

================================================================================
来源：http://nqs.sweek.top

[J01] 获取当前时间
来源：http://lbp.fanxiaobao.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://opz.fktsv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://msn.fengsongda.top

JS:   new Date();  Date.now()
来源：http://ljk.jyoumei.cn

TS:   new Date();  Date.now()
来源：http://zeg.zhaomingkeji.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://oxs.vqdsnc.cn

Go:   time.Now()
来源：http://vej.nanxinkj.top

Ruby: Time.now
来源：http://cbr.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pyv.fzhhl.top

[J02] 格式化输出
来源：http://ujr.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yry.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nlh.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zop.316326.xyz

TS:   d.toISOString()
来源：http://qbm.zhengqikj.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lsj.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://njd.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qrm.zdqjudy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wnp.zhaomingkeji.xyz

[J03] 字符串解析为日期
来源：http://dzv.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cdj.shanyushiyangtech.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oqm.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://vtd.pycfn.com

TS:   new Date("2024-01-02")
来源：http://rxn.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://qge.daxiang520.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kll.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://ahy.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cvz.hcnkem.com

[J04] 时间戳与日期互转
来源：http://bef.cqqwz.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lgw.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://klo.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zeu.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lsj.havefunace.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zkb.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rlh.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dng.ivvv.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://suy.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://diz.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://zhy.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://srh.zhixingplan.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ibx.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ibr.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://rxx.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oll.hnqzz.top

Ruby: Time.now + 7 * 86400
来源：http://jre.xinyue.icu

C#:   DateTime.Now.AddDays(7)
来源：http://vyu.jlsjyb.cn

[J06] 计算两时间之差
来源：http://lvf.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://ngl.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://jwb.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zzx.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hyn.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://voj.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://mnv.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://wpt.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://saf.jianghu66.top

[J07] 比较两个日期
来源：http://abx.jyoumei.cn

Py:   d1 < d2;  d1 == d2
来源：http://wwu.hnxiangtu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://olv.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://zyg.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://zzz.uphjek.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxs.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lmt.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://hlf.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://duy.fktsv.cn

[J08] 提取年月日与星期
来源：http://qxe.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hzc.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ybs.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://npi.0kj1m.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gar.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hce.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eil.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zfp.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://icy.ctjpmb.com

[J09] 时区处理
来源：http://xcd.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xcj.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cjm.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dmo.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjn.hnxiangtu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eyx.fanxiaobao.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tqz.zhiwuduotai.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vmu.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xmt.xziqi.cn

[J10] 取今天 / 本月第一天
来源：http://stt.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pbu.hnxiangtu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xyl.tianlin.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hfi.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ugc.hfpthk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hhe.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ied.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://con.zdbjq.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kiq.tarul.cn

================================================================================
来源：http://xzj.vehdjk.com

K. JSON 与序列化
来源：http://lal.aizwys.cn

================================================================================
来源：http://xst.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://uha.zdqjudy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hvc.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qjc.cqqwz.cn

JS:   JSON.stringify(obj)
来源：http://upp.yj20258.top

TS:   JSON.stringify(obj)
来源：http://ycl.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bry.xingfuxueyuan.xyz

Go:   json.Marshal(obj)
来源：http://cgp.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://pgw.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tny.xziqi.cn

[K02] JSON 字符串转对象
来源：http://euo.nanxinkj.top

Py:   json.loads(s)
来源：http://fgi.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lpn.gotoacloud.top

JS:   JSON.parse(s)
来源：http://wci.zycfv.cn

TS:   JSON.parse(s)
来源：http://sdb.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yja.ctjpmb.com

Go:   json.Unmarshal(data, &v)
来源：http://vbu.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://cnh.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cmh.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://ruy.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ial.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://all.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dgb.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://arq.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fyd.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fbh.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vkz.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lsg.andypj.xyz

[K04] 读取 JSON 文件
来源：http://awk.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xhs.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hvh.shuidangran.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbp.smart0.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjl.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zsh.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://utn.jlsjyb.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nek.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wkm.zhoulong.xyz

[K05] 深拷贝对象
来源：http://nre.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://yne.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://ckx.sweek.top

JS:   structuredClone(obj)
来源：http://fut.cdnleiting.top

TS:   structuredClone(obj)
来源：http://hpf.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vuu.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wlr.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rms.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zdq.gzhubu.top

[K06] 解析 URL 查询串
来源：http://txx.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://smi.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hwr.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qxk.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwt.zdqjudy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://onr.9152youxi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://njn.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ekc.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jnr.yangfankeji.com

[K07] 进制转换
来源：http://fhx.hammf.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ijg.zhengqikj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jac.yj202588.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lni.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qtp.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://esw.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jqh.c1oappe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://agy.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ynz.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://xge.yj20258.top

Py:   pickle.dumps(obj)
来源：http://bhx.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lyf.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://lun.zhengqikj.top

TS:   v8.serialize(obj)        // Node
来源：http://dig.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jxh.chenlongwang.top

Go:   encoding/gob
来源：http://wgb.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://nsu.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mmj.xziqi.cn

================================================================================
来源：http://cku.tianlin.xyz

L. 网络请求
来源：http://mgl.hcnkem.com

================================================================================
来源：http://qld.redwolf501.top

[L01] 发送 GET 请求
来源：http://hky.jqgufenzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mqe.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://euj.haohaochexian.top

JS:   await fetch(url)
来源：http://vvq.smart0.xyz

TS:   await fetch(url)
来源：http://hwq.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bxy.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://wbh.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sbr.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wiy.redwolf501.top

[L02] 发送 POST JSON
来源：http://bao.bjfxy.top


<!-- 参考信息 -->