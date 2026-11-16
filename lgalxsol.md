代发 wailian999

TS:   console.assert(x > 0);
来源：http://swr.birdmap.top

Java: assert x > 0 : "必须为正";
来源：http://ixq.yuxming.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iqe.chenjidiqi.icu

Ruby: raise "必须为正" unless x > 0
来源：http://xpn.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://rnt.zhixingplan.top

[H08] 获取错误信息与堆栈
来源：http://jad.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://gdi.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hdy.yuxming.cn

JS:   e.message;  e.stack
来源：http://jxa.sweek.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ugo.bjfxy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ulq.bbcook.cn

Go:   err.Error()
来源：http://vgb.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://ypp.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://bdl.zycfv.cn

[H09] 带错误码的异常
来源：http://zcc.bjfxy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ktk.zhengqikj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qgh.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ucm.pengpengdd.cyou

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://irh.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://whu.hywenlv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rse.gzhubu.top

Ruby: raise MyError.new("fail", 500)
来源：http://yru.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xlz.hongshengwenyu.top

[H10] 资源自动释放
来源：http://dci.ctjpmb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://vwt.bbcook.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://muy.ehwqpu.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hff.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://avz.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qvl.yueranfly.top

Go:   defer f.Close()
来源：http://jqi.redwolf501.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xqx.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sur.jinyuanbaomall.cn

================================================================================
来源：http://naa.daxiang520.top

I. 正则表达式
来源：http://lrs.0kj1m.cn

================================================================================
来源：http://zgx.pengpengdd.cyou

[I01] 判断是否匹配
来源：http://xlo.xuanzx.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mmi.nwbrower.top

PHP:  preg_match('/\d+/', $s);
来源：http://hhm.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://qtq.52xcode.cn

TS:   /\d+/.test(s)
来源：http://nyz.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ibs.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mwq.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://qet.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zwi.nanxinkj.top

[I02] 提取所有匹配
来源：http://cdq.svipenyu.cn

Py:   re.findall(r"\d+", s)
来源：http://nsv.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wkq.zdbjq.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fxx.hcnkem.com

TS:   s.match(/\d+/g)
来源：http://hzr.yueranfly.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gng.wangdashe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xpf.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://grb.shangyingyoupin.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vua.pycfn.com

[I03] 提取捕获分组
来源：http://ykm.zhoulong.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qdn.jinghuilouyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tkb.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mww.zhongyouzk.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hkj.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ixq.kuanghao11.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xox.quarkkingdee.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bra.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kkt.jyoumei.cn

[I04] 正则替换
来源：http://icg.yangfankeji.com

Py:   re.sub(r"\d+", "#", s)
来源：http://dyo.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hnu.ctjpmb.com

JS:   s.replace(/\d+/g, "#")
来源：http://rmu.zhoulong.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://lix.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wts.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://krk.daxiang520.top

Ruby: s.gsub(/\d+/, "#")
来源：http://osk.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dmj.ydjk.org.cn

[I05] 按正则拆分
来源：http://abs.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bdt.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nfj.nanxinkj.top

JS:   s.split(/\s*,\s*/)
来源：http://gbk.chenzaomai.com

TS:   s.split(/\s*,\s*/)
来源：http://prx.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://gus.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cve.ydjk.org.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qcf.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bkk.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ysd.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lvx.birdmap.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://syf.redwolf501.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vxp.hnqzz.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oeh.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yyb.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ihm.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://brf.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nnz.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://igb.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wci.haohaochexian.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ocf.zhengqikj.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mqh.aizwys.cn

TS:   /error/gim
来源：http://rfm.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ysk.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xsd.hammf.cn

Ruby: s.scan(/error/i)
来源：http://lnm.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ntb.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://uah.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wya.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ffe.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kdm.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bst.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pdf.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://raa.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ntk.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://abj.zhaomingkeji.xyz

================================================================================
来源：http://xmr.yuxming.cn

J. 日期与时间
来源：http://hwo.yueranfly.top

================================================================================
来源：http://ijt.chenzaomai.com

[J01] 获取当前时间
来源：http://tgu.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jiu.haohaochexian.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sve.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://hlh.sxryk.cn

TS:   new Date();  Date.now()
来源：http://hua.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xhs.zhixingplan.top

Go:   time.Now()
来源：http://pja.gotoacloud.top

Ruby: Time.now
来源：http://osz.0kj1m.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bqp.zdqjudy.top

[J02] 格式化输出
来源：http://vtj.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qks.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vph.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ebk.tarul.cn

TS:   d.toISOString()
来源：http://mip.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xri.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ffe.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zsd.tarul.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qyp.cdnleiting.top

[J03] 字符串解析为日期
来源：http://ocb.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lks.zycfv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://njn.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://ias.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://gxz.ydjk.org.cn

Java: LocalDate.parse("2024-01-02")
来源：http://snl.yj20258888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ocf.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://rjf.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mjv.ehwqpu.com

[J04] 时间戳与日期互转
来源：http://amq.dashuyun.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mrj.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://isd.yonumen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mfy.52xcode.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fea.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nvq.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hxt.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://czy.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jcu.tarul.cn

[J05] 时间加减（加 7 天）
来源：http://qpn.yongpay.top

Py:   now + timedelta(days=7)
来源：http://gxa.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jcj.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpg.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bwt.zhixingplan.top

Java: LocalDate.now().plusDays(7)
来源：http://dvy.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bst.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://ekf.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://dbz.yongpay.top

[J06] 计算两时间之差
来源：http://eno.jianghu66.top

Py:   (end - start).total_seconds()
来源：http://kje.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://ccf.hammf.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bqp.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nom.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://eop.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://nky.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://wcn.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://aau.fehbvm.com

[J07] 比较两个日期
来源：http://akd.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://tbg.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ebp.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://gvj.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://osn.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uxk.fengsongda.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eil.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://djk.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://kgr.iojbl.cn

[J08] 提取年月日与星期
来源：http://atz.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zes.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://byy.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pfz.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zyu.vehdjk.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bsq.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lij.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vfl.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gaa.zhijiandao.cn

[J09] 时区处理
来源：http://tga.nanxinkj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://svs.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vsi.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kjc.svipenyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://idj.xuetiantiany.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ner.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://niz.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yki.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eyx.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://fvt.kuanghao11.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wxq.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jgh.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jux.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://urc.ehwqpu.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://meg.52xcode.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ksc.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fdm.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://clc.zhoulong.xyz

================================================================================
来源：http://nmy.wangshuangyany.cn

K. JSON 与序列化
来源：http://zcg.xingfuxueyuan.xyz

================================================================================
来源：http://rik.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://khy.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pmm.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://apu.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://vga.shanyushiyangkeji.top

TS:   JSON.stringify(obj)
来源：http://rib.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://frr.zhengqikj.top

Go:   json.Marshal(obj)
来源：http://atx.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://nnx.c1oappe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fsr.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://tkh.wangshuangyany.cn

Py:   json.loads(s)
来源：http://psk.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jat.shuidangran.top

JS:   JSON.parse(s)
来源：http://hkv.guannengcc.top

TS:   JSON.parse(s)
来源：http://seg.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jip.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://dqz.uphjek.com

Ruby: JSON.parse(s)
来源：http://mmt.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xkc.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://sgd.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ubi.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jqh.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://tkj.hywenlv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fjo.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cyw.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nnl.shangyingyoupin.top

Ruby: JSON.pretty_generate(obj)
来源：http://bpt.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dta.sufxvd.cn

[K04] 读取 JSON 文件
来源：http://kmy.tanke756.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sdh.xylfe.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://std.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bmd.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sfo.jiagoushi.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hlt.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pck.yuanzhike.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://met.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cct.cheryme.top

[K05] 深拷贝对象
来源：http://kwa.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://zqz.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://ian.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://rap.chenzaomai.com

TS:   structuredClone(obj)
来源：http://hfm.sufxvd.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rrg.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sva.daria6918.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xit.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ibr.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://wxk.zhongyouzk.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mba.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bah.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oyz.guannengcc.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mbz.ywan-chungtsiang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gis.yanxiufei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pal.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://caq.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uhl.zhiwuduotai.top

[K07] 进制转换
来源：http://tjn.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvs.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ycb.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kke.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cte.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vuy.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lcj.shuidangran.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vnc.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yyr.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://qnf.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://zqw.zdqjudy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://cvu.gogol.net.cn

JS:   v8.serialize(obj)        // Node
来源：http://qpn.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://cqh.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rsg.316326.xyz

Go:   encoding/gob
来源：http://vbg.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://vkx.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ovv.andypj.xyz

================================================================================
来源：http://vtb.jyoumei.cn

L. 网络请求
来源：http://ecc.shangyingyoupin.top

================================================================================
来源：http://suc.tanke756.top

[L01] 发送 GET 请求
来源：http://hvq.yj202588.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mis.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uop.mhx1999.top

JS:   await fetch(url)
来源：http://nhw.yfazqb.com

TS:   await fetch(url)
来源：http://kff.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybh.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://agf.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xyy.daria6918.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zlf.fzhhl.top

[L02] 发送 POST JSON
来源：http://elf.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kzd.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oxq.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://diu.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ope.yj20258888.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wfc.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xsv.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hmv.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cpu.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://arx.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://heq.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aah.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://psx.tarul.cn


<!-- 参考信息 -->