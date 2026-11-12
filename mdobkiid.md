代发 wailian999

[H07] 断言
来源：http://tjq.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://qdp.xuetiantiany.cn

PHP:  assert($x > 0);
来源：http://yyn.epnwcf.com

JS:   console.assert(x > 0);
来源：http://fsd.cashguo.top

TS:   console.assert(x > 0);
来源：http://opc.uphjek.com

Java: assert x > 0 : "必须为正";
来源：http://fjq.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://res.gogol.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lnn.dashuyun.cn

C#:   Debug.Assert(x > 0);
来源：http://urb.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://xyi.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://kiw.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://obl.ywan-chungtsiang.top

JS:   e.message;  e.stack
来源：http://xvd.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ymz.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wmw.ctjpmb.com

Go:   err.Error()
来源：http://ynt.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://gvm.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://iqh.ehwqpu.com

[H09] 带错误码的异常
来源：http://xkt.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nsc.xylfe.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://osk.aizwys.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eav.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lor.shangyingyoupin.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://inz.ydjk.org.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://twk.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://hmz.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://gzt.jianghu66.top

[H10] 资源自动释放
来源：http://dly.yongpay.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://vmh.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zwn.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://idg.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ziv.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://adb.zhiwuduotai.top

Go:   defer f.Close()
来源：http://eox.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xgy.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://khi.bjfxy.top

================================================================================
来源：http://xop.zhongyouzk.top

I. 正则表达式
来源：http://ltn.birdmap.top

================================================================================
来源：http://upn.yongpay.top

[I01] 判断是否匹配
来源：http://rzb.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mrc.meibo888.top

PHP:  preg_match('/\d+/', $s);
来源：http://uzu.nanxinkj.top

JS:   /\d+/.test(s)
来源：http://wsl.havefunace.top

TS:   /\d+/.test(s)
来源：http://lfz.yuanzhike.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yuw.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kor.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://woo.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zwz.hcnkem.com

[I02] 提取所有匹配
来源：http://cii.havefunace.top

Py:   re.findall(r"\d+", s)
来源：http://uye.pycfn.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xrs.gotoacloud.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uzy.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://qgh.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jby.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cbs.gaohongyu789.top

Ruby: s.scan(/\d+/)
来源：http://uhn.zhongyouzk.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jzh.yuxming.cn

[I03] 提取捕获分组
来源：http://csh.chenjidiqi.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zxl.c1oappe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qxh.fanxiaobao.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dau.ppjwa.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zkk.guannengcc.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://deh.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nfn.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ebk.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ibq.jlsjyb.cn

[I04] 正则替换
来源：http://dyw.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://gvk.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://irg.sufxvd.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ily.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xou.svipenyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fwz.yueranfly.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yse.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ook.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ubx.yongpay.top

[I05] 按正则拆分
来源：http://cuy.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://rrp.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bst.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://kgw.tanke756.top

TS:   s.split(/\s*,\s*/)
来源：http://vkf.xinyue.icu

Java: s.split("\\s*,\\s*")
来源：http://bpv.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ycf.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://igd.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fek.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ylb.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ypt.tianlin.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dng.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://krz.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tag.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bcb.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xap.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lib.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ocz.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://nsn.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lcj.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dkd.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tth.jiagoushi.top

TS:   /error/gim
来源：http://hbg.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mmz.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ltn.jlsjyb.cn

Ruby: s.scan(/error/i)
来源：http://zei.zhoulong.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ieb.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://lxe.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fmr.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pqa.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ldj.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ujt.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://jmq.hnxiangtu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lms.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wnc.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zrr.yj20258888.top

================================================================================
来源：http://jvy.hammf.cn

J. 日期与时间
来源：http://zql.zhixingplan.top

================================================================================
来源：http://rci.0kj1m.cn

[J01] 获取当前时间
来源：http://ana.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://tey.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ylg.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://pui.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://lqn.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jhx.sjlbkw.cn

Go:   time.Now()
来源：http://bne.hcnkem.com

Ruby: Time.now
来源：http://dpc.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wvw.hnqzz.top

[J02] 格式化输出
来源：http://nmq.316326.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ggh.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tau.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nxp.jiagoushi.top

TS:   d.toISOString()
来源：http://bsb.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gex.daxiang520.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ysy.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ebs.yanxiufei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwy.cqqwz.cn

[J03] 字符串解析为日期
来源：http://xjm.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ota.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://plr.ctjpmb.com

JS:   new Date("2024-01-02")
来源：http://nlq.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://bxn.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://nqy.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebk.hongshengwenyu.top

Ruby: Date.parse("2024-01-02")
来源：http://qfz.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dyb.yj20258888.top

[J04] 时间戳与日期互转
来源：http://jjw.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gkb.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lbo.sxryk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lzp.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fct.vqdsnc.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kwc.wangdashe.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xmg.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jht.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fcu.zhijiandao.cn

[J05] 时间加减（加 7 天）
来源：http://ecy.gotoacloud.top

Py:   now + timedelta(days=7)
来源：http://eaa.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dff.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqj.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jtl.fanxiaobao.xyz

Java: LocalDate.now().plusDays(7)
来源：http://aau.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ndc.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://nnu.ctjpmb.com

C#:   DateTime.Now.AddDays(7)
来源：http://asm.haohaochexian.top

[J06] 计算两时间之差
来源：http://qip.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://dvl.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://gwy.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uzb.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dko.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jmp.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://ndx.tanke756.top

Ruby: end - start                 # 返回秒数
来源：http://ktq.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://mmp.bjfxy.top

[J07] 比较两个日期
来源：http://yld.gotoacloud.top

Py:   d1 < d2;  d1 == d2
来源：http://ahg.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kxg.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://ftz.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nun.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://elf.ivvv.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://esa.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pjl.sufxvd.cn

C#:   d1 < d2;  d1 == d2
来源：http://mav.shangyingyoupin.top

[J08] 提取年月日与星期
来源：http://qwo.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fxd.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bgf.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uwa.epnwcf.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rbk.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eup.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ucv.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mos.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pnl.vqdsnc.cn

[J09] 时区处理
来源：http://eux.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sbv.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bqf.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tiu.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ifi.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xsf.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ago.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hqs.havefunace.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://scw.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://wid.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://usq.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fxx.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yyz.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://nmh.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pnz.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iik.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://own.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://owv.birdmap.top

================================================================================
来源：http://fjd.kuanghao11.cn

K. JSON 与序列化
来源：http://pnp.zhiwuduotai.top

================================================================================
来源：http://hwz.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://ikw.iojbl.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://joz.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sfo.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://mra.tianlin.xyz

TS:   JSON.stringify(obj)
来源：http://mhs.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qpy.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://pzt.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://etb.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hgd.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://ata.ydzc1.top

Py:   json.loads(s)
来源：http://saa.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qur.fktsv.cn

JS:   JSON.parse(s)
来源：http://sym.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://fvh.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://flt.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://zig.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://sbx.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uvb.cucudq.cn

[K03] JSON 美化输出（带缩进）
来源：http://oou.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vps.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ett.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hyj.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gpr.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rar.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fue.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mrk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yqq.vehdjk.com

[K04] 读取 JSON 文件
来源：http://kqj.gaohongyu789.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rtw.yfazqb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ogo.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pnx.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://plk.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wlp.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lej.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://dfa.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aga.daxiang520.top

[K05] 深拷贝对象
来源：http://izx.hfpthk.cn

Py:   copy.deepcopy(obj)
来源：http://mnl.hysaishi.cn

PHP:  unserialize(serialize($obj));
来源：http://cto.wangdashe.top

JS:   structuredClone(obj)
来源：http://ewa.iojbl.cn

TS:   structuredClone(obj)
来源：http://tkp.shuidangran.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bhn.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xbx.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ebq.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mvb.jinghuilouyu.cn

[K06] 解析 URL 查询串
来源：http://ymz.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://znf.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vlz.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jtl.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://afp.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rzf.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dck.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qcm.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qeh.zdqjudy.top

[K07] 进制转换
来源：http://qhd.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ciw.hysaishi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qpu.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://add.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://che.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ejf.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xjq.yuxming.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bkk.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hpn.ydzc1.top

[K08] 二进制序列化（非 JSON）
来源：http://kij.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://jfz.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://rgy.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://fbq.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://czs.sysykeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nzc.316326.xyz

Go:   encoding/gob
来源：http://xxe.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://iho.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ovr.fzhhl.top

================================================================================
来源：http://hfi.vehdjk.com

L. 网络请求
来源：http://gdz.xylfe.cn

================================================================================
来源：http://onv.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://lvt.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://otw.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uak.jqgfzy.top

JS:   await fetch(url)
来源：http://nsv.yj20258888.top

TS:   await fetch(url)
来源：http://ztn.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bga.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://zzg.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wsa.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gcq.yuxming.cn

[L02] 发送 POST JSON
来源：http://art.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://xld.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rvv.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://szn.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qqa.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ifp.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zkn.cheryme.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bnf.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ooi.gogol.net.cn


<!-- 参考信息 -->