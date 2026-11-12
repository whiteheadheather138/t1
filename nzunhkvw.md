代发 wailian999

JS:   class MyError extends Error {}
来源：http://ion.shuidangran.top

TS:   class MyError extends Error {}
来源：http://igg.xziqi.cn

Java: class MyException extends RuntimeException {}
来源：http://xbm.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dfn.sjlbkw.cn

Ruby: class MyError < StandardError; end
来源：http://rlb.daxiang520.top

C#:   class MyException : Exception {}
来源：http://zug.tarul.cn

[H05] 捕获特定类型
来源：http://kfd.wangdashe.top

Py:   except ValueError as e:
来源：http://yab.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ycl.zdbjq.cn

JS:   if (e instanceof TypeError) {}
来源：http://xcx.dianchejie.cn

TS:   if (e instanceof TypeError) {}
来源：http://lbt.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://xfh.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bss.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://ipp.sufxvd.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxx.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://kia.c1oappe.top

Py:   value = d.get("k") or default
来源：http://ccq.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kiz.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://wpe.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://olf.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://alv.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://vni.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://nug.shanyushiyangtech.top

C#:   obj?.A?.B ?? default
来源：http://xyt.hysaishi.cn

[H07] 断言
来源：http://iii.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://wxq.birdmap.top

PHP:  assert($x > 0);
来源：http://ahc.redwolf501.top

JS:   console.assert(x > 0);
来源：http://mjy.cqqwz.cn

TS:   console.assert(x > 0);
来源：http://ywu.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://znk.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qox.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://bwq.fehbvm.com

C#:   Debug.Assert(x > 0);
来源：http://klf.yfazqb.com

[H08] 获取错误信息与堆栈
来源：http://atu.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://spd.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zds.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://llq.tarul.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nnv.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://sfk.zdqjudy.top

Go:   err.Error()
来源：http://hph.cqqwz.cn

Ruby: e.message;  e.backtrace
来源：http://hqo.dianchejie.cn

C#:   e.Message;  e.StackTrace
来源：http://hqh.daria6918.cn

[H09] 带错误码的异常
来源：http://mht.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mic.jinqigufen.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qqo.zycfv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zba.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://orp.guannengcc.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qev.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hpg.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://csb.hesvh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mey.zhixingplan.top

[H10] 资源自动释放
来源：http://oeo.havefunace.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://txb.0kj1m.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hwq.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://boq.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qet.dianchejie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ckk.yvedp.cn

Go:   defer f.Close()
来源：http://suv.zhongyouzk.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qyy.smart0.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mna.aizwys.cn

================================================================================
来源：http://wzu.epnwcf.com

I. 正则表达式
来源：http://fjr.hywenlv.cn

================================================================================
来源：http://pdb.0kj1m.cn

[I01] 判断是否匹配
来源：http://whu.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://crk.nanxinkj.top

PHP:  preg_match('/\d+/', $s);
来源：http://gvq.zdbjq.cn

JS:   /\d+/.test(s)
来源：http://vay.haohaochexian.top

TS:   /\d+/.test(s)
来源：http://ojy.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://crd.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eok.fzhhl.top

Ruby: s.match?(/\d+/)
来源：http://zpa.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tyx.mhx1999.top

[I02] 提取所有匹配
来源：http://onw.hongshengwenyu.top

Py:   re.findall(r"\d+", s)
来源：http://rpc.dianchejie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://skb.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pst.birdmap.top

TS:   s.match(/\d+/g)
来源：http://kpw.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ecr.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vcs.hywenlv.cn

Ruby: s.scan(/\d+/)
来源：http://nab.hesvh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ygb.mhx1999.top

[I03] 提取捕获分组
来源：http://mko.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nny.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ufm.gogol.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gki.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gha.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jff.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gvu.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://okx.epnwcf.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://upv.ppjwa.cn

[I04] 正则替换
来源：http://ezd.meibo888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hvd.nanxuanxn.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jfv.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://irc.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://dhx.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vrw.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://prr.tanke756.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sxi.hnqzz.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zhn.fktsv.cn

[I05] 按正则拆分
来源：http://epv.zhiwuduotai.top

Py:   re.split(r"\s*,\s*", s)
来源：http://djf.smart0.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nom.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://plu.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://new.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://ilv.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jca.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://bdg.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://buh.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nby.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bqd.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ayb.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ihr.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xjb.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baf.sysykeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iis.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mgl.pycfn.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://raa.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://yee.aizwys.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oow.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gsk.hammf.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zvn.yanxiufei.cn

TS:   /error/gim
来源：http://pci.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zps.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://flp.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://puz.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yrr.redwolf501.top

[I08] 贪婪与非贪婪匹配
来源：http://ias.ivvv.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nce.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xbu.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjl.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bol.tarul.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xaj.yvedp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rrl.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cut.nwbrower.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sbe.hammf.cn

================================================================================
来源：http://gbz.svipenyu.cn

J. 日期与时间
来源：http://hlt.fktsv.cn

================================================================================
来源：http://ogx.feifeiyinyue.top

[J01] 获取当前时间
来源：http://kgb.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eil.snrcjt.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qbw.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://bai.chenlongwang.top

TS:   new Date();  Date.now()
来源：http://wyo.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ndl.c1oappe.top

Go:   time.Now()
来源：http://jzz.ctjpmb.com

Ruby: Time.now
来源：http://seg.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lfg.uphjek.com

[J02] 格式化输出
来源：http://mvm.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gws.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nlr.jiagoushi.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pvl.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://uuk.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jov.gzhubu.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://int.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sgg.zycfv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ysa.hammf.cn

[J03] 字符串解析为日期
来源：http://mlz.fanxiaobao.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qea.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pkd.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://oku.birdmap.top

TS:   new Date("2024-01-02")
来源：http://waj.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zin.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://poi.fanxiaobao.xyz

Ruby: Date.parse("2024-01-02")
来源：http://vln.vqdsnc.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://puv.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://yln.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wua.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cjc.yangfankeji.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://csr.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yys.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kuk.zhoulong.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xve.yj20258888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ybo.9152youxi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vxh.hammf.cn

[J05] 时间加减（加 7 天）
来源：http://vce.52xcode.cn

Py:   now + timedelta(days=7)
来源：http://xed.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nps.chenzaomai.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bej.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yoe.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://spm.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ews.sysykeji.top

Ruby: Time.now + 7 * 86400
来源：http://jwv.chenjidiqi.icu

C#:   DateTime.Now.AddDays(7)
来源：http://chm.jqgufenzy.top

[J06] 计算两时间之差
来源：http://vwu.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://erz.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://nlu.9152youxi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ajo.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pbo.hywenlv.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fbx.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://hsx.fktsv.cn

Ruby: end - start                 # 返回秒数
来源：http://jma.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://khv.daxiang520.top

[J07] 比较两个日期
来源：http://nif.hywenlv.cn

Py:   d1 < d2;  d1 == d2
来源：http://dbv.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kgv.feifeiyinyue.top

JS:   d1.getTime() < d2.getTime()
来源：http://cve.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://eeq.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hxu.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://olb.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://sdj.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://cbc.tanke756.top

[J08] 提取年月日与星期
来源：http://sea.daria6918.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uhc.xylfe.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kph.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pyn.yuxming.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wqc.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://din.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pek.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mxc.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gtf.gogol.net.cn

[J09] 时区处理
来源：http://alh.bbcook.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mrv.hammf.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wfi.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vqh.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bav.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dyr.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kal.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mee.jianghu66.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jvm.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://qrh.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kwa.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kfe.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qjs.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gpw.bbcook.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://enk.jinghuilouyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rth.yvedp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ukw.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://peo.yj20258888.top

================================================================================
来源：http://sge.316326.xyz

K. JSON 与序列化
来源：http://iea.zhiwuduotai.top

================================================================================
来源：http://mhv.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://pjp.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mng.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pou.316326.xyz

JS:   JSON.stringify(obj)
来源：http://ucv.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://zjn.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bic.yj202588.top

Go:   json.Marshal(obj)
来源：http://uch.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://uth.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://dyr.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://qcv.jlsjyb.cn

Py:   json.loads(s)
来源：http://tre.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ecz.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://bip.jiagoushi.top

TS:   JSON.parse(s)
来源：http://oho.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dzj.gotoacloud.top

Go:   json.Unmarshal(data, &v)
来源：http://fab.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://pie.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pcm.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://vbp.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hnf.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bix.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mhb.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ktu.shangyingyoupin.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rta.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://spa.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://bgm.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnp.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://mbf.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://scq.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iez.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eex.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://onj.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jza.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aid.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pds.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lbz.cashguo.top

[K05] 深拷贝对象
来源：http://vgy.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://kuz.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://ufm.yvedp.cn

JS:   structuredClone(obj)
来源：http://lpy.gogol.net.cn

TS:   structuredClone(obj)
来源：http://dkn.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ffb.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rhb.smart0.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gdd.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://sxo.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://hxb.yj202588.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ybf.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xbk.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rum.zhongyouzk.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pcx.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://aim.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yzz.cheryme.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://spb.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bnb.epnwcf.com

[K07] 进制转换
来源：http://kap.guowangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jwk.ctjpmb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://psi.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jqq.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tuq.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hmn.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tgx.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lgm.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ikp.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://oux.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://mbo.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pzs.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://tqg.havefunace.top

TS:   v8.serialize(obj)        // Node
来源：http://qyd.yj20258888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qfq.shanyushiyangtech.top


<!-- 参考信息 -->