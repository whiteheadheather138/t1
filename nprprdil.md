代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://qvp.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://wui.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://nkq.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yha.jiagoushi.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tra.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hgm.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iys.kuanghao11.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dnv.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jyd.sjlbkw.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rlz.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dvz.hcnkem.com

[H10] 资源自动释放
来源：http://ffi.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mwa.ctjpmb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bqf.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qxo.0kj1m.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gsk.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xar.haohaochexian.top

Go:   defer f.Close()
来源：http://akw.xziqi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gsp.xylfe.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lqb.shangyingyoupin.top

================================================================================
来源：http://ted.yuxming.cn

I. 正则表达式
来源：http://tpf.cdnleiting.top

================================================================================
来源：http://ybz.meibo888.top

[I01] 判断是否匹配
来源：http://wlh.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tqp.daria6918.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wlk.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://izs.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://gzs.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qvp.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uja.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://ljs.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lby.ivvv.top

[I02] 提取所有匹配
来源：http://ksj.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://guw.shzxlz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nfg.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lml.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://qpz.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lbb.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qod.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://mqf.zdbjq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mya.chenzaomai.com

[I03] 提取捕获分组
来源：http://jdz.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ogj.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xbz.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qtk.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fiz.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nlw.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cfh.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eom.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mcc.hywenlv.cn

[I04] 正则替换
来源：http://miw.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://pfc.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yny.shanyushiyangtech.top

JS:   s.replace(/\d+/g, "#")
来源：http://idc.daria6918.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nom.yongpay.top

Java: s.replaceAll("\\d+", "#")
来源：http://skp.0kj1m.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qgi.chenzaomai.com

Ruby: s.gsub(/\d+/, "#")
来源：http://idq.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://phs.hammf.cn

[I05] 按正则拆分
来源：http://mzi.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rql.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cgb.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://iss.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://bfa.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://luc.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kfw.epnwcf.com

Ruby: s.split(/\s*,\s*/)
来源：http://vdz.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://waa.dianchejie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oji.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tnv.guowangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gbp.zdqjudy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vpb.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zwy.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fys.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzs.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dop.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://znt.ppjwa.cn

[I07] 忽略大小写与多行模式
来源：http://cnu.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://axb.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cxd.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tpx.yj202588.top

TS:   /error/gim
来源：http://blq.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xkp.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgw.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://zfc.bjfxy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azq.ywan-chungtsiang.top

[I08] 贪婪与非贪婪匹配
来源：http://ppi.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pbv.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ent.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ckb.yanxiufei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://twv.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nxl.fzhhl.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ket.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rwo.jyoumei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sbb.yj202588.top

================================================================================
来源：http://hse.jianghu66.top

J. 日期与时间
来源：http://scf.svipenyu.cn

================================================================================
来源：http://zlv.hnxiangtu.top

[J01] 获取当前时间
来源：http://met.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cau.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://skq.fehbvm.com

JS:   new Date();  Date.now()
来源：http://lqc.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://hdj.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jvp.hongshengwenyu.top

Go:   time.Now()
来源：http://zgk.snrcjt.cn

Ruby: Time.now
来源：http://ked.shanyushiyangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dwk.zdbjq.cn

[J02] 格式化输出
来源：http://uzm.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://drc.yanxiufei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lyj.ehwqpu.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ahq.nwbrower.top

TS:   d.toISOString()
来源：http://gsp.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gmr.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lcz.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bfp.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ueo.shangyingyoupin.top

[J03] 字符串解析为日期
来源：http://wts.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dmu.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kdy.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://tkj.nanxuanxn.top

TS:   new Date("2024-01-02")
来源：http://awg.chenlongwang.top

Java: LocalDate.parse("2024-01-02")
来源：http://jqi.xinyue.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gvz.xinyue.icu

Ruby: Date.parse("2024-01-02")
来源：http://glw.hcnkem.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rja.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://vom.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iax.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uwd.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://axk.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://wwo.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hgg.guowangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nrt.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ivu.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jdi.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://upb.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://vhx.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xwj.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujd.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nem.chenzaomai.com

Java: LocalDate.now().plusDays(7)
来源：http://ldl.jqgufenzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wee.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://eds.havefunace.top

C#:   DateTime.Now.AddDays(7)
来源：http://ayi.nanxinkj.top

[J06] 计算两时间之差
来源：http://pzg.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://ffg.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://xsu.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dxk.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wdg.shanyushiyangtech.top

Java: Duration.between(start, end).toSeconds()
来源：http://jsv.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://msb.pycfn.com

Ruby: end - start                 # 返回秒数
来源：http://pie.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://mth.yuxming.cn

[J07] 比较两个日期
来源：http://ndd.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ntu.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gib.wangshuangyany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bhx.ctjpmb.com

TS:   d1.getTime() < d2.getTime()
来源：http://ckk.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://srs.pengpengdd.cyou

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gtw.hcnkem.com

Ruby: d1 < d2;  d1 == d2
来源：http://tgb.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://anq.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://eds.jianghu66.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://osu.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mrw.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://owe.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vjt.hnxiangtu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wke.fktsv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fer.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vix.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ghx.xinyue.icu

[J09] 时区处理
来源：http://mdc.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hwy.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://api.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qnz.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gon.sweek.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qua.yj20258888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ypc.havefunace.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zfb.ehwqpu.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kul.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://eat.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xhi.dashuyun.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wzo.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zzb.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mis.ctjpmb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vqp.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bmh.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zor.gaohongyu789.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hts.yj202588.top

================================================================================
来源：http://mdu.zhoulong.xyz

K. JSON 与序列化
来源：http://qzz.daria6918.cn

================================================================================
来源：http://itt.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://wkj.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dep.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ssu.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://ggc.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://mbm.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vvw.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://qzb.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://qeq.svipenyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wib.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://bul.vehdjk.com

Py:   json.loads(s)
来源：http://iyc.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kjv.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://vlu.hesvh.cn

TS:   JSON.parse(s)
来源：http://prh.jinqigufen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vwd.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://pfy.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://ctq.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ybm.cqqwz.cn

[K03] JSON 美化输出（带缩进）
来源：http://ynp.cashguo.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wve.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dzg.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iwz.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mpb.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aip.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ulg.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gkr.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jbm.bjfxy.top

[K04] 读取 JSON 文件
来源：http://kdu.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tyw.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kxh.andypj.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yho.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rnm.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ufh.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pmt.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uye.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ujz.hnxiangtu.top

[K05] 深拷贝对象
来源：http://vnm.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://ltv.kuanghao11.cn

PHP:  unserialize(serialize($obj));
来源：http://fuk.vehdjk.com

JS:   structuredClone(obj)
来源：http://yrx.9152youxi.cn

TS:   structuredClone(obj)
来源：http://bet.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wts.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://use.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wyc.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ilh.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://lcz.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bou.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kse.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ycs.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://upj.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nyu.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dik.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lse.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://crz.gogol.net.cn

[K07] 进制转换
来源：http://riu.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pji.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cgw.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ify.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://exb.yvedp.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kkh.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://scr.iojbl.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jmm.zhixingplan.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://orw.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://xke.hysaishi.cn

Py:   pickle.dumps(obj)
来源：http://hus.wangdashe.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dnv.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://pwz.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://fbo.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mpc.yangfankeji.com

Go:   encoding/gob
来源：http://fky.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://vaq.dashuyun.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wke.0kj1m.cn

================================================================================
来源：http://osf.yj20258.top

L. 网络请求
来源：http://nin.ydzc1.top

================================================================================
来源：http://lkx.ybcxt.top

[L01] 发送 GET 请求
来源：http://niq.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uzb.cheryme.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fdk.fktsv.cn

JS:   await fetch(url)
来源：http://tcw.zhixingplan.top

TS:   await fetch(url)
来源：http://xqs.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lxf.316326.xyz

Go:   resp, err := http.Get(url)
来源：http://kgq.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uzf.guannengcc.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ntd.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://hkh.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://ehn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tjd.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gir.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yty.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dxv.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nxd.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zyg.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gcl.haohaochexian.top

[L03] 设置自定义请求头
来源：http://wrg.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ntw.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zcw.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyc.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mpb.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wsa.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hej.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ooa.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://phf.uphjek.com

[L04] 设置超时
来源：http://nfz.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://rfg.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uij.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fiz.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bkn.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jgs.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bus.hfpthk.cn


<!-- 参考信息 -->