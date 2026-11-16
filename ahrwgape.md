代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://dib.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://pky.chenzaomai.com

[H09] 带错误码的异常
来源：http://kng.chenjidiqi.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ops.yueranfly.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://msz.hammf.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ceg.hongshengwenyu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mzt.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rvp.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hqf.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://zyh.fehbvm.com

C#:   // 自定义异常类中加 Code 属性
来源：http://xif.aibaodan.cn

[H10] 资源自动释放
来源：http://ppn.tanke756.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hyk.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://liz.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hzs.fzhhl.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uks.vqdsnc.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gvw.fengsongda.top

Go:   defer f.Close()
来源：http://lgz.ybcxt.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iof.havefunace.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://muo.hysaishi.cn

================================================================================
来源：http://qtl.yangfankeji.com

I. 正则表达式
来源：http://wvg.jinqigufen.top

================================================================================
来源：http://cnk.hesvh.cn

[I01] 判断是否匹配
来源：http://emp.hnxiangtu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wzt.jianghu66.top

PHP:  preg_match('/\d+/', $s);
来源：http://zdy.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://xak.iojbl.cn

TS:   /\d+/.test(s)
来源：http://ird.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sxz.andypj.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ykw.fanxiaobao.xyz

Ruby: s.match?(/\d+/)
来源：http://vtw.shanyushiyangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://abk.tarul.cn

[I02] 提取所有匹配
来源：http://bwj.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://wny.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zjy.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://squ.hesvh.cn

TS:   s.match(/\d+/g)
来源：http://mvb.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zdf.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kks.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://gze.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mhj.nanxinkj.top

[I03] 提取捕获分组
来源：http://rsv.nwbrower.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fjb.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xzw.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://otw.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zhh.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mku.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tuk.bjfxy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oel.zhijiandao.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vgb.zhiwuduotai.top

[I04] 正则替换
来源：http://fwg.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://bef.jinqigufen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mcr.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://vtn.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ksr.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ahe.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pxj.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zfg.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xfe.smart0.xyz

[I05] 按正则拆分
来源：http://dtb.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wkj.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ylg.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://bhl.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://vvz.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://ooi.nanxinkj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eir.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://zsx.meibo888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kbe.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://acg.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bzr.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pac.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rir.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://caj.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://aqz.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://spm.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://czr.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xpc.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://bya.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://evs.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svv.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lbq.c1oappe.top

TS:   /error/gim
来源：http://jrt.xylfe.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://grj.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wrz.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://fpj.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cbw.haohaochexian.top

[I08] 贪婪与非贪婪匹配
来源：http://kwt.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gce.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://giq.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fzl.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wnv.tianlin.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://fbb.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jmo.yvedp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vuf.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wjs.haohaochexian.top

================================================================================
来源：http://xqa.xuetiantiany.cn

J. 日期与时间
来源：http://vdi.jqgufenzy.top

================================================================================
来源：http://rqs.aizwys.cn

[J01] 获取当前时间
来源：http://cyq.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pij.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vax.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://tns.c1oappe.top

TS:   new Date();  Date.now()
来源：http://uok.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://iul.shangyingyoupin.top

Go:   time.Now()
来源：http://zrk.cheryme.top

Ruby: Time.now
来源：http://vjm.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tof.uphjek.com

[J02] 格式化输出
来源：http://phw.sxryk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jdn.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iqt.fzhhl.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ypg.yueranfly.top

TS:   d.toISOString()
来源：http://ahh.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ued.wangdashe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gjm.jianghu66.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ime.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jva.pycfn.com

[J03] 字符串解析为日期
来源：http://ygv.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mlo.zhixingplan.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gaj.ivvv.top

JS:   new Date("2024-01-02")
来源：http://nzm.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://llr.mhx1999.top

Java: LocalDate.parse("2024-01-02")
来源：http://oqr.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mkt.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://yow.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xby.yonumen.top

[J04] 时间戳与日期互转
来源：http://hop.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xhw.snrcjt.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kpl.dianchejie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yud.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dus.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tgt.jiagoushi.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vub.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qsm.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xjv.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://fgq.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://unb.ehwqpu.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://eer.aibaodan.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hjr.ppjwa.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zft.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://wef.yj20258.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ecw.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://fwa.yuxming.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xor.dianchejie.cn

[J06] 计算两时间之差
来源：http://lgt.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://mfu.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://zzl.hcnkem.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kpt.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lky.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://hom.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://feg.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://aqh.tarul.cn

C#:   (end - start).TotalSeconds
来源：http://ncr.chenjidiqi.icu

[J07] 比较两个日期
来源：http://wnw.ydzc1.top

Py:   d1 < d2;  d1 == d2
来源：http://onc.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nak.andypj.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://rri.quarkkingdee.top

TS:   d1.getTime() < d2.getTime()
来源：http://izy.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sko.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vnv.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://ieg.tarul.cn

C#:   d1 < d2;  d1 == d2
来源：http://jjb.nanxuanxn.top

[J08] 提取年月日与星期
来源：http://aje.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qeo.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kxn.wangdashe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zpk.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fml.jinqigufen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pyh.xuanzx.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nyp.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aba.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ary.wangdashe.top

[J09] 时区处理
来源：http://fps.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eqo.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kqd.cqqwz.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iib.cdnleiting.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uyb.tianlin.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uvh.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gwa.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cri.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://elj.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://dwo.cdnleiting.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cog.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fmd.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hoc.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gri.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xot.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nrx.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vbl.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jzw.hcnkem.com

================================================================================
来源：http://tka.epnwcf.com

K. JSON 与序列化
来源：http://xgs.ctjpmb.com

================================================================================
来源：http://nxe.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://nma.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ahu.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rno.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://mix.tarul.cn

TS:   JSON.stringify(obj)
来源：http://zib.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dsk.ybcxt.top

Go:   json.Marshal(obj)
来源：http://hwa.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cvx.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://agd.xuanzx.com

[K02] JSON 字符串转对象
来源：http://tlt.ivvv.top

Py:   json.loads(s)
来源：http://cho.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://odp.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://eth.sysykeji.top

TS:   JSON.parse(s)
来源：http://txk.hcnkem.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://djz.yj20258888.top

Go:   json.Unmarshal(data, &v)
来源：http://dsp.ywan-chungtsiang.top

Ruby: JSON.parse(s)
来源：http://rqh.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iaa.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://kpv.epnwcf.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ksa.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qde.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ilh.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bnp.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://inc.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://chd.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ayg.andypj.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://drz.yvedp.cn

[K04] 读取 JSON 文件
来源：http://pcr.bjfxy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ytv.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tcy.yvedp.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rat.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jlr.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ibw.ivvv.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vvg.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lwq.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yan.jqgufenzy.top

[K05] 深拷贝对象
来源：http://kjc.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://deo.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://aed.hesvh.cn

JS:   structuredClone(obj)
来源：http://lmb.nanxinkj.top

TS:   structuredClone(obj)
来源：http://ygw.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jpz.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rlc.fengsongda.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://obq.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gex.daxiang520.top

[K06] 解析 URL 查询串
来源：http://jwa.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kxl.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kpx.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzo.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wbp.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fof.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://utz.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://axm.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eba.yj20258888.top

[K07] 进制转换
来源：http://sgj.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nmr.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ete.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tfj.iojbl.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mkz.vehdjk.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mzq.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aun.xingfuxueyuan.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://suo.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ned.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://bbc.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://oio.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://blx.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://xzt.shzxlz.cn

TS:   v8.serialize(obj)        // Node
来源：http://jya.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kee.xinyue.icu

Go:   encoding/gob
来源：http://zbl.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://lac.cqqwz.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://arn.vqdsnc.cn

================================================================================
来源：http://nlb.zhongyouzk.top

L. 网络请求
来源：http://foj.gotoacloud.top

================================================================================
来源：http://aou.meibo888.top

[L01] 发送 GET 请求
来源：http://sdq.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jsm.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sgh.zdbjq.cn

JS:   await fetch(url)
来源：http://chd.hfpthk.cn

TS:   await fetch(url)
来源：http://mdl.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qhc.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://hhf.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hoc.uphjek.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oau.xinyue.icu

[L02] 发送 POST JSON
来源：http://aap.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://mug.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hox.shuidangran.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fdy.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iuf.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://oib.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wuf.aizwys.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wuv.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhh.tian-w.cn

[L03] 设置自定义请求头
来源：http://dwj.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yjt.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zun.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zcv.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://buw.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vib.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nop.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wey.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dgz.ppjwa.cn

[L04] 设置超时
来源：http://lrf.meibo888.top

Py:   requests.get(url, timeout=5)
来源：http://bze.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zdy.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://atm.bjfxy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tir.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ezl.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cjh.52xcode.cn


<!-- 参考信息 -->