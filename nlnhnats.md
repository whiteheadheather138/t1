代发 wailian999

JS:   e.message;  e.stack
来源：http://btn.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://snj.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://yfq.quarkkingdee.top

Go:   err.Error()
来源：http://hrg.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://vsm.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://fbw.birdmap.top

[H09] 带错误码的异常
来源：http://nfp.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dpt.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rgr.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ebu.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nju.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ubl.hongshengwenyu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yuv.yuanzhike.top

Ruby: raise MyError.new("fail", 500)
来源：http://mxo.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hrv.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://hbz.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://sfc.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://has.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ewl.cashguo.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cgj.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uqv.birdmap.top

Go:   defer f.Close()
来源：http://ulz.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://szn.wangdashe.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gbe.hcnkem.com

================================================================================
来源：http://jme.shangyingyoupin.top

I. 正则表达式
来源：http://jmw.zycfv.cn

================================================================================
来源：http://ydd.fengsongda.top

[I01] 判断是否匹配
来源：http://men.yuxming.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ybx.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://fiu.mhx1999.top

JS:   /\d+/.test(s)
来源：http://koe.tian-w.cn

TS:   /\d+/.test(s)
来源：http://ibs.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fak.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ibr.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://mvd.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wij.quarkkingdee.top

[I02] 提取所有匹配
来源：http://fwx.snrcjt.cn

Py:   re.findall(r"\d+", s)
来源：http://zcw.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://itg.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pra.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://kzp.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lba.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ids.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://riy.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sno.jlsjyb.cn

[I03] 提取捕获分组
来源：http://kto.gogol.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fvc.vehdjk.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jqo.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pto.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ikc.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tbj.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jus.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gym.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mvh.0kj1m.cn

[I04] 正则替换
来源：http://sgi.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fld.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kew.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mnw.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://ghb.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rxn.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eda.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://esh.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yxk.epnwcf.com

[I05] 按正则拆分
来源：http://wkk.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rga.yuanzhike.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jjv.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://pkt.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://hrk.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://mmm.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sfo.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://hxf.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pcc.smart0.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ehi.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aet.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fps.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jta.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://snr.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://loi.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://czp.9152youxi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bjw.xingfuxueyuan.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hgk.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://xug.jinqigfzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mmc.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ngk.tian-w.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dta.wangdashe.top

TS:   /error/gim
来源：http://cwx.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwh.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xlh.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://wmi.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sqq.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://kdm.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tdn.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ses.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rms.fanxiaobao.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dyl.chenjidiqi.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://rpb.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zfy.gotoacloud.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fon.daxiang520.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fwx.ivvv.top

================================================================================
来源：http://wfg.zhoulong.xyz

J. 日期与时间
来源：http://fwd.vqdsnc.cn

================================================================================
来源：http://zbu.xziqi.cn

[J01] 获取当前时间
来源：http://bol.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nzp.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mun.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://zec.yueranfly.top

TS:   new Date();  Date.now()
来源：http://ipz.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qbn.tianlin.xyz

Go:   time.Now()
来源：http://onc.guannengcc.top

Ruby: Time.now
来源：http://pfs.ybcxt.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uyw.fanxiaobao.xyz

[J02] 格式化输出
来源：http://ork.wangdashe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fox.sufxvd.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dna.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wkf.9152youxi.cn

TS:   d.toISOString()
来源：http://idn.uphjek.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vkz.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wxv.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://snq.yvedp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uvb.tianlin.xyz

[J03] 字符串解析为日期
来源：http://hlg.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nfl.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qsw.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://kqd.hysaishi.cn

TS:   new Date("2024-01-02")
来源：http://hjq.aibaodan.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gzw.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yxx.nanxinkj.top

Ruby: Date.parse("2024-01-02")
来源：http://mjv.zhiwuduotai.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qhx.316326.xyz

[J04] 时间戳与日期互转
来源：http://ion.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mnu.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vdc.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oku.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jsd.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cko.jqgfzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xwz.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://auj.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bbk.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://bgc.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://kot.kuanghao11.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sql.tian-w.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzl.fengsongda.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cgw.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://rpk.jinghuilouyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ucl.hfpthk.cn

Ruby: Time.now + 7 * 86400
来源：http://pxl.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://yid.jinghuilouyu.cn

[J06] 计算两时间之差
来源：http://nej.jqgfzy.top

Py:   (end - start).total_seconds()
来源：http://fmv.tianlin.xyz

PHP:  $end->diff($start)->days;
来源：http://skc.gaohongyu789.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qrj.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wpo.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://xrv.zhaomingkeji.xyz

Go:   end.Sub(start).Hours()
来源：http://qoz.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://wvh.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://obg.yj202588.top

[J07] 比较两个日期
来源：http://nqi.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://usd.yangfankeji.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vlu.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://alf.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://mpc.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://top.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zyw.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tqm.feifeiyinyue.top

C#:   d1 < d2;  d1 == d2
来源：http://cdd.snrcjt.cn

[J08] 提取年月日与星期
来源：http://ttw.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hyq.chenjidiqi.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gua.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bad.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://njh.cqqwz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ahv.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://abq.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://esm.kuanghao11.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lyi.sweek.top

[J09] 时区处理
来源：http://twy.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzi.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhp.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pns.yanxiufei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tfk.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vex.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://icr.yj20258888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fhr.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kkv.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://zzc.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vsh.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dmi.sysykeji.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xzh.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czl.wangdashe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zeq.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xlu.jinyuanbaomall.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wes.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cbr.sweek.top

================================================================================
来源：http://zxk.smart0.xyz

K. JSON 与序列化
来源：http://rfu.shuidangran.top

================================================================================
来源：http://yyo.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://dfm.zhijiandao.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cdj.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wna.yongpay.top

JS:   JSON.stringify(obj)
来源：http://yeu.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://vle.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mhz.hesvh.cn

Go:   json.Marshal(obj)
来源：http://kjc.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bpm.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ulr.fktsv.cn

[K02] JSON 字符串转对象
来源：http://uon.ppjwa.cn

Py:   json.loads(s)
来源：http://eut.gzhubu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hgy.svipenyu.cn

JS:   JSON.parse(s)
来源：http://cvb.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://lgs.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bwg.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://ekp.fzhhl.top

Ruby: JSON.parse(s)
来源：http://yua.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yof.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://xlb.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zjx.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kgc.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nbn.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wbj.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tqp.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vbi.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://nhy.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rwk.sxryk.cn

[K04] 读取 JSON 文件
来源：http://gbl.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://orb.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://osm.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://luy.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dbm.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ifp.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tyz.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://the.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vnu.shanyushiyangkeji.top

[K05] 深拷贝对象
来源：http://xru.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://usk.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://vef.zdqjudy.top

JS:   structuredClone(obj)
来源：http://ngd.hnqzz.top

TS:   structuredClone(obj)
来源：http://zjc.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ase.vqdsnc.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://opm.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xwx.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bxv.epnwcf.com

[K06] 解析 URL 查询串
来源：http://shj.zhoulong.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uus.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zng.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kcm.feifeiyinyue.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yjn.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sdu.jinqigfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjb.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uvf.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nio.hfpthk.cn

[K07] 进制转换
来源：http://pwc.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ztk.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rgc.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vli.xingfuxueyuan.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cpn.pengpengdd.cyou

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pzb.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zln.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xpk.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ygo.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://soa.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://uaz.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cvz.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://oua.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://soi.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xmh.cdnleiting.top

Go:   encoding/gob
来源：http://vdb.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://hht.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://akt.gzhubu.top

================================================================================
来源：http://dlp.jinqigufen.top

L. 网络请求
来源：http://ywp.jinqigufen.top

================================================================================
来源：http://fcf.yangfankeji.com

[L01] 发送 GET 请求
来源：http://ahb.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zhg.wangshuangyany.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ain.dianchejie.cn

JS:   await fetch(url)
来源：http://cyw.epnwcf.com

TS:   await fetch(url)
来源：http://sqa.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baf.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://ntt.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://feg.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zin.cqqwz.cn

[L02] 发送 POST JSON
来源：http://psv.fehbvm.com

Py:   requests.post(url, json={"a": 1})
来源：http://fay.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vit.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zfa.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ioa.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eif.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kht.zhengqikj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dvz.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uti.redwolf501.top

[L03] 设置自定义请求头
来源：http://kfs.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fef.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wzy.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mdv.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rhx.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://syj.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nye.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjl.daria6918.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cgi.xuanzx.com

[L04] 设置超时
来源：http://rfp.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://kas.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lxo.andypj.xyz


<!-- 参考信息 -->