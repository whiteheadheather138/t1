代发 wailian999

TS:   console.assert(x > 0);
来源：http://kcx.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://gfa.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aqb.dianchejie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cwo.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://vek.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://juo.fengsongda.top

Py:   str(e);  traceback.format_exc()
来源：http://atv.cdnleiting.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fkj.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://qcd.wangdashe.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ltj.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aok.zycfv.cn

Go:   err.Error()
来源：http://lpf.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://xda.guowangkeji.top

C#:   e.Message;  e.StackTrace
来源：http://ulx.dashuyun.cn

[H09] 带错误码的异常
来源：http://ijd.pycfn.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nat.shzxlz.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://spv.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ira.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fsk.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://meh.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xif.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://npz.zhiwuduotai.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ksi.chenzaomai.com

[H10] 资源自动释放
来源：http://bqr.ppjwa.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gql.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rvf.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zgu.smart0.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cgk.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nzd.sweek.top

Go:   defer f.Close()
来源：http://hkp.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kzn.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jhq.redwolf501.top

================================================================================
来源：http://oer.nanxinkj.top

I. 正则表达式
来源：http://aam.gotoacloud.top

================================================================================
来源：http://fwm.jiagoushi.top

[I01] 判断是否匹配
来源：http://eut.yuanzhike.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://whl.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://onp.jianghu66.top

JS:   /\d+/.test(s)
来源：http://gch.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://adv.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vet.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://igk.hnxiangtu.top

Ruby: s.match?(/\d+/)
来源：http://plo.uphjek.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://snu.dashuyun.cn

[I02] 提取所有匹配
来源：http://col.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://gvh.hcnkem.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ugq.xuanzx.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tpn.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://ecs.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dmi.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kdp.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://iyn.jiagoushi.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zvj.jinyuanbaomall.cn

[I03] 提取捕获分组
来源：http://qka.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zjd.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wba.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rxm.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://afq.cashguo.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dqv.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vxj.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bsa.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lye.chenjidiqi.icu

[I04] 正则替换
来源：http://zfo.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pvf.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pet.ybcxt.top

JS:   s.replace(/\d+/g, "#")
来源：http://qye.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hfw.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://orf.jinqigufen.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ooe.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://jdp.zycfv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mwj.yongpay.top

[I05] 按正则拆分
来源：http://wcm.hywenlv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wqn.yj202588.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bbx.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://bqu.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://eih.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://wgk.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ebd.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://slv.hnqzz.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dxj.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gca.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nyq.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xgq.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axs.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://phz.meibo888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qbd.yueranfly.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lyf.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lvx.tarul.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xdw.chenzaomai.com

[I07] 忽略大小写与多行模式
来源：http://vud.c1oappe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ifb.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nsy.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mbe.hysaishi.cn

TS:   /error/gim
来源：http://lpu.bbcook.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oje.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xov.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://btx.yanxiufei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fsx.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://mbc.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iow.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://czp.jqgufenzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://orf.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uht.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pxl.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kcx.andypj.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cax.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dts.fktsv.cn

================================================================================
来源：http://fxf.haohaochexian.top

J. 日期与时间
来源：http://ska.zhoulong.xyz

================================================================================
来源：http://cro.cdnleiting.top

[J01] 获取当前时间
来源：http://cqz.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://fvl.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yfz.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://bzt.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://fqi.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://ref.smart0.xyz

Go:   time.Now()
来源：http://ssv.tianlin.xyz

Ruby: Time.now
来源：http://dxy.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uyv.dashuyun.cn

[J02] 格式化输出
来源：http://rqo.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zbl.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rpo.kuanghao11.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ctq.shanyushiyangtech.top

TS:   d.toISOString()
来源：http://hwu.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vce.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kcl.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jkx.fehbvm.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jgb.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://pgb.havefunace.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ily.fktsv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kdc.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://jty.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://rwq.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uls.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bes.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://dul.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bpp.yj20258.top

[J04] 时间戳与日期互转
来源：http://gmo.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qnt.xinyue.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://otn.ybcxt.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rpx.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cbk.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://msh.sysykeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dsb.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://txg.feifeiyinyue.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oel.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://wya.yanxiufei.cn

Py:   now + timedelta(days=7)
来源：http://fxc.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sas.yvedp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfm.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xxl.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://vmy.fktsv.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vqx.xylfe.cn

Ruby: Time.now + 7 * 86400
来源：http://ygm.tianlin.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://wce.haohaochexian.top

[J06] 计算两时间之差
来源：http://zqb.hcnkem.com

Py:   (end - start).total_seconds()
来源：http://jft.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://mbv.svipenyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tir.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fss.kuanghao11.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jfs.52xcode.cn

Go:   end.Sub(start).Hours()
来源：http://oih.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://oiu.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://qyq.birdmap.top

[J07] 比较两个日期
来源：http://ntj.aibaodan.cn

Py:   d1 < d2;  d1 == d2
来源：http://xcj.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hnz.gotoacloud.top

JS:   d1.getTime() < d2.getTime()
来源：http://mhm.yonumen.top

TS:   d1.getTime() < d2.getTime()
来源：http://qmy.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ewu.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://drr.zdbjq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qgp.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://zth.hnqzz.top

[J08] 提取年月日与星期
来源：http://hzn.daxiang520.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iid.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://efh.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oqq.svipenyu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mjh.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ank.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bje.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ing.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kxz.svipenyu.cn

[J09] 时区处理
来源：http://hqy.zdbjq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vyy.ybcxt.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yie.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://awj.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ngt.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lge.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dky.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dvm.0kj1m.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://onl.ctjpmb.com

[J10] 取今天 / 本月第一天
来源：http://qte.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ead.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xeq.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hnp.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mqt.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sct.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrj.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qpu.ctjpmb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unf.ivvv.top

================================================================================
来源：http://uxw.bbcook.cn

K. JSON 与序列化
来源：http://lhl.kuanghao11.cn

================================================================================
来源：http://wsm.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://gxq.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://stp.jiagoushi.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zvx.pycfn.com

JS:   JSON.stringify(obj)
来源：http://vrv.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://fni.0kj1m.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vyo.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://rei.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hhq.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pyx.zycfv.cn

[K02] JSON 字符串转对象
来源：http://hpj.yvedp.cn

Py:   json.loads(s)
来源：http://ako.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ntx.fehbvm.com

JS:   JSON.parse(s)
来源：http://hsd.aizwys.cn

TS:   JSON.parse(s)
来源：http://mjl.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mlh.daxiang520.top

Go:   json.Unmarshal(data, &v)
来源：http://xbh.ivvv.top

Ruby: JSON.parse(s)
来源：http://qid.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://phb.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://uoj.daria6918.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jac.c1oappe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ehz.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yzs.ydzc1.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kdg.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fxx.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://met.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://hwb.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jix.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://kvk.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mpz.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qxd.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oiz.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whi.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rba.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ynn.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ebn.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bks.vehdjk.com

[K05] 深拷贝对象
来源：http://yyo.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://usw.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://tpg.bbcook.cn

JS:   structuredClone(obj)
来源：http://clp.ivvv.top

TS:   structuredClone(obj)
来源：http://gtv.feifeiyinyue.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ybu.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vif.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kqb.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mxl.shuidangran.top

[K06] 解析 URL 查询串
来源：http://rsk.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://plj.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fwq.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nfk.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngj.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wsl.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fxg.gotoacloud.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://rlt.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bcn.gaohongyu789.top

[K07] 进制转换
来源：http://qps.xuanzx.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nnc.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ovv.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ftx.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jca.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dgx.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ibx.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://meb.yanxiufei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://you.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://cev.cashguo.top

Py:   pickle.dumps(obj)
来源：http://jbo.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://apj.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://ltl.cdnleiting.top

TS:   v8.serialize(obj)        // Node
来源：http://cck.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hta.shangyingyoupin.top

Go:   encoding/gob
来源：http://rcp.ywan-chungtsiang.top

Ruby: Marshal.dump(obj)
来源：http://mlf.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://csh.sufxvd.cn

================================================================================
来源：http://djc.tianlin.xyz

L. 网络请求
来源：http://oui.c1oappe.top

================================================================================
来源：http://dvn.mhx1999.top

[L01] 发送 GET 请求
来源：http://uvk.xziqi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vbq.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bqk.smart0.xyz

JS:   await fetch(url)
来源：http://mdj.hnqzz.top

TS:   await fetch(url)
来源：http://cbt.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jua.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://qah.xylfe.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fnp.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vav.yuxming.cn

[L02] 发送 POST JSON
来源：http://yxc.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vym.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://diw.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lcm.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mgo.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jou.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yoc.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jax.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ehc.ctjpmb.com

[L03] 设置自定义请求头
来源：http://lzm.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qlc.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cta.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://shb.cashguo.top


<!-- 参考信息 -->