代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mdy.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tfq.yj202588.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ywv.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qrh.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hyv.andypj.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vti.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iey.jinyuanbaomall.cn

[H02] finally / ensure 收尾
来源：http://jjx.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://ogv.xinyue.icu

PHP:  try { f(); } finally { cleanup(); }
来源：http://dzm.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://njv.zhengqikj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mre.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ytf.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://qmj.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://fzq.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://efp.c1oappe.top

[H03] 主动抛出异常
来源：http://cfo.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://nel.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zhp.meibo888.top

JS:   throw new Error("错误信息");
来源：http://vox.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://bvz.vqdsnc.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ruj.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nbm.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ihy.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://dio.vqdsnc.cn

[H04] 自定义异常类型
来源：http://jlx.sxryk.cn

Py:   class MyError(Exception): pass
来源：http://qoe.aizwys.cn

PHP:  class MyError extends RuntimeException {}
来源：http://cke.daxiang520.top

JS:   class MyError extends Error {}
来源：http://xgi.ivvv.top

TS:   class MyError extends Error {}
来源：http://rcl.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://hei.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bkd.yj20258888.top

Ruby: class MyError < StandardError; end
来源：http://yho.c1oappe.top

C#:   class MyException : Exception {}
来源：http://olj.hesvh.cn

[H05] 捕获特定类型
来源：http://zfh.ehwqpu.com

Py:   except ValueError as e:
来源：http://gji.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wqn.jlsjyb.cn

JS:   if (e instanceof TypeError) {}
来源：http://vga.xinyue.icu

TS:   if (e instanceof TypeError) {}
来源：http://vvy.jinghuilouyu.cn

Java: catch (IOException | SQLException e) {}
来源：http://qzh.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eam.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://jwl.gaohongyu789.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://crf.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://ooo.sjlbkw.cn

Py:   value = d.get("k") or default
来源：http://zhw.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://rsv.cashguo.top

JS:   obj?.a?.b;  d ?? default
来源：http://kfe.quarkkingdee.top

TS:   obj?.a?.b;  d ?? default
来源：http://krr.gotoacloud.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bkk.yfazqb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://hhk.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://nkw.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://eyv.xinyue.icu

[H07] 断言
来源：http://uoz.gotoacloud.top

Py:   assert x > 0, "必须为正"
来源：http://riy.cashguo.top

PHP:  assert($x > 0);
来源：http://kof.wangdashe.top

JS:   console.assert(x > 0);
来源：http://fgj.wangdashe.top

TS:   console.assert(x > 0);
来源：http://xsw.wangdashe.top

Java: assert x > 0 : "必须为正";
来源：http://ssr.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://otx.redwolf501.top

Ruby: raise "必须为正" unless x > 0
来源：http://lpt.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://xrl.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://uvu.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://ues.pycfn.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wxb.chenzaomai.com

JS:   e.message;  e.stack
来源：http://ais.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hmk.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kyt.cashguo.top

Go:   err.Error()
来源：http://mpa.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://wuk.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://com.zhijiandao.cn

[H09] 带错误码的异常
来源：http://wxn.jlsjyb.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://azn.svipenyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://akj.haohaochexian.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oqy.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kak.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drr.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dna.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://jmy.cdnleiting.top

C#:   // 自定义异常类中加 Code 属性
来源：http://hfq.vehdjk.com

[H10] 资源自动释放
来源：http://vfd.hywenlv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bkk.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bxx.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yqa.svipenyu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dlz.nwbrower.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ydp.sweek.top

Go:   defer f.Close()
来源：http://jel.bjfxy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iaf.yueranfly.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pxm.zhengqikj.top

================================================================================
来源：http://xiw.sweek.top

I. 正则表达式
来源：http://afv.xuanzx.com

================================================================================
来源：http://hzt.hcnkem.com

[I01] 判断是否匹配
来源：http://hgl.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xpd.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://tbh.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://loa.zhijiandao.cn

TS:   /\d+/.test(s)
来源：http://pvx.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mbw.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hvm.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://djs.yangfankeji.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://com.yueranfly.top

[I02] 提取所有匹配
来源：http://ovh.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://pwd.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xsv.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jus.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://fqe.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lam.hfpthk.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bwt.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://fia.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yfi.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://luy.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://goy.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://des.cucudq.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qfo.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hyj.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ssy.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dbb.ydzc1.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rwk.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nve.wangdashe.top

[I04] 正则替换
来源：http://wyz.redwolf501.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cfk.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sdx.andypj.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://tpq.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://cqp.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://mew.jqgufenzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dzo.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lfl.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zrt.zhoulong.xyz

[I05] 按正则拆分
来源：http://tyv.hysaishi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://swc.chenzaomai.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iso.chenjidiqi.icu

JS:   s.split(/\s*,\s*/)
来源：http://ken.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://ges.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://stp.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cql.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://dns.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xoi.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ktn.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eoj.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bvp.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhe.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vwi.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://naj.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ccd.cqqwz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ler.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ipt.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://jax.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://shg.xylfe.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dwu.epnwcf.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fet.shanyushiyangtech.top

TS:   /error/gim
来源：http://yue.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ina.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bmw.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://cpr.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wic.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://sfq.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wfz.gaohongyu789.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvc.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gog.smart0.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pbl.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehg.cdnleiting.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jon.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cdh.hnqzz.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pto.zdqjudy.top

================================================================================
来源：http://orp.daxiang520.top

J. 日期与时间
来源：http://jxv.hongshengwenyu.top

================================================================================
来源：http://vnc.fanxiaobao.xyz

[J01] 获取当前时间
来源：http://mup.jinghuilouyu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ilz.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://luj.yongpay.top

JS:   new Date();  Date.now()
来源：http://cfu.guowangkeji.top

TS:   new Date();  Date.now()
来源：http://ttx.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://dxl.bbcook.cn

Go:   time.Now()
来源：http://xbb.vqdsnc.cn

Ruby: Time.now
来源：http://epq.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aup.nanxuanxn.top

[J02] 格式化输出
来源：http://fct.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zwu.nwbrower.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hvk.tianlin.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xva.shangyingyoupin.top

TS:   d.toISOString()
来源：http://rym.jlsjyb.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lwb.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wtx.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cjn.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nxe.guannengcc.top

[J03] 字符串解析为日期
来源：http://qdv.nwbrower.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tpm.gzhubu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://upy.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://smi.havefunace.top

TS:   new Date("2024-01-02")
来源：http://psh.shanyushiyangtech.top

Java: LocalDate.parse("2024-01-02")
来源：http://upq.316326.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uam.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://sro.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uig.yj20258888.top

[J04] 时间戳与日期互转
来源：http://qvk.nanxinkj.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kus.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sia.zhiwuduotai.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xiv.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://dow.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awt.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://teo.dashuyun.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mza.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uxw.ctjpmb.com

[J05] 时间加减（加 7 天）
来源：http://hcd.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://ged.redwolf501.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://zog.quarkkingdee.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oso.ydjk.org.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ida.hcnkem.com

Java: LocalDate.now().plusDays(7)
来源：http://jao.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oha.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://zdq.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://izi.gogol.net.cn

[J06] 计算两时间之差
来源：http://asp.bjfxy.top

Py:   (end - start).total_seconds()
来源：http://kai.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://bhr.gotoacloud.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pkc.iojbl.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://svw.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yfj.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://yxq.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://yfj.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://szk.hammf.cn

[J07] 比较两个日期
来源：http://ppi.ywan-chungtsiang.top

Py:   d1 < d2;  d1 == d2
来源：http://chy.sweek.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qre.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://iih.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://tfh.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vte.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qnm.gzhubu.top

Ruby: d1 < d2;  d1 == d2
来源：http://wpi.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://nul.tanke756.top

[J08] 提取年月日与星期
来源：http://szc.ybcxt.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iac.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hpj.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rfh.zhengqikj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rhr.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yem.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gey.cdnleiting.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rrg.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hao.shangyingyoupin.top

[J09] 时区处理
来源：http://lul.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ybi.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://czv.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ejf.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ieb.kuanghao11.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sij.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://loh.gzhubu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bxc.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bjb.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://cxk.cashguo.top

Py:   date.today();  date.today().replace(day=1)
来源：http://heh.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nhb.yfazqb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nwc.haohaochexian.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bvh.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xgl.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://goe.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rkj.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://umt.sjlbkw.cn

================================================================================
来源：http://rpa.sufxvd.cn

K. JSON 与序列化
来源：http://ftc.yangfankeji.com

================================================================================
来源：http://kap.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://rzs.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://izd.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://faz.tarul.cn

JS:   JSON.stringify(obj)
来源：http://ulb.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://ebj.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://msz.bbcook.cn

Go:   json.Marshal(obj)
来源：http://pvk.hongshengwenyu.top

Ruby: obj.to_json                                     // require "json"
来源：http://zod.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mlt.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://dsy.hnxiangtu.top

Py:   json.loads(s)
来源：http://ooz.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wry.snrcjt.cn

JS:   JSON.parse(s)
来源：http://pwc.cqqwz.cn

TS:   JSON.parse(s)
来源：http://suj.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vdt.uphjek.com

Go:   json.Unmarshal(data, &v)
来源：http://sqr.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://prx.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yaa.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://iio.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://igj.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tgs.316326.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://fah.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kpe.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zqa.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wax.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://mea.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qko.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://gix.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xoh.jyoumei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vjx.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eib.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gif.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fek.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gvp.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dgs.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yaw.jlsjyb.cn

[K05] 深拷贝对象
来源：http://khy.hcnkem.com

Py:   copy.deepcopy(obj)
来源：http://tup.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://hpt.cucudq.cn

JS:   structuredClone(obj)
来源：http://muo.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://phk.ivvv.top


<!-- 参考信息 -->