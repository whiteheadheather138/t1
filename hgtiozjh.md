代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bhc.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zbi.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tng.iojbl.cn

[H02] finally / ensure 收尾
来源：http://tao.yanxiufei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://efi.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vtp.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tdt.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rol.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pvn.quarkkingdee.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bdo.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vir.smart0.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://nmp.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://vuf.ydzc1.top

Py:   raise ValueError("错误信息")
来源：http://meu.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hch.gzhubu.top

JS:   throw new Error("错误信息");
来源：http://zwb.jqgufenzy.top

TS:   throw new Error("错误信息");
来源：http://bfa.yangfankeji.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://yab.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://igo.hammf.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ejd.aizwys.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eex.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://ikm.gogol.net.cn

Py:   class MyError(Exception): pass
来源：http://oad.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hhe.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://ssy.hcnkem.com

TS:   class MyError extends Error {}
来源：http://wkq.tanke756.top

Java: class MyException extends RuntimeException {}
来源：http://jym.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://voq.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://trq.kuanghao11.cn

C#:   class MyException : Exception {}
来源：http://pvp.yvedp.cn

[H05] 捕获特定类型
来源：http://tkc.shzxlz.cn

Py:   except ValueError as e:
来源：http://nau.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://idw.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://kgd.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://dnp.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://sok.ybcxt.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dxk.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://ifz.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xar.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://xpf.gotoacloud.top

Py:   value = d.get("k") or default
来源：http://ndk.gotoacloud.top

PHP:  $v = $d["k"] ?? null;
来源：http://seq.jinqigufen.top

JS:   obj?.a?.b;  d ?? default
来源：http://wiz.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sef.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kfs.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://khi.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://qbp.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://kpw.jlsjyb.cn

[H07] 断言
来源：http://pjb.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://hcg.ppjwa.cn

PHP:  assert($x > 0);
来源：http://jyn.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://wei.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://fpw.haohaochexian.top

Java: assert x > 0 : "必须为正";
来源：http://tde.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jfo.shuidangran.top

Ruby: raise "必须为正" unless x > 0
来源：http://nvz.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://zis.jqgufenzy.top

[H08] 获取错误信息与堆栈
来源：http://fot.xinyue.icu

Py:   str(e);  traceback.format_exc()
来源：http://nqo.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pov.xingfuxueyuan.xyz

JS:   e.message;  e.stack
来源：http://mux.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://arf.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bbr.gogol.net.cn

Go:   err.Error()
来源：http://mml.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://ckv.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://ngy.ybcxt.top

[H09] 带错误码的异常
来源：http://lbd.hongshengwenyu.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://udf.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://vju.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jda.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hmy.9152youxi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yry.wangshuangyany.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://awh.chenlongwang.top

Ruby: raise MyError.new("fail", 500)
来源：http://gaq.sjlbkw.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cxi.ehwqpu.com

[H10] 资源自动释放
来源：http://syf.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uec.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wza.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ktt.ivvv.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wje.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jbs.yangfankeji.com

Go:   defer f.Close()
来源：http://kdy.hnxiangtu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zct.cdnleiting.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hak.zhengqikj.top

================================================================================
来源：http://nsr.xingfuxueyuan.xyz

I. 正则表达式
来源：http://wpb.fzhhl.top

================================================================================
来源：http://obe.chenlongwang.top

[I01] 判断是否匹配
来源：http://gks.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://edw.fanxiaobao.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://maa.jinqigufen.top

JS:   /\d+/.test(s)
来源：http://jpe.wangdashe.top

TS:   /\d+/.test(s)
来源：http://ouk.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://aji.yuxming.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cic.zhongyouzk.top

Ruby: s.match?(/\d+/)
来源：http://gdz.nanxinkj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tcs.zhiwuduotai.top

[I02] 提取所有匹配
来源：http://grq.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://ipu.hnqzz.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fde.gaohongyu789.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zpr.52xcode.cn

TS:   s.match(/\d+/g)
来源：http://mgj.guowangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vyl.meibo888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ecp.fanxiaobao.xyz

Ruby: s.scan(/\d+/)
来源：http://vqu.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://osh.vqdsnc.cn

[I03] 提取捕获分组
来源：http://wxl.52xcode.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eme.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uao.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfi.sweek.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qds.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ljg.chenlongwang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wri.andypj.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nef.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uze.bbcook.cn

[I04] 正则替换
来源：http://bmg.jyoumei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gwh.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fpe.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://oka.guannengcc.top

TS:   s.replace(/\d+/g, "#")
来源：http://teu.yuanzhike.top

Java: s.replaceAll("\\d+", "#")
来源：http://nza.pengpengdd.cyou

Go:   re.ReplaceAllString(s, "#")
来源：http://cri.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://aoh.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gyu.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://hjc.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://gtc.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hvi.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://pea.ivvv.top

TS:   s.split(/\s*,\s*/)
来源：http://tug.ctjpmb.com

Java: s.split("\\s*,\\s*")
来源：http://wcx.yonumen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ffz.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://xex.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jet.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ful.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wmh.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://szu.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcg.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jxv.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xls.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ane.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://suo.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://byk.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://vvz.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://was.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vvr.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://coz.yonumen.top

TS:   /error/gim
来源：http://yos.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vdi.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pro.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://yph.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xxl.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://hma.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imd.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rnu.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxu.zhiwuduotai.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nyf.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ckf.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://obg.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vha.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lvn.hnqzz.top

================================================================================
来源：http://klu.jyoumei.cn

J. 日期与时间
来源：http://iaj.c1oappe.top

================================================================================
来源：http://npy.hysaishi.cn

[J01] 获取当前时间
来源：http://ouj.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://efr.hysaishi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://azb.gzhubu.top

JS:   new Date();  Date.now()
来源：http://phb.sxryk.cn

TS:   new Date();  Date.now()
来源：http://rdh.yj202588.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cqn.yj20258.top

Go:   time.Now()
来源：http://ykg.dashuyun.cn

Ruby: Time.now
来源：http://ufw.sjlbkw.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rxn.sjlbkw.cn

[J02] 格式化输出
来源：http://yjy.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://voa.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ftw.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xdl.yfazqb.com

TS:   d.toISOString()
来源：http://osa.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fvy.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://unv.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjt.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pkm.9152youxi.cn

[J03] 字符串解析为日期
来源：http://ygd.cheryme.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ztc.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://krf.yongpay.top

JS:   new Date("2024-01-02")
来源：http://xtz.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://kao.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://zmc.epnwcf.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://osh.svipenyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://jgz.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qzn.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://rxa.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wxf.andypj.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xpd.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vdr.cqqwz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nkq.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gnt.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vni.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ddu.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ccp.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://fho.ywan-chungtsiang.top

Py:   now + timedelta(days=7)
来源：http://iqc.zhijiandao.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qci.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wez.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://esy.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://gov.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pik.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://duo.fktsv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kvi.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://ptk.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://epc.c1oappe.top

PHP:  $end->diff($start)->days;
来源：http://pmb.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bgq.zhoulong.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://emu.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://cvo.fktsv.cn

Go:   end.Sub(start).Hours()
来源：http://zbs.redwolf501.top

Ruby: end - start                 # 返回秒数
来源：http://ahp.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://kxm.ctjpmb.com

[J07] 比较两个日期
来源：http://cyq.cashguo.top

Py:   d1 < d2;  d1 == d2
来源：http://urq.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mfc.hfpthk.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rry.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://rlr.zhijiandao.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cfr.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eul.birdmap.top

Ruby: d1 < d2;  d1 == d2
来源：http://ysb.ppjwa.cn

C#:   d1 < d2;  d1 == d2
来源：http://fnu.vqdsnc.cn

[J08] 提取年月日与星期
来源：http://wrm.chenlongwang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://elb.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xia.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ehf.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rai.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bnn.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xhn.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mro.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aux.sufxvd.cn

[J09] 时区处理
来源：http://nlg.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wrz.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lbg.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hnk.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqs.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kdb.xinyue.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cyj.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cce.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rur.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://bkc.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://het.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kij.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rpe.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://auj.dashuyun.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yvw.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pmr.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyn.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gsp.gzhubu.top

================================================================================
来源：http://ddv.pycfn.com

K. JSON 与序列化
来源：http://eop.yongpay.top

================================================================================
来源：http://qyw.yuxming.cn

[K01] 对象转 JSON 字符串
来源：http://zfp.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hll.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gpc.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://dds.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://qnu.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ukg.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://hdx.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://ltu.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aak.redwolf501.top

[K02] JSON 字符串转对象
来源：http://ror.xylfe.cn

Py:   json.loads(s)
来源：http://wkl.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pio.tanke756.top

JS:   JSON.parse(s)
来源：http://zyp.hammf.cn

TS:   JSON.parse(s)
来源：http://iav.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zyu.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://fvf.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://nqa.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://acb.fengsongda.top

[K03] JSON 美化输出（带缩进）
来源：http://cke.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fgx.fzhhl.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ttd.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fto.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hnm.hysaishi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dpf.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nme.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://cdr.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lln.ybcxt.top

[K04] 读取 JSON 文件
来源：http://poq.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ivf.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uye.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://spi.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lec.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gny.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vdh.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ube.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tof.ehwqpu.com

[K05] 深拷贝对象
来源：http://gtj.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://udi.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://pfr.redwolf501.top

JS:   structuredClone(obj)
来源：http://hex.ehwqpu.com

TS:   structuredClone(obj)
来源：http://yzt.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uxs.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kcj.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cjf.c1oappe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zev.nwbrower.top


<!-- 参考信息 -->