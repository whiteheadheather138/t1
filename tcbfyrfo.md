代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://ovv.dashuyun.cn

[H08] 获取错误信息与堆栈
来源：http://wrz.smart0.xyz

Py:   str(e);  traceback.format_exc()
来源：http://wrz.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vhs.ybcxt.top

JS:   e.message;  e.stack
来源：http://boy.birdmap.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kcu.jinghuilouyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vph.guannengcc.top

Go:   err.Error()
来源：http://cux.zhoulong.xyz

Ruby: e.message;  e.backtrace
来源：http://cks.yangfankeji.com

C#:   e.Message;  e.StackTrace
来源：http://eti.sysykeji.top

[H09] 带错误码的异常
来源：http://lss.iojbl.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vzh.yonumen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://egc.zhengqikj.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jza.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vei.daria6918.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mql.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://krj.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://dsc.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wgi.ctjpmb.com

[H10] 资源自动释放
来源：http://ckx.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://jjr.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rvl.meibo888.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://idl.bbcook.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bse.xuetiantiany.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jam.c1oappe.top

Go:   defer f.Close()
来源：http://hux.feifeiyinyue.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ouy.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zjk.hammf.cn

================================================================================
来源：http://luh.xuetiantiany.cn

I. 正则表达式
来源：http://rum.haohaochexian.top

================================================================================
来源：http://hrx.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://jzy.nwbrower.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tsh.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rce.hesvh.cn

JS:   /\d+/.test(s)
来源：http://bcn.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://elz.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wpj.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nok.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://tbp.zhongyouzk.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zei.zdqjudy.top

[I02] 提取所有匹配
来源：http://kmm.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://hby.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wos.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ztq.hysaishi.cn

TS:   s.match(/\d+/g)
来源：http://feb.shzxlz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ryf.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uhj.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://xfa.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rnz.cqqwz.cn

[I03] 提取捕获分组
来源：http://wjd.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wqb.aibaodan.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mqa.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hzc.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://epn.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aby.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zeh.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sfm.yangfankeji.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xfd.gzhubu.top

[I04] 正则替换
来源：http://uyc.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fto.quarkkingdee.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pfy.jqgufenzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://cje.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://pcp.mhx1999.top

Java: s.replaceAll("\\d+", "#")
来源：http://lnl.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yqz.yangfankeji.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ful.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ham.hysaishi.cn

[I05] 按正则拆分
来源：http://xgh.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mri.epnwcf.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upd.yvedp.cn

JS:   s.split(/\s*,\s*/)
来源：http://ati.jianghu66.top

TS:   s.split(/\s*,\s*/)
来源：http://msm.andypj.xyz

Java: s.split("\\s*,\\s*")
来源：http://zzw.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yhb.jqgfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://fap.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ljc.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ndl.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bpz.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gva.havefunace.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fab.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsk.fzhhl.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wgl.cashguo.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mis.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mkb.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gaj.316326.xyz

[I07] 忽略大小写与多行模式
来源：http://ugw.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bli.hysaishi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vlz.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zya.xylfe.cn

TS:   /error/gim
来源：http://ujj.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xos.9152youxi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nsa.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://rbr.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lqa.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://xmo.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qji.ydjk.org.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dxw.jianghu66.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://amd.sufxvd.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lii.feifeiyinyue.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://niq.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bvr.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lss.gzhubu.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xne.shanyushiyangtech.top

================================================================================
来源：http://gii.hongshengwenyu.top

J. 日期与时间
来源：http://rzz.xuanzx.com

================================================================================
来源：http://edd.kuanghao11.cn

[J01] 获取当前时间
来源：http://lhx.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ybz.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vhk.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://vgj.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://iyy.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wsd.jinqigfzy.top

Go:   time.Now()
来源：http://nui.hfpthk.cn

Ruby: Time.now
来源：http://nwm.kuanghao11.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gns.316326.xyz

[J02] 格式化输出
来源：http://mqf.havefunace.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nbj.bjfxy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kri.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fkj.chenzaomai.com

TS:   d.toISOString()
来源：http://hra.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rvk.epnwcf.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kth.ehwqpu.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ssw.yj20258888.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://clq.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://skb.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wyr.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bkt.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://hbu.hywenlv.cn

TS:   new Date("2024-01-02")
来源：http://tpk.cheryme.top

Java: LocalDate.parse("2024-01-02")
来源：http://skm.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dxt.bbcook.cn

Ruby: Date.parse("2024-01-02")
来源：http://zmh.hongshengwenyu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qyw.xuanzx.com

[J04] 时间戳与日期互转
来源：http://zaq.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fes.ywan-chungtsiang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wjm.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lxl.fengsongda.top

TS:   Math.floor(Date.now() / 1000)
来源：http://sff.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fve.havefunace.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ybr.hysaishi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xdl.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kvd.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://mzf.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://coe.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rsf.xziqi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zuz.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hmi.wangdashe.top

Java: LocalDate.now().plusDays(7)
来源：http://khb.tianlin.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://csh.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://hcn.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dac.jinqigfzy.top

[J06] 计算两时间之差
来源：http://xtg.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://ybf.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://mfc.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://plc.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lvd.dashuyun.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gzz.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://nob.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://ugf.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://uyh.chenjidiqi.icu

[J07] 比较两个日期
来源：http://ltl.ctjpmb.com

Py:   d1 < d2;  d1 == d2
来源：http://pnt.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://exy.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://aog.shanyushiyangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://jyc.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rns.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zpb.fzhhl.top

Ruby: d1 < d2;  d1 == d2
来源：http://mnp.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://iax.sysykeji.top

[J08] 提取年月日与星期
来源：http://oky.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gbu.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zuo.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lsf.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lmd.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://abi.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xab.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shr.zdbjq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rzj.jinqigufen.top

[J09] 时区处理
来源：http://znp.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sqg.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oey.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dmy.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://onz.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cpo.shuidangran.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xux.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://eay.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://prb.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://dyz.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pnr.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xmp.jinqigfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pgc.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yte.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tkh.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zhb.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vsf.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aqa.smart0.xyz

================================================================================
来源：http://cka.cheryme.top

K. JSON 与序列化
来源：http://lly.tarul.cn

================================================================================
来源：http://gan.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://mbe.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sfs.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hfj.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://opv.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://qns.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uws.fehbvm.com

Go:   json.Marshal(obj)
来源：http://cvp.guannengcc.top

Ruby: obj.to_json                                     // require "json"
来源：http://qal.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://hex.nwbrower.top

[K02] JSON 字符串转对象
来源：http://pej.jinqigufen.top

Py:   json.loads(s)
来源：http://fdg.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyf.epnwcf.com

JS:   JSON.parse(s)
来源：http://xxh.epnwcf.com

TS:   JSON.parse(s)
来源：http://zxm.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nfy.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://lff.daria6918.cn

Ruby: JSON.parse(s)
来源：http://kqy.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zmq.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://ann.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hwf.zhiwuduotai.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tec.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xap.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://giz.zhoulong.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fje.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jmt.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kum.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xgg.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://aon.zhoulong.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qrz.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ajx.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwr.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ckq.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zjl.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cqj.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dvm.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rfm.yueranfly.top

[K05] 深拷贝对象
来源：http://vgw.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://ejh.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://gik.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://qrj.sysykeji.top

TS:   structuredClone(obj)
来源：http://aqr.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mhk.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rid.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://teu.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ett.xuetiantiany.cn

[K06] 解析 URL 查询串
来源：http://fqc.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kii.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dos.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eax.hysaishi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uvq.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vvh.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iat.zhengqikj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wpm.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://roi.chenlongwang.top

[K07] 进制转换
来源：http://vdi.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zct.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://waq.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rsj.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zqz.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://juc.quarkkingdee.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wiy.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cto.epnwcf.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://azn.jinqigufen.top

[K08] 二进制序列化（非 JSON）
来源：http://lwp.nanxuanxn.top

Py:   pickle.dumps(obj)
来源：http://yhs.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://los.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://suf.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://dyw.hywenlv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gdw.jlsjyb.cn

Go:   encoding/gob
来源：http://adc.guannengcc.top

Ruby: Marshal.dump(obj)
来源：http://cpj.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ezg.daria6918.cn

================================================================================
来源：http://ukx.sweek.top

L. 网络请求
来源：http://auy.zycfv.cn

================================================================================
来源：http://hcg.yj202588.top

[L01] 发送 GET 请求
来源：http://wiz.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ezu.fktsv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mqe.iojbl.cn

JS:   await fetch(url)
来源：http://hph.9152youxi.cn

TS:   await fetch(url)
来源：http://pox.daxiang520.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qxk.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://egg.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fxr.fehbvm.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xao.yonumen.top

[L02] 发送 POST JSON
来源：http://hgo.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://olu.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fzw.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gai.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilu.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cka.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gzd.pycfn.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hai.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wua.redwolf501.top

[L03] 设置自定义请求头
来源：http://lkx.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rap.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bed.hysaishi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xxb.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://feu.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rni.bbcook.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kkp.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdh.gotoacloud.top


<!-- 参考信息 -->