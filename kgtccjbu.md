代发 wailian999

TS:   console.assert(x > 0);
来源：http://xzp.ehwqpu.com

Java: assert x > 0 : "必须为正";
来源：http://jys.cashguo.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lot.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qkl.snrcjt.cn

C#:   Debug.Assert(x > 0);
来源：http://zqy.hfpthk.cn

[H08] 获取错误信息与堆栈
来源：http://zgh.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://wob.chenlongwang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ikz.zdqjudy.top

JS:   e.message;  e.stack
来源：http://wbf.hammf.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ium.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xxy.tarul.cn

Go:   err.Error()
来源：http://fvs.jqgfzy.top

Ruby: e.message;  e.backtrace
来源：http://hcu.xuanzx.com

C#:   e.Message;  e.StackTrace
来源：http://pta.52xcode.cn

[H09] 带错误码的异常
来源：http://bzc.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hux.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nxj.yueranfly.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://npd.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://voy.birdmap.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qpa.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://msr.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://kvn.jinghuilouyu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xhu.vqdsnc.cn

[H10] 资源自动释放
来源：http://zui.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mpn.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vvs.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bsj.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xpe.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xcl.havefunace.top

Go:   defer f.Close()
来源：http://rbp.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bkt.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eoi.shangyingyoupin.top

================================================================================
来源：http://deb.tanke756.top

I. 正则表达式
来源：http://xzv.zhiwuduotai.top

================================================================================
来源：http://eqs.nanxinkj.top

[I01] 判断是否匹配
来源：http://hms.redwolf501.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nrb.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kbi.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://rdn.9152youxi.cn

TS:   /\d+/.test(s)
来源：http://ynj.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tgj.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yrm.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://tgs.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gmt.ydzc1.top

[I02] 提取所有匹配
来源：http://iwn.zhixingplan.top

Py:   re.findall(r"\d+", s)
来源：http://jmg.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ajq.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hak.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://zxu.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lon.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oij.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://ayu.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yoj.hywenlv.cn

[I03] 提取捕获分组
来源：http://exx.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eoi.shuidangran.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://imc.hysaishi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hrl.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ujr.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://crj.yuxming.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ebv.52xcode.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yin.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dge.chenlongwang.top

[I04] 正则替换
来源：http://nqj.feifeiyinyue.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kwc.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bqd.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://jag.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://xom.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://hif.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://frm.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://rsn.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://duk.jinyuanbaomall.cn

[I05] 按正则拆分
来源：http://xhz.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wuj.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://phg.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://hpj.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://lak.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://hlj.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bdu.wangshuangyany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://axr.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://awj.zhaomingkeji.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gid.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://usw.haohaochexian.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ssl.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gyz.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dfn.iojbl.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://upe.zhoulong.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsp.jinghuilouyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixv.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tuj.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://fol.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://phn.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vqp.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ltx.hcnkem.com

TS:   /error/gim
来源：http://oat.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pgr.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rvx.yj202588.top

Ruby: s.scan(/error/i)
来源：http://hcf.sxryk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pvr.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://saj.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zmi.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://urt.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qyw.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://khp.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ueg.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yok.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://loc.sweek.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dmb.yonumen.top

================================================================================
来源：http://fqn.ywan-chungtsiang.top

J. 日期与时间
来源：http://trg.xuetiantiany.cn

================================================================================
来源：http://wwz.chenlongwang.top

[J01] 获取当前时间
来源：http://rqj.aibaodan.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qem.iojbl.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pxn.tian-w.cn

JS:   new Date();  Date.now()
来源：http://eux.tian-w.cn

TS:   new Date();  Date.now()
来源：http://lww.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hle.feifeiyinyue.top

Go:   time.Now()
来源：http://ozi.zhoulong.xyz

Ruby: Time.now
来源：http://opm.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://agy.xuetiantiany.cn

[J02] 格式化输出
来源：http://wvi.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwj.yangfankeji.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sxr.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aix.fzhhl.top

TS:   d.toISOString()
来源：http://arz.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hrd.xziqi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lsd.xylfe.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qki.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xcf.ydzc1.top

[J03] 字符串解析为日期
来源：http://gzf.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fgl.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aub.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://qrp.ydjk.org.cn

TS:   new Date("2024-01-02")
来源：http://xbe.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://fzn.nwbrower.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ncx.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://oen.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ylv.bbcook.cn

[J04] 时间戳与日期互转
来源：http://cis.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rvm.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://guu.tian-w.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yli.meibo888.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xlx.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://puy.hcnkem.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gbg.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cwb.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pas.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://gvx.jlsjyb.cn

Py:   now + timedelta(days=7)
来源：http://ldl.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wjq.cdnleiting.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aat.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gpp.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://bje.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wvk.tian-w.cn

Ruby: Time.now + 7 * 86400
来源：http://oyf.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vuz.yvedp.cn

[J06] 计算两时间之差
来源：http://oot.mhx1999.top

Py:   (end - start).total_seconds()
来源：http://lur.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://jnm.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bmu.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blk.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yli.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://qfm.jqgfzy.top

Ruby: end - start                 # 返回秒数
来源：http://jer.zdqjudy.top

C#:   (end - start).TotalSeconds
来源：http://klr.9152youxi.cn

[J07] 比较两个日期
来源：http://hiz.jqgfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://flz.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ncy.ctjpmb.com

JS:   d1.getTime() < d2.getTime()
来源：http://yhi.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://ofi.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rzx.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cad.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://pqv.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://axu.9152youxi.cn

[J08] 提取年月日与星期
来源：http://lwt.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kdj.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fbp.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vyc.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aed.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://whh.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yym.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rvs.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://djc.hywenlv.cn

[J09] 时区处理
来源：http://tjp.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vmn.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ukb.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vtp.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oas.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gpf.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rqa.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://udz.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pjt.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://hpf.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gjz.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jvn.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bcm.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oyy.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mmk.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jtp.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zmo.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tju.andypj.xyz

================================================================================
来源：http://llv.daxiang520.top

K. JSON 与序列化
来源：http://cza.ctjpmb.com

================================================================================
来源：http://zfz.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://lwo.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fkm.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zku.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://nzc.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://yyf.svipenyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lit.hnqzz.top

Go:   json.Marshal(obj)
来源：http://myz.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://nin.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://imi.mhx1999.top

[K02] JSON 字符串转对象
来源：http://bcz.fengsongda.top

Py:   json.loads(s)
来源：http://ekn.9152youxi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tlc.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://iij.aizwys.cn

TS:   JSON.parse(s)
来源：http://ipp.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kfz.dianchejie.cn

Go:   json.Unmarshal(data, &v)
来源：http://vfd.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://nsm.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oyv.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://lxq.yongpay.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fpz.haohaochexian.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pzb.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nsv.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://hri.ydjk.org.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jpw.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://woh.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://iim.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xos.daria6918.cn

[K04] 读取 JSON 文件
来源：http://rrq.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://czj.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zcu.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aoz.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://seo.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jdl.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ram.hywenlv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhm.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pyw.jlsjyb.cn

[K05] 深拷贝对象
来源：http://dsp.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://vdf.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://rzy.tianlin.xyz

JS:   structuredClone(obj)
来源：http://oqf.wangdashe.top

TS:   structuredClone(obj)
来源：http://tbh.zhiwuduotai.top

Java: // 手写拷贝构造，或序列化往返
来源：http://sgx.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bqu.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://woz.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pfb.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://upl.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ovf.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qjl.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vcb.tian-w.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://llm.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cug.shangyingyoupin.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://czd.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jxr.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rul.hysaishi.cn

[K07] 进制转换
来源：http://pld.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gha.pengpengdd.cyou

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rrs.ehwqpu.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://oye.chenlongwang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ecs.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gwz.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pni.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gvb.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://lbt.aibaodan.cn

Py:   pickle.dumps(obj)
来源：http://eux.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bgl.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://jvd.jinyuanbaomall.cn

TS:   v8.serialize(obj)        // Node
来源：http://xcu.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rjb.dianchejie.cn

Go:   encoding/gob
来源：http://jko.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://diz.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gbx.dashuyun.cn

================================================================================
来源：http://gpc.ydjk.org.cn

L. 网络请求
来源：http://xcq.tianlin.xyz

================================================================================
来源：http://qct.havefunace.top

[L01] 发送 GET 请求
来源：http://tfj.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://icc.snrcjt.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://eqm.ybcxt.top

JS:   await fetch(url)
来源：http://ctj.sufxvd.cn

TS:   await fetch(url)
来源：http://fan.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xqp.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://jkc.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qsh.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cfk.ctjpmb.com

[L02] 发送 POST JSON
来源：http://zrx.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://qdq.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ryz.zycfv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hib.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbh.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhy.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pup.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vnv.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xrx.yvedp.cn

[L03] 设置自定义请求头
来源：http://gsk.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tkz.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://swv.cheryme.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jkc.hysaishi.cn


<!-- 参考信息 -->