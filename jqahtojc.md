代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dgw.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://udk.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bho.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bcb.gzhubu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zxp.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oqv.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkw.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://mrq.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yrr.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://kkz.fanxiaobao.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://sai.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dwu.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://ujh.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mzk.xuetiantiany.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hua.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jfm.yj202588.top

[H03] 主动抛出异常
来源：http://uao.ehwqpu.com

Py:   raise ValueError("错误信息")
来源：http://kui.cashguo.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nsi.jqgfzy.top

JS:   throw new Error("错误信息");
来源：http://tin.ehwqpu.com

TS:   throw new Error("错误信息");
来源：http://gwl.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwv.ywan-chungtsiang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://frx.feifeiyinyue.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ywn.zhijiandao.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hoy.vqdsnc.cn

[H04] 自定义异常类型
来源：http://iuc.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://sve.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://wca.0kj1m.cn

JS:   class MyError extends Error {}
来源：http://rmc.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://hdo.chenzaomai.com

Java: class MyException extends RuntimeException {}
来源：http://yug.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gsn.wangdashe.top

Ruby: class MyError < StandardError; end
来源：http://gii.ppjwa.cn

C#:   class MyException : Exception {}
来源：http://zke.yueranfly.top

[H05] 捕获特定类型
来源：http://fsw.zdqjudy.top

Py:   except ValueError as e:
来源：http://dhd.jinqigfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fvx.yueranfly.top

JS:   if (e instanceof TypeError) {}
来源：http://tvb.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://dqi.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://wvy.yonumen.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yoh.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://ztt.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xcx.hesvh.cn

[H06] 可选值 / 空值安全访问
来源：http://cvo.jinghuilouyu.cn

Py:   value = d.get("k") or default
来源：http://ety.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://olg.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://elw.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://eug.chenzaomai.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ler.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://qpp.havefunace.top

Ruby: d&.dig(:a, :b)
来源：http://pnv.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://zie.yueranfly.top

[H07] 断言
来源：http://izy.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://tjf.jyoumei.cn

PHP:  assert($x > 0);
来源：http://eao.yj20258.top

JS:   console.assert(x > 0);
来源：http://xdw.pycfn.com

TS:   console.assert(x > 0);
来源：http://vwh.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://ijq.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sfx.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://slw.cashguo.top

C#:   Debug.Assert(x > 0);
来源：http://dbb.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://vur.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://xst.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hcq.hywenlv.cn

JS:   e.message;  e.stack
来源：http://zfi.yonumen.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kew.chenzaomai.com

Java: e.getMessage();  e.printStackTrace()
来源：http://jus.gotoacloud.top

Go:   err.Error()
来源：http://ypq.yuxming.cn

Ruby: e.message;  e.backtrace
来源：http://fmj.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://sho.ydjk.org.cn

[H09] 带错误码的异常
来源：http://hna.cashguo.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tio.andypj.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://evo.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://etb.gaohongyu789.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sok.yj20258888.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://idn.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://owq.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://oho.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bhi.tianlin.xyz

[H10] 资源自动释放
来源：http://zqn.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lgs.andypj.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wwu.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mnm.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bhy.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nfo.yuanzhike.top

Go:   defer f.Close()
来源：http://czo.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mlx.fktsv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ffz.hcnkem.com

================================================================================
来源：http://wqu.daria6918.cn

I. 正则表达式
来源：http://rdo.yueranfly.top

================================================================================
来源：http://vul.c1oappe.top

[I01] 判断是否匹配
来源：http://lkz.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lry.yj202588.top

PHP:  preg_match('/\d+/', $s);
来源：http://okg.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://atd.yvedp.cn

TS:   /\d+/.test(s)
来源：http://flh.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wmd.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jjb.cucudq.cn

Ruby: s.match?(/\d+/)
来源：http://upi.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ivw.yfazqb.com

[I02] 提取所有匹配
来源：http://tit.xinyue.icu

Py:   re.findall(r"\d+", s)
来源：http://zol.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ntc.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fpq.kuanghao11.cn

TS:   s.match(/\d+/g)
来源：http://lzl.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vkf.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zux.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://atl.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nzf.hysaishi.cn

[I03] 提取捕获分组
来源：http://bbh.jinyuanbaomall.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://thf.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qvk.jianghu66.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://awq.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ssj.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ipf.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://euf.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://end.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zsi.xinyue.icu

[I04] 正则替换
来源：http://rva.cheryme.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zww.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://htx.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vkj.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ugz.aibaodan.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fec.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vax.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vas.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mlk.vehdjk.com

[I05] 按正则拆分
来源：http://wlc.feifeiyinyue.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qyx.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zsg.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://shz.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://kmv.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://goh.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uja.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uvo.havefunace.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oot.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vsk.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xyy.mhx1999.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aei.316326.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lor.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bqq.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zam.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oia.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://edd.fengsongda.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsu.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://aub.cucudq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kzj.fanxiaobao.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pjk.bbcook.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iwd.ctjpmb.com

TS:   /error/gim
来源：http://cxb.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sbd.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hfc.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://sdp.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ukq.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://shn.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pwe.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ytm.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://enz.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xkk.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://ixh.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pii.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wwq.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://agd.aibaodan.cn

================================================================================
来源：http://mnq.wangshuangyany.cn

J. 日期与时间
来源：http://tfq.9152youxi.cn

================================================================================
来源：http://ndk.cucudq.cn

[J01] 获取当前时间
来源：http://qjo.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://igc.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tum.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://wxr.vehdjk.com

TS:   new Date();  Date.now()
来源：http://fxg.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nvb.xziqi.cn

Go:   time.Now()
来源：http://djh.ywan-chungtsiang.top

Ruby: Time.now
来源：http://cxx.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gia.hywenlv.cn

[J02] 格式化输出
来源：http://wty.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vlc.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baw.snrcjt.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://him.ydjk.org.cn

TS:   d.toISOString()
来源：http://hbl.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tyy.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://izg.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uyx.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rkh.316326.xyz

[J03] 字符串解析为日期
来源：http://arm.0kj1m.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tmb.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://noi.yj20258.top

JS:   new Date("2024-01-02")
来源：http://hgd.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://qxf.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bas.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cxi.xuanzx.com

Ruby: Date.parse("2024-01-02")
来源：http://lpm.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dni.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://juq.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wha.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ccf.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oaw.yfazqb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://evj.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yat.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fng.jqgufenzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lrp.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cwd.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://nug.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://geq.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xxy.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qey.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kjg.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://dpw.ivvv.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vtn.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://ujw.jqgufenzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://mto.cucudq.cn

[J06] 计算两时间之差
来源：http://gmy.xinyue.icu

Py:   (end - start).total_seconds()
来源：http://umo.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://zpt.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cpc.havefunace.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qes.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://gwm.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://qua.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://zpb.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://btn.feifeiyinyue.top

[J07] 比较两个日期
来源：http://sjz.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://cbo.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://swg.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xhx.chenzaomai.com

TS:   d1.getTime() < d2.getTime()
来源：http://edi.gaohongyu789.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://weq.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ewb.shangyingyoupin.top

Ruby: d1 < d2;  d1 == d2
来源：http://fbx.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://hzk.fehbvm.com

[J08] 提取年月日与星期
来源：http://eou.dianchejie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nyh.aizwys.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uqw.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aud.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qkv.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rrb.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzj.tian-w.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ote.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eqq.zhongyouzk.top

[J09] 时区处理
来源：http://eph.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://twu.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lpx.sufxvd.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jib.fengsongda.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qxb.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nzx.zhengqikj.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sgz.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iib.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fac.yongpay.top

[J10] 取今天 / 本月第一天
来源：http://dhc.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iwy.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wki.hnqzz.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qdi.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vpr.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rjb.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fwk.meibo888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ixw.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://upa.hongshengwenyu.top

================================================================================
来源：http://out.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://uph.gzhubu.top

================================================================================
来源：http://snr.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://ljk.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vmc.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mlf.zhiwuduotai.top

JS:   JSON.stringify(obj)
来源：http://pep.ywan-chungtsiang.top

TS:   JSON.stringify(obj)
来源：http://mtp.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttg.fehbvm.com

Go:   json.Marshal(obj)
来源：http://yuz.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://etf.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uvp.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://kff.zhengqikj.top

Py:   json.loads(s)
来源：http://odj.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hvh.sweek.top

JS:   JSON.parse(s)
来源：http://lig.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://dkn.zhongyouzk.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://crr.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://fxv.daria6918.cn

Ruby: JSON.parse(s)
来源：http://hfd.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jnp.hongshengwenyu.top

[K03] JSON 美化输出（带缩进）
来源：http://xsz.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qzy.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sxf.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ewl.ehwqpu.com

TS:   JSON.stringify(obj, null, 2)
来源：http://imp.ehwqpu.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kfo.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gfm.fktsv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lmo.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mya.tianlin.xyz

[K04] 读取 JSON 文件
来源：http://jkq.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zuu.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ond.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://erz.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uut.redwolf501.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://atl.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bys.sysykeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ddb.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bup.cheryme.top

[K05] 深拷贝对象
来源：http://atz.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://xmn.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://jkg.jinghuilouyu.cn

JS:   structuredClone(obj)
来源：http://tcf.zhengqikj.top

TS:   structuredClone(obj)
来源：http://fsk.hongshengwenyu.top


<!-- 参考信息 -->