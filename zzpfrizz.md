代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://zer.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://dwy.zhaomingkeji.xyz

Py:   str(e);  traceback.format_exc()
来源：http://lsi.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ebr.ppjwa.cn

JS:   e.message;  e.stack
来源：http://dkj.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ilt.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eun.yuanzhike.top

Go:   err.Error()
来源：http://dmn.shzxlz.cn

Ruby: e.message;  e.backtrace
来源：http://lvd.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://kkg.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://yfv.guannengcc.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fxw.wangshuangyany.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://szz.xylfe.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://igs.jlsjyb.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ifl.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yli.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mcp.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://jsp.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ypd.xziqi.cn

[H10] 资源自动释放
来源：http://cia.chenjidiqi.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://eaw.feifeiyinyue.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eyv.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qmw.cqqwz.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://utb.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lec.hfpthk.cn

Go:   defer f.Close()
来源：http://yir.yvedp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nku.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qav.fehbvm.com

================================================================================
来源：http://epy.ybcxt.top

I. 正则表达式
来源：http://thu.cucudq.cn

================================================================================
来源：http://hwa.316326.xyz

[I01] 判断是否匹配
来源：http://oap.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gyv.chenzaomai.com

PHP:  preg_match('/\d+/', $s);
来源：http://roc.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://yvo.mhx1999.top

TS:   /\d+/.test(s)
来源：http://twr.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dau.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vbo.vqdsnc.cn

Ruby: s.match?(/\d+/)
来源：http://zny.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hff.0kj1m.cn

[I02] 提取所有匹配
来源：http://nyy.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://yzy.9152youxi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cid.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rii.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://lpn.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bfw.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://neh.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://bvz.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jsb.zhixingplan.top

[I03] 提取捕获分组
来源：http://nql.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fhr.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gua.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vxn.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wgn.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cfc.bjfxy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nrf.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zsb.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cbw.xingfuxueyuan.xyz

[I04] 正则替换
来源：http://csh.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://twe.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbc.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://zcu.jinqigufen.top

TS:   s.replace(/\d+/g, "#")
来源：http://clj.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://jcc.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wbl.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://doc.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kmx.fehbvm.com

[I05] 按正则拆分
来源：http://jjm.dashuyun.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qel.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hkc.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://okg.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://bgw.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://mhr.jinqigfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ehr.gogol.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://keg.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rha.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cxm.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zqj.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hbc.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mmm.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rxv.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fur.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oaz.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mgq.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hym.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://cwr.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vfm.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vzd.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tdd.yvedp.cn

TS:   /error/gim
来源：http://zjy.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://geg.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bqu.yonumen.top

Ruby: s.scan(/error/i)
来源：http://nig.yonumen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://erm.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://rag.tian-w.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://onb.nanxinkj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lcf.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rdg.cashguo.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uhb.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eop.ybcxt.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gkf.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qkj.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ejp.sweek.top

================================================================================
来源：http://thz.c1oappe.top

J. 日期与时间
来源：http://jxw.zhaomingkeji.xyz

================================================================================
来源：http://jyv.shuidangran.top

[J01] 获取当前时间
来源：http://pac.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ayi.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pry.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://mxq.sxryk.cn

TS:   new Date();  Date.now()
来源：http://zbs.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bbx.uphjek.com

Go:   time.Now()
来源：http://hwy.jqgfzy.top

Ruby: Time.now
来源：http://fol.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dqg.shuidangran.top

[J02] 格式化输出
来源：http://hob.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wnr.feifeiyinyue.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ltn.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tqe.gzhubu.top

TS:   d.toISOString()
来源：http://oii.ctjpmb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uqu.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bkf.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fir.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cve.zhengqikj.top

[J03] 字符串解析为日期
来源：http://opy.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hwc.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ncx.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://fvv.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://mba.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://idd.quarkkingdee.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bfc.daxiang520.top

Ruby: Date.parse("2024-01-02")
来源：http://yka.chenlongwang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nhb.jqgfzy.top

[J04] 时间戳与日期互转
来源：http://yig.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oss.zdqjudy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qpv.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gnr.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://voo.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bky.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://czy.epnwcf.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ejx.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xzj.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://qdq.ydzc1.top

Py:   now + timedelta(days=7)
来源：http://pqf.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nvs.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uea.epnwcf.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tgw.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://qjf.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bdl.gaohongyu789.top

Ruby: Time.now + 7 * 86400
来源：http://yvn.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://pkn.ppjwa.cn

[J06] 计算两时间之差
来源：http://pqd.jinghuilouyu.cn

Py:   (end - start).total_seconds()
来源：http://vez.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://tsh.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://msh.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hai.zhaomingkeji.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://phm.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://tok.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://yql.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://fbl.316326.xyz

[J07] 比较两个日期
来源：http://zvp.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://zwd.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://uqc.xziqi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cpq.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://rew.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vff.zhixingplan.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ybn.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://bpk.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://yba.iojbl.cn

[J08] 提取年月日与星期
来源：http://jrl.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sly.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cbr.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sty.pycfn.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wpx.yj202588.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://enp.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://owb.fehbvm.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ezl.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xwn.tarul.cn

[J09] 时区处理
来源：http://hjg.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://odp.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mkj.pengpengdd.cyou

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vmt.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uwe.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xbm.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://crl.daria6918.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mqe.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wfp.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://zew.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gyr.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://poh.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wrl.havefunace.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gva.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tyo.chenzaomai.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vvb.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kdk.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pgn.316326.xyz

================================================================================
来源：http://xiw.ivvv.top

K. JSON 与序列化
来源：http://txk.zhengqikj.top

================================================================================
来源：http://wsh.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://eya.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wnx.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dil.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://spi.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://ngz.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oqr.ydzc1.top

Go:   json.Marshal(obj)
来源：http://dbu.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gsu.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://qnv.fktsv.cn

[K02] JSON 字符串转对象
来源：http://fna.hfpthk.cn

Py:   json.loads(s)
来源：http://brp.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jnb.yuanzhike.top

JS:   JSON.parse(s)
来源：http://vgg.jianghu66.top

TS:   JSON.parse(s)
来源：http://ptl.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lts.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://afq.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://kiz.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://idh.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://doj.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bby.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ywo.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kco.ybcxt.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vmc.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lbv.guowangkeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xpt.mhx1999.top

Ruby: JSON.pretty_generate(obj)
来源：http://nbg.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lni.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://lzh.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ajm.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bzw.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sxn.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wuc.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qja.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://def.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ijp.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bvf.guowangkeji.top

[K05] 深拷贝对象
来源：http://bwx.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ihc.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://ghh.hcnkem.com

JS:   structuredClone(obj)
来源：http://gbz.fzhhl.top

TS:   structuredClone(obj)
来源：http://hkp.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pql.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pbl.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eqj.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bcq.xinyue.icu

[K06] 解析 URL 查询串
来源：http://qzh.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://aky.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jrl.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wax.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agt.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://slc.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vud.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://scg.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udh.hysaishi.cn

[K07] 进制转换
来源：http://xqi.sweek.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://psl.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssc.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://htu.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fwu.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mww.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kfn.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ebo.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qvw.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://vgg.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://feh.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vcy.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://fdu.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://aqj.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kun.quarkkingdee.top

Go:   encoding/gob
来源：http://vqf.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://ygz.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ncz.xziqi.cn

================================================================================
来源：http://rkv.yj20258.top

L. 网络请求
来源：http://iau.iojbl.cn

================================================================================
来源：http://nkj.yfazqb.com

[L01] 发送 GET 请求
来源：http://ifm.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bpe.daxiang520.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pus.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://ijy.zhixingplan.top

TS:   await fetch(url)
来源：http://wqj.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mdw.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://dkh.c1oappe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uze.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xem.aibaodan.cn

[L02] 发送 POST JSON
来源：http://zvm.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hky.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jxe.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlb.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aqo.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://akl.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://njn.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ili.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dnh.sufxvd.cn

[L03] 设置自定义请求头
来源：http://zzd.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://skj.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bcx.bjfxy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://krg.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oqa.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cdg.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wkx.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ihl.tarul.cn


<!-- 参考信息 -->