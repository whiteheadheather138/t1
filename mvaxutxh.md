代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://dia.hcnkem.com

C#:   e.Message;  e.StackTrace
来源：http://cdg.hcnkem.com

[H09] 带错误码的异常
来源：http://gwb.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://klj.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://srr.hnxiangtu.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jgd.xziqi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tbl.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qmo.svipenyu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lbt.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vlj.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://asw.pengpengdd.cyou

[H10] 资源自动释放
来源：http://jkw.guowangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://usz.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lhn.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://elq.jiagoushi.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jzl.zhoulong.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ego.nwbrower.top

Go:   defer f.Close()
来源：http://igq.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eqg.yj20258.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ldd.52xcode.cn

================================================================================
来源：http://ktt.sysykeji.top

I. 正则表达式
来源：http://wzg.tarul.cn

================================================================================
来源：http://pmw.hfpthk.cn

[I01] 判断是否匹配
来源：http://lsy.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hqx.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://snr.meibo888.top

JS:   /\d+/.test(s)
来源：http://fml.c1oappe.top

TS:   /\d+/.test(s)
来源：http://yxv.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dnc.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bfj.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://qgt.zhijiandao.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rtv.52xcode.cn

[I02] 提取所有匹配
来源：http://tch.nwbrower.top

Py:   re.findall(r"\d+", s)
来源：http://rbq.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mme.uphjek.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wzj.daxiang520.top

TS:   s.match(/\d+/g)
来源：http://uhd.nanxuanxn.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xxv.zhoulong.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ngj.ctjpmb.com

Ruby: s.scan(/\d+/)
来源：http://cvi.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kzm.wangdashe.top

[I03] 提取捕获分组
来源：http://tzw.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ivv.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eed.hfpthk.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ugw.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ayq.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tla.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qkm.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yta.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kps.redwolf501.top

[I04] 正则替换
来源：http://mfa.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://kok.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tdi.smart0.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://akg.hywenlv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ton.yanxiufei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cku.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jal.sufxvd.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mbw.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fsu.yuanzhike.top

[I05] 按正则拆分
来源：http://qbt.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bve.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fke.daria6918.cn

JS:   s.split(/\s*,\s*/)
来源：http://mxa.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://hvv.zhiwuduotai.top

Java: s.split("\\s*,\\s*")
来源：http://mgk.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zsq.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://vcm.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dlf.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nxr.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nco.yongpay.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mxi.zhoulong.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tsn.yj20258.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zyu.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mim.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jfs.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mcc.haohaochexian.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bmn.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://lcl.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xve.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ezs.cucudq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bkn.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://epp.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eff.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wbw.sweek.top

Ruby: s.scan(/error/i)
来源：http://cnc.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mph.jinqigfzy.top

[I08] 贪婪与非贪婪匹配
来源：http://mbi.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lzs.shangyingyoupin.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qlu.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://acw.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gpn.mhx1999.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tch.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hoe.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ghu.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jvt.cdnleiting.top

================================================================================
来源：http://mbz.hcnkem.com

J. 日期与时间
来源：http://onm.jqgufenzy.top

================================================================================
来源：http://fqz.fehbvm.com

[J01] 获取当前时间
来源：http://tjd.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ozs.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gnq.yuxming.cn

JS:   new Date();  Date.now()
来源：http://prt.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://rvq.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://kpm.ybcxt.top

Go:   time.Now()
来源：http://waq.smart0.xyz

Ruby: Time.now
来源：http://kfp.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nly.redwolf501.top

[J02] 格式化输出
来源：http://rqe.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mjf.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nqs.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ygi.yonumen.top

TS:   d.toISOString()
来源：http://uht.xingfuxueyuan.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vha.jinqigfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zvd.zhiwuduotai.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zng.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ffg.0kj1m.cn

[J03] 字符串解析为日期
来源：http://beh.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pgw.yvedp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nnl.zhengqikj.top

JS:   new Date("2024-01-02")
来源：http://zrl.wangdashe.top

TS:   new Date("2024-01-02")
来源：http://gup.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://bjc.hnqzz.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mvt.iojbl.cn

Ruby: Date.parse("2024-01-02")
来源：http://gfp.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qvq.tarul.cn

[J04] 时间戳与日期互转
来源：http://bqu.sufxvd.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://uno.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://his.sweek.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bwm.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://brj.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hmw.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ayp.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ths.svipenyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cof.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://jzp.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://xvl.zhiwuduotai.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dww.fanxiaobao.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ttz.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://prc.shuidangran.top

Java: LocalDate.now().plusDays(7)
来源：http://sno.cheryme.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bji.zhixingplan.top

Ruby: Time.now + 7 * 86400
来源：http://abr.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xfb.havefunace.top

[J06] 计算两时间之差
来源：http://cvg.ydzc1.top

Py:   (end - start).total_seconds()
来源：http://dks.xingfuxueyuan.xyz

PHP:  $end->diff($start)->days;
来源：http://kti.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mzo.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://iig.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://zyx.jyoumei.cn

Go:   end.Sub(start).Hours()
来源：http://xwa.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://oqz.quarkkingdee.top

C#:   (end - start).TotalSeconds
来源：http://sme.meibo888.top

[J07] 比较两个日期
来源：http://zej.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://snm.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nod.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://bkh.9152youxi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nxc.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vcv.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wku.xuetiantiany.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hky.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://mae.wangshuangyany.cn

[J08] 提取年月日与星期
来源：http://qly.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://chd.jyoumei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://brv.hongshengwenyu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iat.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gei.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kxe.svipenyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://doa.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dpg.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gkd.zdbjq.cn

[J09] 时区处理
来源：http://rsf.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://paf.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jfc.fktsv.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kjh.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nlu.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qia.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uin.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jtc.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fcw.zhongyouzk.top

[J10] 取今天 / 本月第一天
来源：http://raj.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wkl.fzhhl.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dxv.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pxm.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tpc.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lek.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mfn.shuidangran.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kzz.316326.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://peg.chenzaomai.com

================================================================================
来源：http://rwj.yuxming.cn

K. JSON 与序列化
来源：http://fja.gzhubu.top

================================================================================
来源：http://xgm.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://mok.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://aar.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wia.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://itn.sweek.top

TS:   JSON.stringify(obj)
来源：http://lom.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ihq.wangshuangyany.cn

Go:   json.Marshal(obj)
来源：http://txq.jinqigfzy.top

Ruby: obj.to_json                                     // require "json"
来源：http://hsi.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ige.gzhubu.top

[K02] JSON 字符串转对象
来源：http://krs.zhoulong.xyz

Py:   json.loads(s)
来源：http://sbo.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzk.sxryk.cn

JS:   JSON.parse(s)
来源：http://yft.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://uah.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qdx.yj202588.top

Go:   json.Unmarshal(data, &v)
来源：http://hvg.cheryme.top

Ruby: JSON.parse(s)
来源：http://pxe.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gne.0kj1m.cn

[K03] JSON 美化输出（带缩进）
来源：http://ngl.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iwf.shangyingyoupin.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cyv.cheryme.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pir.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wug.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ple.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rum.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://skm.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://clw.sysykeji.top

[K04] 读取 JSON 文件
来源：http://sti.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hih.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bxf.jinghuilouyu.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ggp.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yuf.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sdy.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vwj.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nyg.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dfv.iojbl.cn

[K05] 深拷贝对象
来源：http://ocv.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://sey.daria6918.cn

PHP:  unserialize(serialize($obj));
来源：http://qrc.tian-w.cn

JS:   structuredClone(obj)
来源：http://ajh.cucudq.cn

TS:   structuredClone(obj)
来源：http://urf.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zig.shuidangran.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kmw.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rig.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://qhf.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://kcb.vehdjk.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsi.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nyc.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xak.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gxc.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pcs.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iwb.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqo.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pwk.jiagoushi.top

[K07] 进制转换
来源：http://ame.kuanghao11.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wrk.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qjq.ywan-chungtsiang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vip.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vnj.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zmp.meibo888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uzp.yj20258.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bxf.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lfm.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://ajx.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://eze.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vlj.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://dih.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://npl.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://izg.hesvh.cn

Go:   encoding/gob
来源：http://zfy.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://jyy.cdnleiting.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zne.gaohongyu789.top

================================================================================
来源：http://ifh.0kj1m.cn

L. 网络请求
来源：http://jgi.zhengqikj.top

================================================================================
来源：http://ecm.zycfv.cn

[L01] 发送 GET 请求
来源：http://gby.sufxvd.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gxe.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zrp.pengpengdd.cyou

JS:   await fetch(url)
来源：http://noh.xuetiantiany.cn

TS:   await fetch(url)
来源：http://fds.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dfd.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://hvr.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://itu.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ygm.ydzc1.top

[L02] 发送 POST JSON
来源：http://tbw.uphjek.com

Py:   requests.post(url, json={"a": 1})
来源：http://ejp.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://phw.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://edk.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xbp.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kip.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ifk.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mto.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wru.sweek.top

[L03] 设置自定义请求头
来源：http://bhz.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qyq.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cnj.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rta.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kta.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cdo.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gxg.sjlbkw.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mss.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fsf.fzhhl.top

[L04] 设置超时
来源：http://wxo.yanxiufei.cn

Py:   requests.get(url, timeout=5)
来源：http://ujs.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kdz.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pqn.bbcook.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uua.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bno.tianlin.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osw.zhoulong.xyz


<!-- 参考信息 -->