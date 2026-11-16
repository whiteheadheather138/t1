代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://iki.shuidangran.top

C#:   class MyException : Exception {}
来源：http://cee.zdbjq.cn

[H05] 捕获特定类型
来源：http://ldy.hfpthk.cn

Py:   except ValueError as e:
来源：http://pkt.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://duc.iojbl.cn

JS:   if (e instanceof TypeError) {}
来源：http://yet.birdmap.top

TS:   if (e instanceof TypeError) {}
来源：http://zgi.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://wmq.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kqo.ydzc1.top

Ruby: rescue ArgumentError => e
来源：http://trh.epnwcf.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://saf.sysykeji.top

[H06] 可选值 / 空值安全访问
来源：http://clo.bjfxy.top

Py:   value = d.get("k") or default
来源：http://qcy.cdnleiting.top

PHP:  $v = $d["k"] ?? null;
来源：http://pga.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vdq.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xhx.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ckr.daxiang520.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qub.cdnleiting.top

Ruby: d&.dig(:a, :b)
来源：http://agl.yuanzhike.top

C#:   obj?.A?.B ?? default
来源：http://otw.nanxinkj.top

[H07] 断言
来源：http://hsm.shanyushiyangtech.top

Py:   assert x > 0, "必须为正"
来源：http://zvn.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://krw.shanyushiyangtech.top

JS:   console.assert(x > 0);
来源：http://xbw.tian-w.cn

TS:   console.assert(x > 0);
来源：http://cet.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://qjj.yueranfly.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfg.yfazqb.com

Ruby: raise "必须为正" unless x > 0
来源：http://plx.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://ixe.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://ylu.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://kyg.shangyingyoupin.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://voy.snrcjt.cn

JS:   e.message;  e.stack
来源：http://phv.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hux.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kms.birdmap.top

Go:   err.Error()
来源：http://zdr.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://cxx.hysaishi.cn

C#:   e.Message;  e.StackTrace
来源：http://zql.zycfv.cn

[H09] 带错误码的异常
来源：http://mkn.sjlbkw.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ign.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xqi.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pkj.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bxq.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hyp.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bbn.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xdq.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ruk.cheryme.top

[H10] 资源自动释放
来源：http://lmg.jianghu66.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://rea.c1oappe.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fgd.ydjk.org.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fte.jianghu66.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mau.haohaochexian.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wtx.hnqzz.top

Go:   defer f.Close()
来源：http://bjp.vehdjk.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lhm.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://unr.hfpthk.cn

================================================================================
来源：http://sho.yj202588.top

I. 正则表达式
来源：http://fqy.tarul.cn

================================================================================
来源：http://pcj.zhengqikj.top

[I01] 判断是否匹配
来源：http://kjm.sysykeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lnx.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://ieh.zycfv.cn

JS:   /\d+/.test(s)
来源：http://wan.fktsv.cn

TS:   /\d+/.test(s)
来源：http://hks.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://erh.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wae.cqqwz.cn

Ruby: s.match?(/\d+/)
来源：http://nso.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eya.zhongyouzk.top

[I02] 提取所有匹配
来源：http://rok.ydjk.org.cn

Py:   re.findall(r"\d+", s)
来源：http://pur.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pve.chenlongwang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wvg.nanxuanxn.top

TS:   s.match(/\d+/g)
来源：http://vot.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pvz.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mmj.jianghu66.top

Ruby: s.scan(/\d+/)
来源：http://ztz.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wdx.guannengcc.top

[I03] 提取捕获分组
来源：http://unr.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sln.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ezp.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mnt.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vif.ydzc1.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uuj.nwbrower.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dys.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yto.chenjidiqi.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eev.jinqigfzy.top

[I04] 正则替换
来源：http://mdi.zhengqikj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tza.shzxlz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wwp.shangyingyoupin.top

JS:   s.replace(/\d+/g, "#")
来源：http://xuo.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://pzc.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kjm.smart0.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://tfu.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dxn.andypj.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xlo.jqgfzy.top

[I05] 按正则拆分
来源：http://ecc.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iam.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hls.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://mjb.pycfn.com

TS:   s.split(/\s*,\s*/)
来源：http://ywy.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://ctl.9152youxi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lox.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://qlm.gzhubu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://eox.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bva.vehdjk.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zxi.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://poh.cqqwz.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uep.jlsjyb.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agj.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yhy.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jni.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zcy.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yds.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://zsk.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lqh.mhx1999.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wis.aizwys.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://slj.zhoulong.xyz

TS:   /error/gim
来源：http://ztl.dashuyun.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xwz.ybcxt.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nff.jianghu66.top

Ruby: s.scan(/error/i)
来源：http://ewy.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fjr.xinyue.icu

[I08] 贪婪与非贪婪匹配
来源：http://ruy.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://liw.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sjo.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lce.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://njy.nwbrower.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jed.fktsv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iuf.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zna.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zpm.cqqwz.cn

================================================================================
来源：http://lnt.chenlongwang.top

J. 日期与时间
来源：http://eky.ywan-chungtsiang.top

================================================================================
来源：http://thd.hywenlv.cn

[J01] 获取当前时间
来源：http://nop.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://zdf.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lay.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://ref.meibo888.top

TS:   new Date();  Date.now()
来源：http://sar.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uia.yj20258888.top

Go:   time.Now()
来源：http://yqy.ybcxt.top

Ruby: Time.now
来源：http://zpj.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fbl.hammf.cn

[J02] 格式化输出
来源：http://hvz.jlsjyb.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tls.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hfe.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dpz.shuidangran.top

TS:   d.toISOString()
来源：http://bbp.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ovo.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pru.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iwp.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mka.smart0.xyz

[J03] 字符串解析为日期
来源：http://nae.shanyushiyangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hlr.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lsv.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://etf.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://jgn.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://krj.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hci.andypj.xyz

Ruby: Date.parse("2024-01-02")
来源：http://nhb.chenjidiqi.icu

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sif.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://qgp.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pma.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wrc.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wkq.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://uri.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://paj.gogol.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ozw.zhiwuduotai.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kco.jyoumei.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lzz.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://uox.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://wkb.birdmap.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://smh.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zmk.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mof.bbcook.cn

Java: LocalDate.now().plusDays(7)
来源：http://ymw.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sba.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://inp.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://mug.sufxvd.cn

[J06] 计算两时间之差
来源：http://cot.hywenlv.cn

Py:   (end - start).total_seconds()
来源：http://gzm.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://ozr.zhongyouzk.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bqi.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jxk.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://owa.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://peg.shanyushiyangkeji.top

Ruby: end - start                 # 返回秒数
来源：http://xrg.yongpay.top

C#:   (end - start).TotalSeconds
来源：http://gmd.guowangkeji.top

[J07] 比较两个日期
来源：http://snb.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://tgk.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hvv.tarul.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gsm.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://gyl.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xbq.cucudq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uqp.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://vvm.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://qeo.vehdjk.com

[J08] 提取年月日与星期
来源：http://dhr.shangyingyoupin.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aiu.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://smw.gogol.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://inp.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rte.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sad.snrcjt.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rjk.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://atg.wangshuangyany.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lto.jqgfzy.top

[J09] 时区处理
来源：http://ofs.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://amz.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://anr.sjlbkw.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://txg.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uqq.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jpn.ywan-chungtsiang.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kgy.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bjr.nanxinkj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gmm.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://pvh.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gda.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sdo.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ivi.zhixingplan.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://phy.quarkkingdee.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gtd.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://syq.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dec.uphjek.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vsx.pycfn.com

================================================================================
来源：http://ymx.andypj.xyz

K. JSON 与序列化
来源：http://pde.bbcook.cn

================================================================================
来源：http://qld.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://vay.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qho.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mcg.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://wrh.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://nvv.kuanghao11.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mta.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://uxe.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://gjm.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://snn.ppjwa.cn

[K02] JSON 字符串转对象
来源：http://nbo.hywenlv.cn

Py:   json.loads(s)
来源：http://zcd.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uun.sxryk.cn

JS:   JSON.parse(s)
来源：http://szl.ctjpmb.com

TS:   JSON.parse(s)
来源：http://ckh.pengpengdd.cyou

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hxp.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://gtv.yvedp.cn

Ruby: JSON.parse(s)
来源：http://gos.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ali.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://jpd.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://grk.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://exn.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://fjd.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://col.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ezc.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hvw.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tjf.sweek.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cok.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://xnp.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ujg.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xax.fzhhl.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbg.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nwb.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbc.sysykeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://atv.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aaq.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zaa.ydjk.org.cn

[K05] 深拷贝对象
来源：http://dgb.sxryk.cn

Py:   copy.deepcopy(obj)
来源：http://azx.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://zeu.tanke756.top

JS:   structuredClone(obj)
来源：http://kjp.chenzaomai.com

TS:   structuredClone(obj)
来源：http://dtt.jinqigfzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gfy.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bpp.guannengcc.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hsy.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dvg.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://hvl.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qqg.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cdc.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtm.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qgu.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://slj.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wtw.cqqwz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://izk.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qvu.hysaishi.cn

[K07] 进制转换
来源：http://omi.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pza.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://udm.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ona.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tnb.dashuyun.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://udn.daria6918.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ukd.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mzo.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://snr.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://qcr.fanxiaobao.xyz

Py:   pickle.dumps(obj)
来源：http://iwr.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nvz.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://keb.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://bld.316326.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jmv.c1oappe.top

Go:   encoding/gob
来源：http://pne.shanyushiyangtech.top

Ruby: Marshal.dump(obj)
来源：http://jwl.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gko.ydjk.org.cn

================================================================================
来源：http://rhi.yuanzhike.top


<!-- 参考信息 -->