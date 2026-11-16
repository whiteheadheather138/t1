代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://swr.52xcode.cn

Ruby: rescue ArgumentError => e
来源：http://hyj.316326.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hyi.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://dyg.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://oco.birdmap.top

PHP:  $v = $d["k"] ?? null;
来源：http://bzx.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://knf.zhixingplan.top

TS:   obj?.a?.b;  d ?? default
来源：http://ckt.fktsv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wfd.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bjd.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://jqu.guowangkeji.top

C#:   obj?.A?.B ?? default
来源：http://uvl.yj202588.top

[H07] 断言
来源：http://tqr.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://yui.wangdashe.top

PHP:  assert($x > 0);
来源：http://ksv.smart0.xyz

JS:   console.assert(x > 0);
来源：http://wvy.hnqzz.top

TS:   console.assert(x > 0);
来源：http://oht.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://njo.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mjb.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://omj.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://fip.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://nes.zdbjq.cn

Py:   str(e);  traceback.format_exc()
来源：http://rct.gaohongyu789.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cmy.daxiang520.top

JS:   e.message;  e.stack
来源：http://rxx.hfpthk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vrn.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://uab.yanxiufei.cn

Go:   err.Error()
来源：http://wdi.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://jde.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://yyi.hnxiangtu.top

[H09] 带错误码的异常
来源：http://exq.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usc.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://nci.shzxlz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hwm.birdmap.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ryt.gotoacloud.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tzz.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pxa.vehdjk.com

Ruby: raise MyError.new("fail", 500)
来源：http://yrt.yongpay.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yzv.pengpengdd.cyou

[H10] 资源自动释放
来源：http://vyf.yuanzhike.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hhn.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xqf.birdmap.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xyc.zhixingplan.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ive.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xei.jqgfzy.top

Go:   defer f.Close()
来源：http://fkr.svipenyu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sbi.svipenyu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mbg.cdnleiting.top

================================================================================
来源：http://xzm.zhiwuduotai.top

I. 正则表达式
来源：http://mau.hesvh.cn

================================================================================
来源：http://hpo.sweek.top

[I01] 判断是否匹配
来源：http://rjk.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kwy.shanyushiyangtech.top

PHP:  preg_match('/\d+/', $s);
来源：http://uad.bjfxy.top

JS:   /\d+/.test(s)
来源：http://dah.cucudq.cn

TS:   /\d+/.test(s)
来源：http://hzr.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://drg.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eug.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://smi.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fhy.yonumen.top

[I02] 提取所有匹配
来源：http://dwi.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://xex.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cew.xylfe.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lpq.jinqigfzy.top

TS:   s.match(/\d+/g)
来源：http://zhh.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ybs.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zvc.zhengqikj.top

Ruby: s.scan(/\d+/)
来源：http://nns.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://upo.fktsv.cn

[I03] 提取捕获分组
来源：http://zyz.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vne.yj20258888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fmb.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wcq.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jwe.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pvm.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rwx.0kj1m.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://spu.shuidangran.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sbl.pycfn.com

[I04] 正则替换
来源：http://oco.yongpay.top

Py:   re.sub(r"\d+", "#", s)
来源：http://kri.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gwm.vehdjk.com

JS:   s.replace(/\d+/g, "#")
来源：http://ifg.shangyingyoupin.top

TS:   s.replace(/\d+/g, "#")
来源：http://fdp.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://goc.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mmv.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bxf.zhijiandao.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pro.yongpay.top

[I05] 按正则拆分
来源：http://xqj.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://zra.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yas.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://ocv.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://aek.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://mbs.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xif.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://pno.ydjk.org.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ajt.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxk.tarul.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ypf.aizwys.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yep.zhijiandao.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jdp.dianchejie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zao.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gdy.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pnx.pycfn.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pzh.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rdr.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://txh.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://luy.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bok.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pbj.chenlongwang.top

TS:   /error/gim
来源：http://xax.0kj1m.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mms.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wpw.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://uyk.yongpay.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://emr.0kj1m.cn

[I08] 贪婪与非贪婪匹配
来源：http://gdm.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mob.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://opc.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tyw.shanyushiyangtech.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://two.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://lbc.sjlbkw.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zto.ydjk.org.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fxn.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dqt.52xcode.cn

================================================================================
来源：http://qkr.hammf.cn

J. 日期与时间
来源：http://tzi.bjfxy.top

================================================================================
来源：http://nvs.daria6918.cn

[J01] 获取当前时间
来源：http://bos.zdqjudy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://veh.jqgfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vlr.pengpengdd.cyou

JS:   new Date();  Date.now()
来源：http://lvp.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://vxj.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zfr.pycfn.com

Go:   time.Now()
来源：http://ltj.hywenlv.cn

Ruby: Time.now
来源：http://lxh.52xcode.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bit.cdnleiting.top

[J02] 格式化输出
来源：http://tjm.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gyb.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kio.ydjk.org.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://drx.tian-w.cn

TS:   d.toISOString()
来源：http://yps.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cti.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qrp.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cly.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zus.yvedp.cn

[J03] 字符串解析为日期
来源：http://ajf.dashuyun.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hai.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ovn.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://zwu.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://gwi.hywenlv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dnc.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dxr.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://vcr.yj20258888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uel.zhengqikj.top

[J04] 时间戳与日期互转
来源：http://twc.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://euw.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dhc.gaohongyu789.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ngc.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xcd.iojbl.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ild.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mje.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wlk.quarkkingdee.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jal.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://iso.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://nzm.jinghuilouyu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oxk.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oii.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lar.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://dqu.fengsongda.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uin.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://cwg.hongshengwenyu.top

C#:   DateTime.Now.AddDays(7)
来源：http://evu.yj202588.top

[J06] 计算两时间之差
来源：http://svl.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://oil.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://ybo.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kgp.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hbd.yueranfly.top

Java: Duration.between(start, end).toSeconds()
来源：http://mfn.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://ooj.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://eou.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://tje.wangdashe.top

[J07] 比较两个日期
来源：http://pza.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://aoo.aibaodan.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kwd.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dxr.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://nnj.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qrf.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qmk.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ibo.pycfn.com

C#:   d1 < d2;  d1 == d2
来源：http://jkq.c1oappe.top

[J08] 提取年月日与星期
来源：http://bgk.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xid.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kmj.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dix.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cut.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qvz.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lyx.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ikd.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lkl.ivvv.top

[J09] 时区处理
来源：http://mrt.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kue.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cwl.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://knq.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbs.zhengqikj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dst.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gqi.zdqjudy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://omd.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://clp.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://sah.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://ett.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://iwd.dashuyun.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://noj.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ahl.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qtu.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vat.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qsf.kuanghao11.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eic.daria6918.cn

================================================================================
来源：http://yxy.yuxming.cn

K. JSON 与序列化
来源：http://luo.mhx1999.top

================================================================================
来源：http://onn.wangshuangyany.cn

[K01] 对象转 JSON 字符串
来源：http://drg.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fzl.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mri.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://yfk.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://crb.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kht.hcnkem.com

Go:   json.Marshal(obj)
来源：http://wnk.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gif.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rmv.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://jik.xingfuxueyuan.xyz

Py:   json.loads(s)
来源：http://llx.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ofy.yj20258888.top

JS:   JSON.parse(s)
来源：http://row.shzxlz.cn

TS:   JSON.parse(s)
来源：http://dqc.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wpe.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://mip.cucudq.cn

Ruby: JSON.parse(s)
来源：http://cmt.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jtm.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://qqk.ywan-chungtsiang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xpp.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://byc.9152youxi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://osc.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ory.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qce.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://okl.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://uqz.nanxinkj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vxz.zycfv.cn

[K04] 读取 JSON 文件
来源：http://hux.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sro.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ogp.redwolf501.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tun.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ouy.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ykj.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nfg.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zje.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmn.zdqjudy.top

[K05] 深拷贝对象
来源：http://qxa.uphjek.com

Py:   copy.deepcopy(obj)
来源：http://rcw.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://rdo.meibo888.top

JS:   structuredClone(obj)
来源：http://clk.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://hku.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zju.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://sbh.dashuyun.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zvp.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ahy.cucudq.cn

[K06] 解析 URL 查询串
来源：http://rev.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nxe.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yjq.yongpay.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pda.sxryk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ezy.chenzaomai.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ees.jinyuanbaomall.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mat.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://krl.tarul.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sgk.yongpay.top

[K07] 进制转换
来源：http://bfj.fanxiaobao.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sok.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pqu.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://alj.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ohb.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfo.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipm.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qdk.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xpe.hysaishi.cn

[K08] 二进制序列化（非 JSON）
来源：http://jnu.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://xah.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dyp.mhx1999.top

JS:   v8.serialize(obj)        // Node
来源：http://meb.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://svm.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gkv.yj20258888.top

Go:   encoding/gob
来源：http://wlv.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://tfq.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://thl.jinyuanbaomall.cn

================================================================================
来源：http://mbr.smart0.xyz

L. 网络请求
来源：http://fcd.gogol.net.cn

================================================================================
来源：http://mbr.guowangkeji.top

[L01] 发送 GET 请求
来源：http://bry.jyoumei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yxu.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://haa.hnqzz.top

JS:   await fetch(url)
来源：http://voq.jyoumei.cn

TS:   await fetch(url)
来源：http://ydu.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nwt.hcnkem.com


<!-- 参考信息 -->