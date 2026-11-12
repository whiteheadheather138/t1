代发 wailian999

Py:   value = d.get("k") or default
来源：http://vnk.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://coa.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://cvw.sufxvd.cn

TS:   obj?.a?.b;  d ?? default
来源：http://akf.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bwc.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ndt.nanxinkj.top

Ruby: d&.dig(:a, :b)
来源：http://ola.svipenyu.cn

C#:   obj?.A?.B ?? default
来源：http://ofm.hongshengwenyu.top

[H07] 断言
来源：http://kqj.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://tmq.chenlongwang.top

PHP:  assert($x > 0);
来源：http://xik.0kj1m.cn

JS:   console.assert(x > 0);
来源：http://sgq.yuanzhike.top

TS:   console.assert(x > 0);
来源：http://yzs.c1oappe.top

Java: assert x > 0 : "必须为正";
来源：http://ggq.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jhg.c1oappe.top

Ruby: raise "必须为正" unless x > 0
来源：http://wdn.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://hib.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://bal.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://jsa.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zzd.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://cde.xuetiantiany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://arc.chenlongwang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gyb.daxiang520.top

Go:   err.Error()
来源：http://uuu.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://uyb.ywan-chungtsiang.top

C#:   e.Message;  e.StackTrace
来源：http://wzt.yongpay.top

[H09] 带错误码的异常
来源：http://dbn.nwbrower.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gol.fktsv.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vvg.wangdashe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lxz.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cla.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://onu.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ars.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://ckg.ydzc1.top

C#:   // 自定义异常类中加 Code 属性
来源：http://efa.c1oappe.top

[H10] 资源自动释放
来源：http://but.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aue.ivvv.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zgv.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tzc.52xcode.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eeb.shanyushiyangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cop.fktsv.cn

Go:   defer f.Close()
来源：http://wqb.jinghuilouyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://egi.hesvh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ziz.cqqwz.cn

================================================================================
来源：http://wku.jiagoushi.top

I. 正则表达式
来源：http://aot.xingfuxueyuan.xyz

================================================================================
来源：http://jbt.yueranfly.top

[I01] 判断是否匹配
来源：http://snf.epnwcf.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nra.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://vld.sysykeji.top

JS:   /\d+/.test(s)
来源：http://apc.ctjpmb.com

TS:   /\d+/.test(s)
来源：http://pdx.tanke756.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qxu.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xzm.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://kzz.vqdsnc.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cyp.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://egp.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://geb.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://abk.jinqigfzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yls.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://vhb.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nhj.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fmp.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://wgk.yfazqb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fjl.epnwcf.com

[I03] 提取捕获分组
来源：http://upz.cucudq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rfs.yanxiufei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://amf.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gab.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://osh.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yxc.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kvq.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://izr.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jfr.ywan-chungtsiang.top

[I04] 正则替换
来源：http://oip.shuidangran.top

Py:   re.sub(r"\d+", "#", s)
来源：http://onj.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pww.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://ptn.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://zrw.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://nvm.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://tha.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dxq.fktsv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bro.ivvv.top

[I05] 按正则拆分
来源：http://acb.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://pnq.hesvh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hgj.ivvv.top

JS:   s.split(/\s*,\s*/)
来源：http://orj.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://fyv.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://enx.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jvr.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qrq.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nkj.ydjk.org.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://csr.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dux.jinghuilouyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://udl.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hmb.shanyushiyangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqr.shuidangran.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vwu.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qqr.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dcc.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pyh.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://ass.ctjpmb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jlo.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cmt.zhijiandao.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uhc.jinghuilouyu.cn

TS:   /error/gim
来源：http://afa.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fxv.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fqz.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://wom.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yhl.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ntb.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pog.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kar.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://faa.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ras.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uos.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fgf.pengpengdd.cyou

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://roa.tian-w.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ihc.hywenlv.cn

================================================================================
来源：http://vfz.yuxming.cn

J. 日期与时间
来源：http://uzj.ydzc1.top

================================================================================
来源：http://waj.wangdashe.top

[J01] 获取当前时间
来源：http://mza.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cxh.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mow.jlsjyb.cn

JS:   new Date();  Date.now()
来源：http://rwd.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://hgc.kuanghao11.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gso.ctjpmb.com

Go:   time.Now()
来源：http://tyh.pycfn.com

Ruby: Time.now
来源：http://bnl.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fgn.shangyingyoupin.top

[J02] 格式化输出
来源：http://nrb.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fzo.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulx.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ssh.vqdsnc.cn

TS:   d.toISOString()
来源：http://mlc.jinqigufen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ubg.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rrg.smart0.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oab.zhoulong.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yfa.jianghu66.top

[J03] 字符串解析为日期
来源：http://dhk.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wlv.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vkz.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://nnq.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://cro.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lmt.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ytr.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://xbx.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fem.mhx1999.top

[J04] 时间戳与日期互转
来源：http://moa.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://npb.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yin.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iah.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pby.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lbg.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zqj.jinqigufen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://weo.jianghu66.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fta.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://dja.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://awy.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ukh.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ldg.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zgi.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://fhf.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iie.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://ede.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://ixw.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://pjn.xziqi.cn

Py:   (end - start).total_seconds()
来源：http://due.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://mcq.zhiwuduotai.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wir.zdbjq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aiz.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://loj.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://lxx.zhoulong.xyz

Ruby: end - start                 # 返回秒数
来源：http://mtp.316326.xyz

C#:   (end - start).TotalSeconds
来源：http://prb.shangyingyoupin.top

[J07] 比较两个日期
来源：http://rsv.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://tgl.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xjr.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://rpm.mhx1999.top

TS:   d1.getTime() < d2.getTime()
来源：http://tjl.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://swu.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lif.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://hqc.epnwcf.com

C#:   d1 < d2;  d1 == d2
来源：http://drj.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://obl.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ift.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jdl.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://srs.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://avc.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://llq.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pzd.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://krx.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tig.nwbrower.top

[J09] 时区处理
来源：http://odv.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pky.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ner.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ycj.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jhu.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbr.havefunace.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hmb.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fjb.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kfo.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://nmf.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bdg.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lii.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bha.daxiang520.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ycm.pengpengdd.cyou

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rrd.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://isx.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpv.52xcode.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://shi.wangdashe.top

================================================================================
来源：http://rwz.gogol.net.cn

K. JSON 与序列化
来源：http://yvy.epnwcf.com

================================================================================
来源：http://hnp.sjlbkw.cn

[K01] 对象转 JSON 字符串
来源：http://pzx.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mpc.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ozz.0kj1m.cn

JS:   JSON.stringify(obj)
来源：http://bnn.xziqi.cn

TS:   JSON.stringify(obj)
来源：http://rfn.shzxlz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://npd.xuanzx.com

Go:   json.Marshal(obj)
来源：http://ona.daxiang520.top

Ruby: obj.to_json                                     // require "json"
来源：http://ere.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vfb.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://ngk.gotoacloud.top

Py:   json.loads(s)
来源：http://mbp.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rsf.yueranfly.top

JS:   JSON.parse(s)
来源：http://xxf.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://ywj.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oux.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://izf.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://ecg.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://krd.xuetiantiany.cn

[K03] JSON 美化输出（带缩进）
来源：http://vhj.zhijiandao.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://grn.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://evr.aizwys.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bjc.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dxd.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xul.fanxiaobao.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zko.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://qee.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pai.ybcxt.top

[K04] 读取 JSON 文件
来源：http://cdu.xuetiantiany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bmt.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oxr.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zhj.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://orl.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aub.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hou.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rtk.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zqq.birdmap.top

[K05] 深拷贝对象
来源：http://owx.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://two.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://qhg.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://ldo.yfazqb.com

TS:   structuredClone(obj)
来源：http://rrh.pycfn.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mbv.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ffb.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://epu.cheryme.top

C#:   // 序列化往返，或自定义 Clone
来源：http://njr.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://agg.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qhx.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dfw.havefunace.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jup.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uwe.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://phz.ctjpmb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://jre.ehwqpu.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xvd.tianlin.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rku.pengpengdd.cyou

[K07] 进制转换
来源：http://iqr.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xxe.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tkv.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://auq.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://udz.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yhx.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kqe.xylfe.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ebv.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cfr.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://aek.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://sij.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wyk.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://igk.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://mhb.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ihw.cucudq.cn

Go:   encoding/gob
来源：http://rwo.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://hso.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bou.gaohongyu789.top

================================================================================
来源：http://zyv.jqgufenzy.top

L. 网络请求
来源：http://ool.jyoumei.cn

================================================================================
来源：http://caw.haohaochexian.top

[L01] 发送 GET 请求
来源：http://yfw.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ard.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wgb.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://jtn.ydjk.org.cn

TS:   await fetch(url)
来源：http://mzf.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fvs.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://ovt.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wik.cheryme.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://drm.haohaochexian.top

[L02] 发送 POST JSON
来源：http://bgv.jqgfzy.top


<!-- 参考信息 -->