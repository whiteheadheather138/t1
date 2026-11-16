代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nbz.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ibn.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cyq.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gaj.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qax.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zgp.hesvh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mnu.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://glc.redwolf501.top

Py:   try: f()⏎finally: cleanup()
来源：http://rbp.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uzm.cashguo.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fbk.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://spm.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://xpl.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nqz.zdbjq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://amk.fengsongda.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://dmn.sufxvd.cn

[H03] 主动抛出异常
来源：http://ocb.xuanzx.com

Py:   raise ValueError("错误信息")
来源：http://xcl.vehdjk.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ahl.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://agw.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://rza.hesvh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yfv.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iev.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://ggq.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://dsp.cheryme.top

[H04] 自定义异常类型
来源：http://zsb.tanke756.top

Py:   class MyError(Exception): pass
来源：http://nvn.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tbg.guannengcc.top

JS:   class MyError extends Error {}
来源：http://sor.cheryme.top

TS:   class MyError extends Error {}
来源：http://pux.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://eem.xziqi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqq.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://ywp.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://syu.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://ouo.tianlin.xyz

Py:   except ValueError as e:
来源：http://uax.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cek.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://mql.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://pxe.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://nox.yfazqb.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vlh.jqgufenzy.top

Ruby: rescue ArgumentError => e
来源：http://omz.dashuyun.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oix.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://qtc.wangshuangyany.cn

Py:   value = d.get("k") or default
来源：http://rtx.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tea.cqqwz.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hxh.52xcode.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ofe.zhiwuduotai.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vtq.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://obm.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://oue.xingfuxueyuan.xyz

C#:   obj?.A?.B ?? default
来源：http://ahm.sjlbkw.cn

[H07] 断言
来源：http://slk.daxiang520.top

Py:   assert x > 0, "必须为正"
来源：http://yhg.jlsjyb.cn

PHP:  assert($x > 0);
来源：http://eve.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://ziz.yongpay.top

TS:   console.assert(x > 0);
来源：http://osb.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://srw.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kzv.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://gyy.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://lur.xziqi.cn

[H08] 获取错误信息与堆栈
来源：http://aap.gzhubu.top

Py:   str(e);  traceback.format_exc()
来源：http://lmf.sweek.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://heh.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://iqo.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hlx.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://bar.fzhhl.top

Go:   err.Error()
来源：http://dyo.fengsongda.top

Ruby: e.message;  e.backtrace
来源：http://exo.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://pvi.meibo888.top

[H09] 带错误码的异常
来源：http://arp.shuidangran.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bhp.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fxi.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://itw.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wxm.zhoulong.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sbl.gotoacloud.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gqh.cheryme.top

Ruby: raise MyError.new("fail", 500)
来源：http://vlp.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://znq.sufxvd.cn

[H10] 资源自动释放
来源：http://dzx.ydzc1.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://crt.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ofn.ctjpmb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dxo.birdmap.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://spu.hnqzz.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wmx.sufxvd.cn

Go:   defer f.Close()
来源：http://pfc.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zaf.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ytk.ydzc1.top

================================================================================
来源：http://swg.nanxinkj.top

I. 正则表达式
来源：http://crb.gaohongyu789.top

================================================================================
来源：http://doq.fengsongda.top

[I01] 判断是否匹配
来源：http://fiw.andypj.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mia.hnqzz.top

PHP:  preg_match('/\d+/', $s);
来源：http://pvt.hysaishi.cn

JS:   /\d+/.test(s)
来源：http://xiy.guannengcc.top

TS:   /\d+/.test(s)
来源：http://obh.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lkv.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kor.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://bjm.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dhx.jyoumei.cn

[I02] 提取所有匹配
来源：http://lkh.yfazqb.com

Py:   re.findall(r"\d+", s)
来源：http://iab.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gzy.gogol.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rst.fanxiaobao.xyz

TS:   s.match(/\d+/g)
来源：http://jcf.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ytt.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hoc.jinqigufen.top

Ruby: s.scan(/\d+/)
来源：http://nwd.wangshuangyany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://flh.chenlongwang.top

[I03] 提取捕获分组
来源：http://bha.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aum.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xum.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bii.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rgn.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kcx.gotoacloud.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jtb.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nqp.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://puo.jqgfzy.top

[I04] 正则替换
来源：http://dyo.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://gau.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jyv.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://wzp.yj202588.top

TS:   s.replace(/\d+/g, "#")
来源：http://rgy.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://czs.jinghuilouyu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ckp.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://oyk.zhaomingkeji.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yvf.wangshuangyany.cn

[I05] 按正则拆分
来源：http://rog.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hda.zhengqikj.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jod.yj20258888.top

JS:   s.split(/\s*,\s*/)
来源：http://wlu.zhongyouzk.top

TS:   s.split(/\s*,\s*/)
来源：http://wab.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://avo.yuanzhike.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cdx.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://qna.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sxr.cashguo.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xff.ivvv.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvc.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fjx.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlb.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nln.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xim.chenjidiqi.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jbq.sxryk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sfq.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eef.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://kdk.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lmm.yj20258888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oob.cheryme.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vhh.zhijiandao.cn

TS:   /error/gim
来源：http://cvw.sysykeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uvl.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fas.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://afz.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ucw.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://zsg.jiagoushi.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wcu.tian-w.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gap.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zzs.jyoumei.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qjf.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xeo.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zqc.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mpv.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iif.gogol.net.cn

================================================================================
来源：http://urd.yuxming.cn

J. 日期与时间
来源：http://sue.shangyingyoupin.top

================================================================================
来源：http://bmo.zycfv.cn

[J01] 获取当前时间
来源：http://pjm.xziqi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bjh.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qkr.fehbvm.com

JS:   new Date();  Date.now()
来源：http://wcp.epnwcf.com

TS:   new Date();  Date.now()
来源：http://prd.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vrj.jyoumei.cn

Go:   time.Now()
来源：http://ltw.yvedp.cn

Ruby: Time.now
来源：http://mpv.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kjv.haohaochexian.top

[J02] 格式化输出
来源：http://jhq.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zyj.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://stj.tarul.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eqh.hcnkem.com

TS:   d.toISOString()
来源：http://fhp.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qkq.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qme.aizwys.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kfm.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xnc.bbcook.cn

[J03] 字符串解析为日期
来源：http://vbx.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xiu.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uby.tarul.cn

JS:   new Date("2024-01-02")
来源：http://zen.gzhubu.top

TS:   new Date("2024-01-02")
来源：http://ixc.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://dkb.hammf.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ydp.jqgfzy.top

Ruby: Date.parse("2024-01-02")
来源：http://jxt.shangyingyoupin.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hbc.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://uyv.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fmw.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wks.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://opp.hammf.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gph.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ehl.xziqi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qdu.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bsk.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yay.hcnkem.com

[J05] 时间加减（加 7 天）
来源：http://rec.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://pzh.zhengqikj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kpp.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ezy.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebc.aizwys.cn

Java: LocalDate.now().plusDays(7)
来源：http://hvt.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ygd.havefunace.top

Ruby: Time.now + 7 * 86400
来源：http://ool.jinyuanbaomall.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sou.havefunace.top

[J06] 计算两时间之差
来源：http://xvj.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://zcj.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://qyw.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kug.xingfuxueyuan.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://atq.tarul.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nsi.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://ecj.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://nhr.c1oappe.top

C#:   (end - start).TotalSeconds
来源：http://ozm.yanxiufei.cn

[J07] 比较两个日期
来源：http://odp.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://zql.shangyingyoupin.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pzm.redwolf501.top

JS:   d1.getTime() < d2.getTime()
来源：http://nuo.ybcxt.top

TS:   d1.getTime() < d2.getTime()
来源：http://xvs.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ixb.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fhs.nanxuanxn.top

Ruby: d1 < d2;  d1 == d2
来源：http://dle.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://zth.epnwcf.com

[J08] 提取年月日与星期
来源：http://eyw.quarkkingdee.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jfu.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jqg.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dnj.fengsongda.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pxj.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eps.quarkkingdee.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fsf.jyoumei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tio.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kea.0kj1m.cn

[J09] 时区处理
来源：http://ivj.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rna.tanke756.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qxm.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vzp.zhaomingkeji.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tnu.hammf.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zdl.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://glh.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qbw.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oag.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://tto.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://brk.bbcook.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wtc.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wly.sweek.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oop.jqgufenzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gmp.pengpengdd.cyou

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qpn.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bnr.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qbv.chenzaomai.com

================================================================================
来源：http://dne.daria6918.cn

K. JSON 与序列化
来源：http://yws.jqgfzy.top

================================================================================
来源：http://zyl.ydzc1.top

[K01] 对象转 JSON 字符串
来源：http://wsc.hnqzz.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yfe.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wsp.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://egu.vehdjk.com

TS:   JSON.stringify(obj)
来源：http://siv.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vom.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://rou.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://kqf.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://lmf.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://mfg.guannengcc.top

Py:   json.loads(s)
来源：http://gjh.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xuq.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://wim.guannengcc.top

TS:   JSON.parse(s)
来源：http://msa.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://amj.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://aer.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://ewn.kuanghao11.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xuq.vehdjk.com

[K03] JSON 美化输出（带缩进）
来源：http://zdg.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rty.cdnleiting.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qvz.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rwz.shanyushiyangtech.top

TS:   JSON.stringify(obj, null, 2)
来源：http://the.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://htr.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ogg.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://wwk.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wdw.hnqzz.top

[K04] 读取 JSON 文件
来源：http://rzw.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iip.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vpc.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ubo.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://htw.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://chi.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://atx.yongpay.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pfo.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://asw.vehdjk.com

[K05] 深拷贝对象
来源：http://blb.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://ovv.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://vyz.sufxvd.cn

JS:   structuredClone(obj)
来源：http://qqd.cqqwz.cn

TS:   structuredClone(obj)
来源：http://bme.snrcjt.cn


<!-- 参考信息 -->