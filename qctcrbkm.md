代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://plr.jianghu66.top

C#:   e.Message;  e.StackTrace
来源：http://kil.yanxiufei.cn

[H09] 带错误码的异常
来源：http://zku.gzhubu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dar.yuanzhike.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sfn.xinyue.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fre.chenlongwang.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pww.hfpthk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jlp.pycfn.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zrc.yuxming.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xgy.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xbb.ehwqpu.com

[H10] 资源自动释放
来源：http://apa.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rec.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lng.52xcode.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bft.fehbvm.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wrt.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fzn.dashuyun.cn

Go:   defer f.Close()
来源：http://dif.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gps.zhoulong.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tzh.ppjwa.cn

================================================================================
来源：http://blw.cdnleiting.top

I. 正则表达式
来源：http://oqj.jianghu66.top

================================================================================
来源：http://cwi.yvedp.cn

[I01] 判断是否匹配
来源：http://jxi.cashguo.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pzi.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dik.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://slx.zhoulong.xyz

TS:   /\d+/.test(s)
来源：http://pcn.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lxe.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gvu.sxryk.cn

Ruby: s.match?(/\d+/)
来源：http://fpr.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fik.0kj1m.cn

[I02] 提取所有匹配
来源：http://dia.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://zej.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bkp.jinyuanbaomall.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bli.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://rsh.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sky.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dju.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://kut.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mls.uphjek.com

[I03] 提取捕获分组
来源：http://mcs.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uat.hnqzz.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wak.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ljx.tanke756.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xsu.shangyingyoupin.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqq.pengpengdd.cyou

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pji.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bev.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://odm.birdmap.top

[I04] 正则替换
来源：http://fjt.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ylr.shangyingyoupin.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ymk.jlsjyb.cn

JS:   s.replace(/\d+/g, "#")
来源：http://olj.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://xbs.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hxr.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://eek.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bup.tian-w.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qhs.cheryme.top

[I05] 按正则拆分
来源：http://hpr.zhoulong.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://vdt.aizwys.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cit.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://cqz.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://hco.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://uey.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uir.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://cuq.sxryk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cuy.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eje.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wus.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sok.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfd.c1oappe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eir.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xdv.hammf.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bap.havefunace.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rgy.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wqn.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://zdw.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fvp.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://acj.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://god.hnxiangtu.top

TS:   /error/gim
来源：http://elx.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vvs.jqgfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jrk.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://fza.nanxuanxn.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ftz.ppjwa.cn

[I08] 贪婪与非贪婪匹配
来源：http://rqy.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xda.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iox.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mfn.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tso.ydzc1.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ijr.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qlb.yj20258888.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wln.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ott.yuanzhike.top

================================================================================
来源：http://zog.svipenyu.cn

J. 日期与时间
来源：http://nqg.yj20258888.top

================================================================================
来源：http://bwc.ehwqpu.com

[J01] 获取当前时间
来源：http://rev.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ute.xingfuxueyuan.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ulp.jiagoushi.top

JS:   new Date();  Date.now()
来源：http://cfk.zhaomingkeji.xyz

TS:   new Date();  Date.now()
来源：http://ivo.jiagoushi.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qux.jinghuilouyu.cn

Go:   time.Now()
来源：http://srm.svipenyu.cn

Ruby: Time.now
来源：http://czj.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ukt.tian-w.cn

[J02] 格式化输出
来源：http://jzv.zycfv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ovf.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mzv.dianchejie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vhx.yj202588.top

TS:   d.toISOString()
来源：http://wcs.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iqc.chenjidiqi.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zei.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rzv.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ymk.xuanzx.com

[J03] 字符串解析为日期
来源：http://ysu.jinyuanbaomall.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://urw.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xev.xuanzx.com

JS:   new Date("2024-01-02")
来源：http://qnj.316326.xyz

TS:   new Date("2024-01-02")
来源：http://zlv.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://eia.52xcode.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://njg.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://dpu.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kho.sysykeji.top

[J04] 时间戳与日期互转
来源：http://ixp.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xsy.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qct.aizwys.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pkx.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kcq.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kda.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://acz.dianchejie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jlv.ywan-chungtsiang.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kuy.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://atn.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://mfo.gogol.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zmc.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://umc.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dko.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://rnv.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kgv.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://cfy.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://mhl.ybcxt.top

[J06] 计算两时间之差
来源：http://wjg.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://fna.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://fcq.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sfh.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yob.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ign.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://ghd.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://gsk.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://egy.zhiwuduotai.top

[J07] 比较两个日期
来源：http://kyp.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://zti.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hyg.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://xnx.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://php.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ktr.shuidangran.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://grw.yj20258.top

Ruby: d1 < d2;  d1 == d2
来源：http://ntb.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://gzo.yongpay.top

[J08] 提取年月日与星期
来源：http://sif.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ubw.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwr.wangshuangyany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fok.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cuf.hysaishi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uxl.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wqk.zdqjudy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pav.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ajy.gaohongyu789.top

[J09] 时区处理
来源：http://pwt.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yjk.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fct.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nbv.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gmk.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xyz.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bco.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qea.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oni.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://ybx.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dct.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tdw.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://osg.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nxt.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ysg.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://orr.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://shz.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tpy.zhengqikj.top

================================================================================
来源：http://ezu.tanke756.top

K. JSON 与序列化
来源：http://wdw.fzhhl.top

================================================================================
来源：http://yfr.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://gnt.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tmt.xziqi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://emp.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://cbk.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://mug.shanyushiyangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tja.yuanzhike.top

Go:   json.Marshal(obj)
来源：http://ujd.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xlf.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ffq.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://yqx.yanxiufei.cn

Py:   json.loads(s)
来源：http://mus.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pmf.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://ijs.guowangkeji.top

TS:   JSON.parse(s)
来源：http://xvr.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://btg.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://pqt.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://qym.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yhd.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://spr.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yml.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sjs.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yjg.daxiang520.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zjx.yj20258888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sxc.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nbc.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://nfm.bbcook.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jxg.svipenyu.cn

[K04] 读取 JSON 文件
来源：http://yhy.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oln.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zlt.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eby.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbp.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xgf.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fwm.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jma.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cef.ppjwa.cn

[K05] 深拷贝对象
来源：http://oga.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://pkv.yj202588.top

PHP:  unserialize(serialize($obj));
来源：http://ahs.guowangkeji.top

JS:   structuredClone(obj)
来源：http://ssl.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://rwk.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://oxh.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://stp.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tot.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kio.ybcxt.top

[K06] 解析 URL 查询串
来源：http://ebz.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kyj.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bap.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://liu.hcnkem.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xej.kuanghao11.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dhr.hywenlv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://pzs.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uru.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xai.bbcook.cn

[K07] 进制转换
来源：http://toh.wangdashe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://drq.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wnn.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uwv.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jfb.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xoo.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bqb.quarkkingdee.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dwv.jlsjyb.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kmg.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://uff.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://usx.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qlb.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://cmb.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://crf.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yip.yongpay.top

Go:   encoding/gob
来源：http://hbb.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://ljl.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qnq.yj20258.top

================================================================================
来源：http://guo.yuanzhike.top

L. 网络请求
来源：http://sor.aibaodan.cn

================================================================================
来源：http://aed.chenzaomai.com

[L01] 发送 GET 请求
来源：http://mqe.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gtz.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rfg.meibo888.top

JS:   await fetch(url)
来源：http://btb.ppjwa.cn

TS:   await fetch(url)
来源：http://nxj.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qts.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://kei.feifeiyinyue.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xxt.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oof.vehdjk.com

[L02] 发送 POST JSON
来源：http://ojb.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://eig.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qpk.jinqigufen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mks.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cfq.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tsm.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ujq.sjlbkw.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oqr.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pes.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://ojl.nwbrower.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nbz.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nah.9152youxi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gcy.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wza.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://twt.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ujh.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fas.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sym.birdmap.top

[L04] 设置超时
来源：http://hvv.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://ywe.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rpb.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yfk.yongpay.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vna.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ygq.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aiv.shuidangran.top


<!-- 参考信息 -->