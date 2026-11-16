代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jgl.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hld.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://icr.mhx1999.top

[H02] finally / ensure 收尾
来源：http://fkh.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://ase.xuanzx.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://dlb.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vvn.zdbjq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ymd.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://xxh.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oxu.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://edu.jinyuanbaomall.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vcn.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://nqs.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://gjk.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ske.jlsjyb.cn

JS:   throw new Error("错误信息");
来源：http://aqh.zhongyouzk.top

TS:   throw new Error("错误信息");
来源：http://ywu.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://exo.aizwys.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mke.aibaodan.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cde.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zby.ybcxt.top

[H04] 自定义异常类型
来源：http://tah.9152youxi.cn

Py:   class MyError(Exception): pass
来源：http://tud.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://jhy.316326.xyz

JS:   class MyError extends Error {}
来源：http://aaa.shuidangran.top

TS:   class MyError extends Error {}
来源：http://dla.vqdsnc.cn

Java: class MyException extends RuntimeException {}
来源：http://qdr.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iaz.redwolf501.top

Ruby: class MyError < StandardError; end
来源：http://djn.iojbl.cn

C#:   class MyException : Exception {}
来源：http://rwa.aizwys.cn

[H05] 捕获特定类型
来源：http://esm.nanxuanxn.top

Py:   except ValueError as e:
来源：http://zfq.hammf.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fja.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://gfy.epnwcf.com

TS:   if (e instanceof TypeError) {}
来源：http://ntb.birdmap.top

Java: catch (IOException | SQLException e) {}
来源：http://dhd.nanxuanxn.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iwf.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://uvu.mhx1999.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vxf.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://zoh.shanyushiyangkeji.top

Py:   value = d.get("k") or default
来源：http://zrn.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://rdd.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://myj.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://qql.cqqwz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kbw.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://knr.ivvv.top

Ruby: d&.dig(:a, :b)
来源：http://fbs.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://qvh.shzxlz.cn

[H07] 断言
来源：http://ady.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://ozw.sxryk.cn

PHP:  assert($x > 0);
来源：http://ros.c1oappe.top

JS:   console.assert(x > 0);
来源：http://muc.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://lwm.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://hmr.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nrn.fzhhl.top

Ruby: raise "必须为正" unless x > 0
来源：http://usp.dianchejie.cn

C#:   Debug.Assert(x > 0);
来源：http://ugj.quarkkingdee.top

[H08] 获取错误信息与堆栈
来源：http://lob.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://uvs.pengpengdd.cyou

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ify.bjfxy.top

JS:   e.message;  e.stack
来源：http://tam.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hri.bbcook.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://raw.cdnleiting.top

Go:   err.Error()
来源：http://zsf.gzhubu.top

Ruby: e.message;  e.backtrace
来源：http://lmc.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://vzg.fzhhl.top

[H09] 带错误码的异常
来源：http://kvh.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sui.yuxming.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tyr.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ycy.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vkj.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iqh.quarkkingdee.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gme.gaohongyu789.top

Ruby: raise MyError.new("fail", 500)
来源：http://amr.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ffu.zhiwuduotai.top

[H10] 资源自动释放
来源：http://ria.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mls.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iaa.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yji.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lkn.gzhubu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rqn.shuidangran.top

Go:   defer f.Close()
来源：http://nmz.zdbjq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vqd.9152youxi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dnn.yanxiufei.cn

================================================================================
来源：http://ghi.nwbrower.top

I. 正则表达式
来源：http://hrj.shangyingyoupin.top

================================================================================
来源：http://myu.svipenyu.cn

[I01] 判断是否匹配
来源：http://bcv.jinqigfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://avn.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pjr.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://tif.yueranfly.top

TS:   /\d+/.test(s)
来源：http://qsa.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qkq.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tzj.sysykeji.top

Ruby: s.match?(/\d+/)
来源：http://acl.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kye.aibaodan.cn

[I02] 提取所有匹配
来源：http://sbq.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://htp.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ydo.sxryk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://unp.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://zsl.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://haf.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://opq.bjfxy.top

Ruby: s.scan(/\d+/)
来源：http://sap.daria6918.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rxq.ydzc1.top

[I03] 提取捕获分组
来源：http://ssl.aizwys.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://umj.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sxh.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bof.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nzg.daxiang520.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bbi.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vdb.vehdjk.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://awg.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igp.hnxiangtu.top

[I04] 正则替换
来源：http://uaw.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xnb.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gyu.yuxming.cn

JS:   s.replace(/\d+/g, "#")
来源：http://huh.feifeiyinyue.top

TS:   s.replace(/\d+/g, "#")
来源：http://nva.zhixingplan.top

Java: s.replaceAll("\\d+", "#")
来源：http://ohz.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tuu.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ioi.yvedp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jho.haohaochexian.top

[I05] 按正则拆分
来源：http://qba.aizwys.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ioa.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzq.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://kkx.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://psi.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://vzq.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://srh.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://jvc.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cbi.dashuyun.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://izz.gaohongyu789.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cxd.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cem.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ecf.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gip.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fzd.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jgv.yj20258.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://obo.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jgr.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://iik.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qff.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fve.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fap.zhiwuduotai.top

TS:   /error/gim
来源：http://muk.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://igc.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hlm.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://ngu.fehbvm.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yxm.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://qwv.smart0.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cgb.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hvo.aizwys.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wmj.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qha.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://zly.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://szy.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cvf.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aye.hysaishi.cn

================================================================================
来源：http://epd.yvedp.cn

J. 日期与时间
来源：http://lvu.dianchejie.cn

================================================================================
来源：http://uhh.0kj1m.cn

[J01] 获取当前时间
来源：http://nur.shanyushiyangkeji.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nja.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drg.redwolf501.top

JS:   new Date();  Date.now()
来源：http://vnt.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://xvj.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ebh.pengpengdd.cyou

Go:   time.Now()
来源：http://pmm.fanxiaobao.xyz

Ruby: Time.now
来源：http://zng.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pcn.hammf.cn

[J02] 格式化输出
来源：http://cxo.nwbrower.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txd.gogol.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tly.mhx1999.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hxd.feifeiyinyue.top

TS:   d.toISOString()
来源：http://kxp.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fki.chenlongwang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xbz.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ylb.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xby.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://sjg.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jtb.wangdashe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qxa.shangyingyoupin.top

JS:   new Date("2024-01-02")
来源：http://cvt.shanyushiyangtech.top

TS:   new Date("2024-01-02")
来源：http://urm.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://zsq.chenlongwang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://umv.snrcjt.cn

Ruby: Date.parse("2024-01-02")
来源：http://ecw.vehdjk.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://btk.aibaodan.cn

[J04] 时间戳与日期互转
来源：http://aav.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://acr.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sqb.bbcook.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cfp.c1oappe.top

TS:   Math.floor(Date.now() / 1000)
来源：http://cjs.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://anj.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gsm.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://luk.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qch.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://fcc.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://yrb.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://abg.zdbjq.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wcf.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dql.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://bzt.daria6918.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xco.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://erc.haohaochexian.top

C#:   DateTime.Now.AddDays(7)
来源：http://bqc.tianlin.xyz

[J06] 计算两时间之差
来源：http://xze.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://zrm.jinyuanbaomall.cn

PHP:  $end->diff($start)->days;
来源：http://moh.redwolf501.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eur.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://odh.jianghu66.top

Java: Duration.between(start, end).toSeconds()
来源：http://hgc.ppjwa.cn

Go:   end.Sub(start).Hours()
来源：http://dxr.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://tni.gotoacloud.top

C#:   (end - start).TotalSeconds
来源：http://dqz.guowangkeji.top

[J07] 比较两个日期
来源：http://jij.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://ojq.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://oad.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://uwz.redwolf501.top

TS:   d1.getTime() < d2.getTime()
来源：http://pcz.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fkp.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eso.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://cmc.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://llp.aizwys.cn

[J08] 提取年月日与星期
来源：http://gvb.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vsl.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://joz.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bav.smart0.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hgi.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vgp.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://anj.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xue.hnqzz.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sld.tanke756.top

[J09] 时区处理
来源：http://qtz.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ddq.tianlin.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bqf.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gnu.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vhq.yvedp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://czv.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xwl.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://udr.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rvh.nanxuanxn.top

[J10] 取今天 / 本月第一天
来源：http://hpu.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rgj.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yho.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uyn.jinqigufen.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://szu.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hoz.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qfs.shzxlz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fzl.tian-w.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oht.zhaomingkeji.xyz

================================================================================
来源：http://yox.hfpthk.cn

K. JSON 与序列化
来源：http://qbb.pycfn.com

================================================================================
来源：http://hwq.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://psi.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kod.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dbr.quarkkingdee.top

JS:   JSON.stringify(obj)
来源：http://zwv.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://uzj.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xrd.xinyue.icu

Go:   json.Marshal(obj)
来源：http://vjn.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ees.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://tgl.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://izh.haohaochexian.top

Py:   json.loads(s)
来源：http://fbh.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://frv.uphjek.com

JS:   JSON.parse(s)
来源：http://lvg.gotoacloud.top

TS:   JSON.parse(s)
来源：http://ibz.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ogf.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://pvi.daria6918.cn

Ruby: JSON.parse(s)
来源：http://wjg.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jss.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://euk.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ayu.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pcz.guowangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kul.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://gba.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gsa.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xcj.xinyue.icu

Ruby: JSON.pretty_generate(obj)
来源：http://iif.gzhubu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pqd.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://emn.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ety.xziqi.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hrj.cdnleiting.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ium.yongpay.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://afq.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xvc.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aro.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://buv.tarul.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://din.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://ofn.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://dvg.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://ulm.chenlongwang.top

JS:   structuredClone(obj)
来源：http://fzw.andypj.xyz

TS:   structuredClone(obj)
来源：http://ltx.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pfr.xuetiantiany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lst.shzxlz.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jnq.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zfm.mhx1999.top


<!-- 参考信息 -->