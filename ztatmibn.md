代发 wailian999

TS:   console.assert(x > 0);
来源：http://onc.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://iln.shanyushiyangkeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://odv.dashuyun.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fyw.iojbl.cn

C#:   Debug.Assert(x > 0);
来源：http://uwz.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://dap.zhixingplan.top

Py:   str(e);  traceback.format_exc()
来源：http://tvg.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ybk.cheryme.top

JS:   e.message;  e.stack
来源：http://wza.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vyh.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://fkg.zhiwuduotai.top

Go:   err.Error()
来源：http://nmu.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://aem.xuetiantiany.cn

C#:   e.Message;  e.StackTrace
来源：http://rsm.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://ipe.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fyt.chenlongwang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://zyp.tian-w.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uiq.zhaomingkeji.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ngy.c1oappe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lmt.andypj.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wyo.cdnleiting.top

Ruby: raise MyError.new("fail", 500)
来源：http://xno.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yvh.shanyushiyangkeji.top

[H10] 资源自动释放
来源：http://jeq.hfpthk.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uhx.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qtu.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zcu.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://abn.zhengqikj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fnu.wangshuangyany.cn

Go:   defer f.Close()
来源：http://gxh.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rhg.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gkl.jinqigfzy.top

================================================================================
来源：http://ozp.shangyingyoupin.top

I. 正则表达式
来源：http://anl.zycfv.cn

================================================================================
来源：http://for.yonumen.top

[I01] 判断是否匹配
来源：http://kql.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ecb.dianchejie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jzr.yuxming.cn

JS:   /\d+/.test(s)
来源：http://nyo.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://yek.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qnl.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://glp.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://wli.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mbv.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://zmv.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://ynn.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgk.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://twv.yj20258.top

TS:   s.match(/\d+/g)
来源：http://rrd.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vyy.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mdb.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://qee.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://how.tianlin.xyz

[I03] 提取捕获分组
来源：http://xxu.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tkk.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gub.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jqu.havefunace.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bcw.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://afb.aibaodan.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aol.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qfy.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://swj.jinyuanbaomall.cn

[I04] 正则替换
来源：http://dbr.dianchejie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://thg.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ugk.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://nsl.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://prs.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://dqs.guowangkeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vnr.cheryme.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hwd.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uba.andypj.xyz

[I05] 按正则拆分
来源：http://tnk.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rtm.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nvu.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://gkt.52xcode.cn

TS:   s.split(/\s*,\s*/)
来源：http://htt.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://xhq.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hui.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://dun.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tid.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iqc.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bqd.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yak.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbw.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ldr.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tam.vehdjk.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://geg.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yjj.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://clm.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://pes.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zcu.jinqigufen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://afv.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ext.yvedp.cn

TS:   /error/gim
来源：http://nsi.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://siw.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eme.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://cbc.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://chq.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://fzk.cdnleiting.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jhf.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qlu.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bqh.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://umj.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://cdh.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ntv.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hgn.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zmu.ehwqpu.com

================================================================================
来源：http://onk.kuanghao11.cn

J. 日期与时间
来源：http://gew.jinghuilouyu.cn

================================================================================
来源：http://mcy.cheryme.top

[J01] 获取当前时间
来源：http://nfv.shzxlz.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wgo.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ioy.wangshuangyany.cn

JS:   new Date();  Date.now()
来源：http://asz.shanyushiyangkeji.top

TS:   new Date();  Date.now()
来源：http://oec.zdbjq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nll.xinyue.icu

Go:   time.Now()
来源：http://shy.yj20258888.top

Ruby: Time.now
来源：http://rof.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://laq.hcnkem.com

[J02] 格式化输出
来源：http://gaq.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ugn.gaohongyu789.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vrd.cucudq.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tnt.cucudq.cn

TS:   d.toISOString()
来源：http://prg.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aox.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vbl.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bwu.kuanghao11.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ott.yonumen.top

[J03] 字符串解析为日期
来源：http://dem.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pty.vqdsnc.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dyt.yuanzhike.top

JS:   new Date("2024-01-02")
来源：http://mri.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://bgp.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qpa.fzhhl.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aga.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://nyn.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fug.yonumen.top

[J04] 时间戳与日期互转
来源：http://cqp.gaohongyu789.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dmf.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ajh.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kux.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fxy.guannengcc.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rlp.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://owb.yj202588.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nau.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rks.chenzaomai.com

[J05] 时间加减（加 7 天）
来源：http://brp.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://gzk.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://tgb.yonumen.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kaf.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jqa.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://inv.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://umc.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://ege.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://dzf.quarkkingdee.top

[J06] 计算两时间之差
来源：http://dyu.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://jfv.yj202588.top

PHP:  $end->diff($start)->days;
来源：http://egm.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fro.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sot.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://nbe.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://dlx.hysaishi.cn

Ruby: end - start                 # 返回秒数
来源：http://bas.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://fie.hongshengwenyu.top

[J07] 比较两个日期
来源：http://mbk.tanke756.top

Py:   d1 < d2;  d1 == d2
来源：http://ktt.ehwqpu.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ucf.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oxq.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://umm.yanxiufei.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pax.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tii.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fcl.guowangkeji.top

C#:   d1 < d2;  d1 == d2
来源：http://rqn.zhoulong.xyz

[J08] 提取年月日与星期
来源：http://ldi.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vim.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mxv.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://osh.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oon.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fpn.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oac.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tdv.andypj.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://faf.fktsv.cn

[J09] 时区处理
来源：http://hel.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ypq.uphjek.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wce.shangyingyoupin.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbh.ctjpmb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpz.mhx1999.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qym.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ipn.chenzaomai.com

Ruby: Time.now.getlocal("+08:00")
来源：http://yod.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hsc.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://ukt.xuetiantiany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xft.sxryk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cza.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hfz.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tqk.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://crf.daxiang520.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://adk.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vle.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wsf.jinqigfzy.top

================================================================================
来源：http://nxy.zhiwuduotai.top

K. JSON 与序列化
来源：http://cis.cdnleiting.top

================================================================================
来源：http://jab.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://vzj.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ggd.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zin.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://tuj.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://zvt.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nnv.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://gms.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://icf.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dhi.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://jbg.jlsjyb.cn

Py:   json.loads(s)
来源：http://qnk.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://atw.guowangkeji.top

JS:   JSON.parse(s)
来源：http://zub.52xcode.cn

TS:   JSON.parse(s)
来源：http://aya.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aam.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://jve.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://edh.c1oappe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jnq.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://qqr.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bgu.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sry.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bbw.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ebi.xuetiantiany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://leb.cucudq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ncv.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://tir.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uxi.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://tht.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gex.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://efx.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jcc.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jbz.epnwcf.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://faw.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://snt.hnqzz.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rcs.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kqx.shzxlz.cn

[K05] 深拷贝对象
来源：http://bqh.smart0.xyz

Py:   copy.deepcopy(obj)
来源：http://hdm.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://uui.daria6918.cn

JS:   structuredClone(obj)
来源：http://kbr.gzhubu.top

TS:   structuredClone(obj)
来源：http://mrq.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://nqo.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ubc.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qvk.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vqn.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://xbt.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ovc.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lpo.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ass.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjx.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uqw.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://tov.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wpm.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yli.aibaodan.cn

[K07] 进制转换
来源：http://cxe.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://psx.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dca.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cfx.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fhz.gaohongyu789.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rpx.sjlbkw.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ntz.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qko.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tlz.nanxinkj.top

[K08] 二进制序列化（非 JSON）
来源：http://qkm.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://nwe.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rge.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://ooj.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://hgn.shanyushiyangtech.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://loj.sxryk.cn

Go:   encoding/gob
来源：http://yxh.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://ixo.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fpn.xylfe.cn

================================================================================
来源：http://cpl.gotoacloud.top

L. 网络请求
来源：http://xxg.cdnleiting.top

================================================================================
来源：http://beb.yuxming.cn

[L01] 发送 GET 请求
来源：http://uab.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://siq.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lsd.guowangkeji.top

JS:   await fetch(url)
来源：http://akl.cucudq.cn

TS:   await fetch(url)
来源：http://uhd.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fpo.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://pct.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iut.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yli.hesvh.cn

[L02] 发送 POST JSON
来源：http://dug.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://cbc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nfh.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://acs.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lvc.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vtu.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hmc.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hpn.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gmv.bjfxy.top

[L03] 设置自定义请求头
来源：http://lrf.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tyk.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gvv.yj202588.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oar.yonumen.top


<!-- 参考信息 -->