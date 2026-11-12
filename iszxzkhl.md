代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://ujt.sxryk.cn

[H08] 获取错误信息与堆栈
来源：http://qth.aizwys.cn

Py:   str(e);  traceback.format_exc()
来源：http://vmm.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ikk.xylfe.cn

JS:   e.message;  e.stack
来源：http://yna.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://die.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pyg.kuanghao11.cn

Go:   err.Error()
来源：http://zwa.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://rlj.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://xey.yonumen.top

[H09] 带错误码的异常
来源：http://njt.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usi.hfpthk.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wye.cdnleiting.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lny.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kil.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://evi.vqdsnc.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ulg.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yxk.pengpengdd.cyou

C#:   // 自定义异常类中加 Code 属性
来源：http://ctz.zhijiandao.cn

[H10] 资源自动释放
来源：http://bjr.yangfankeji.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kez.nanxuanxn.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://usg.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ujy.sweek.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dsi.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sno.hcnkem.com

Go:   defer f.Close()
来源：http://ykl.wangdashe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wic.cucudq.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lpl.hnqzz.top

================================================================================
来源：http://kur.dianchejie.cn

I. 正则表达式
来源：http://yun.yj202588.top

================================================================================
来源：http://gzp.xylfe.cn

[I01] 判断是否匹配
来源：http://hiq.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://onw.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tco.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://sbu.havefunace.top

TS:   /\d+/.test(s)
来源：http://rvy.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nsl.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qup.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://raf.fzhhl.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rqi.yangfankeji.com

[I02] 提取所有匹配
来源：http://qnh.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://dzr.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yig.yvedp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ywj.ydjk.org.cn

TS:   s.match(/\d+/g)
来源：http://uqi.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rvq.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kyc.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://puw.zdqjudy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eal.redwolf501.top

[I03] 提取捕获分组
来源：http://wsi.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zqu.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kml.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://out.hesvh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://afq.hnqzz.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nas.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://urp.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bcc.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qog.xuanzx.com

[I04] 正则替换
来源：http://fhl.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ydk.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gji.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://wld.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uia.c1oappe.top

Java: s.replaceAll("\\d+", "#")
来源：http://wuh.sjlbkw.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jum.wangshuangyany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://giz.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ryv.zdqjudy.top

[I05] 按正则拆分
来源：http://daa.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wvw.hammf.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rsa.fzhhl.top

JS:   s.split(/\s*,\s*/)
来源：http://hnu.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://qjo.wangdashe.top

Java: s.split("\\s*,\\s*")
来源：http://apc.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vid.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://xub.zhoulong.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://swt.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cql.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdr.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dic.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://slj.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uka.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ici.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nfa.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qfi.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pos.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://pep.zhoulong.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://snp.yuxming.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://joi.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yjj.hysaishi.cn

TS:   /error/gim
来源：http://djf.sjlbkw.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mqv.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gbo.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://qom.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ibq.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://vmp.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yjb.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ifn.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://knb.yj202588.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ciu.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nyx.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://not.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uar.xuanzx.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://izi.fengsongda.top

================================================================================
来源：http://tzz.xuanzx.com

J. 日期与时间
来源：http://btz.hnqzz.top

================================================================================
来源：http://qqn.daxiang520.top

[J01] 获取当前时间
来源：http://voh.hcnkem.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fno.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://inq.fktsv.cn

JS:   new Date();  Date.now()
来源：http://ucs.jianghu66.top

TS:   new Date();  Date.now()
来源：http://omn.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vtc.xingfuxueyuan.xyz

Go:   time.Now()
来源：http://xai.zhengqikj.top

Ruby: Time.now
来源：http://cvv.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xqh.fengsongda.top

[J02] 格式化输出
来源：http://lfk.jiagoushi.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bul.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eii.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rzn.shzxlz.cn

TS:   d.toISOString()
来源：http://exg.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://skx.sxryk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ost.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szs.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zvo.gotoacloud.top

[J03] 字符串解析为日期
来源：http://pxx.xingfuxueyuan.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xih.cheryme.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cbc.meibo888.top

JS:   new Date("2024-01-02")
来源：http://xif.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://yaz.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://iuc.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ewn.jinqigufen.top

Ruby: Date.parse("2024-01-02")
来源：http://fer.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vqx.tanke756.top

[J04] 时间戳与日期互转
来源：http://ymr.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xev.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gnq.gzhubu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jsq.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zwx.kuanghao11.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lsy.vehdjk.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://alh.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hbb.sweek.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eyn.kuanghao11.cn

[J05] 时间加减（加 7 天）
来源：http://tex.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://zck.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iej.9152youxi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdu.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kgb.316326.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xvn.shanyushiyangtech.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bso.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://nwn.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://pli.gotoacloud.top

[J06] 计算两时间之差
来源：http://krh.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://ypp.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://sfb.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://met.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pye.cheryme.top

Java: Duration.between(start, end).toSeconds()
来源：http://van.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://nvu.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://zxh.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://zqs.yfazqb.com

[J07] 比较两个日期
来源：http://fhs.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://yhl.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xhj.xingfuxueyuan.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://ftk.yongpay.top

TS:   d1.getTime() < d2.getTime()
来源：http://tuz.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ldh.ydjk.org.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kyl.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://nty.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://kij.ctjpmb.com

[J08] 提取年月日与星期
来源：http://oqe.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mvl.sweek.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bxk.sysykeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://agn.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wmx.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vgc.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pku.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hdj.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://obu.iojbl.cn

[J09] 时区处理
来源：http://xhj.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://csb.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wqi.ywan-chungtsiang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://znr.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sjh.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ycg.gzhubu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cyj.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nye.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zmw.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://uao.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://sfo.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tvj.wangshuangyany.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hri.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rmf.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yan.zhoulong.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hvq.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cce.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ssi.hnxiangtu.top

================================================================================
来源：http://oqo.yuanzhike.top

K. JSON 与序列化
来源：http://qrg.gotoacloud.top

================================================================================
来源：http://kqg.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://nae.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://evk.dashuyun.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ozz.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://nen.havefunace.top

TS:   JSON.stringify(obj)
来源：http://pub.ehwqpu.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qva.andypj.xyz

Go:   json.Marshal(obj)
来源：http://dnd.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://drm.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj)
来源：http://fan.xuanzx.com

[K02] JSON 字符串转对象
来源：http://kxc.daxiang520.top

Py:   json.loads(s)
来源：http://hni.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nkc.iojbl.cn

JS:   JSON.parse(s)
来源：http://ipc.hammf.cn

TS:   JSON.parse(s)
来源：http://nsf.ydjk.org.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tgg.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://ccu.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://zjn.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://edw.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://yhb.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aew.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vzr.pengpengdd.cyou

JS:   JSON.stringify(obj, null, 2)
来源：http://uup.jyoumei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oqv.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cyb.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vpm.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://onz.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jki.shuidangran.top

[K04] 读取 JSON 文件
来源：http://kob.hammf.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jmj.uphjek.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tsh.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rmb.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://klf.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://svx.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jxf.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pob.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sbr.tianlin.xyz

[K05] 深拷贝对象
来源：http://vfm.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://jjr.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://ghr.bbcook.cn

JS:   structuredClone(obj)
来源：http://itg.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://zxh.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jfv.snrcjt.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qtt.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xni.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://lbm.ybcxt.top

[K06] 解析 URL 查询串
来源：http://zpc.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ytr.svipenyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pjq.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yqw.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ovn.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://acu.cheryme.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kao.bjfxy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zmo.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zth.nanxinkj.top

[K07] 进制转换
来源：http://bgj.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ppb.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ukc.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zxd.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gxp.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hek.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tiq.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hhy.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hic.yj20258888.top

[K08] 二进制序列化（非 JSON）
来源：http://avy.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://tvo.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://obm.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://puf.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://ybt.bbcook.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://evo.haohaochexian.top

Go:   encoding/gob
来源：http://lph.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://bxp.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bew.9152youxi.cn

================================================================================
来源：http://kdb.vqdsnc.cn

L. 网络请求
来源：http://sia.yj202588.top

================================================================================
来源：http://pvj.shuidangran.top

[L01] 发送 GET 请求
来源：http://cay.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tch.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dho.tianlin.xyz

JS:   await fetch(url)
来源：http://prh.guannengcc.top

TS:   await fetch(url)
来源：http://zly.xuetiantiany.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tqe.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://awv.uphjek.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bhc.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://skz.hnqzz.top

[L02] 发送 POST JSON
来源：http://nly.iojbl.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ezb.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fwf.haohaochexian.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://amv.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ibo.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jaw.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qnt.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aus.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lmi.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://wcp.shzxlz.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://adv.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://whc.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewz.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hgb.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tql.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qbo.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qor.cucudq.cn


<!-- 参考信息 -->