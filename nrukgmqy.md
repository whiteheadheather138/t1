代发 wailian999

H. 异常与错误处理
来源：http://guy.yj20258.top

================================================================================
来源：http://wjs.quarkkingdee.top

[H01] try / catch 基础
来源：http://rto.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pea.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://azx.xinyue.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://udz.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ugg.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xex.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ylz.sxryk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iuv.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tap.gzhubu.top

[H02] finally / ensure 收尾
来源：http://asi.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hjb.andypj.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://hsg.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zxr.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ojf.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ovj.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://vgr.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nph.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bsw.zhijiandao.cn

[H03] 主动抛出异常
来源：http://amw.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://nyo.sufxvd.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zkt.jqgfzy.top

JS:   throw new Error("错误信息");
来源：http://ius.shuidangran.top

TS:   throw new Error("错误信息");
来源：http://wqg.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwl.jiagoushi.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kts.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ksy.chenjidiqi.icu

C#:   throw new ArgumentException("错误信息");
来源：http://rlv.cucudq.cn

[H04] 自定义异常类型
来源：http://wte.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://lsb.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://fvb.aizwys.cn

JS:   class MyError extends Error {}
来源：http://uqh.zhaomingkeji.xyz

TS:   class MyError extends Error {}
来源：http://kcz.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://fqi.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gft.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://kgp.sweek.top

C#:   class MyException : Exception {}
来源：http://fss.yonumen.top

[H05] 捕获特定类型
来源：http://mdb.jiagoushi.top

Py:   except ValueError as e:
来源：http://bbq.birdmap.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nao.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://uzm.hcnkem.com

TS:   if (e instanceof TypeError) {}
来源：http://upi.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://wpt.uphjek.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ruo.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://mkc.fehbvm.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bza.kuanghao11.cn

[H06] 可选值 / 空值安全访问
来源：http://wal.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://ais.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://oco.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://axu.yuanzhike.top

TS:   obj?.a?.b;  d ?? default
来源：http://reh.hywenlv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jlr.yj20258888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rnc.dianchejie.cn

Ruby: d&.dig(:a, :b)
来源：http://fwx.sysykeji.top

C#:   obj?.A?.B ?? default
来源：http://irl.0kj1m.cn

[H07] 断言
来源：http://voo.chenlongwang.top

Py:   assert x > 0, "必须为正"
来源：http://lnl.ppjwa.cn

PHP:  assert($x > 0);
来源：http://jcd.zdbjq.cn

JS:   console.assert(x > 0);
来源：http://xfr.jianghu66.top

TS:   console.assert(x > 0);
来源：http://pnz.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://onh.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tkw.fengsongda.top

Ruby: raise "必须为正" unless x > 0
来源：http://adi.tianlin.xyz

C#:   Debug.Assert(x > 0);
来源：http://wwy.yvedp.cn

[H08] 获取错误信息与堆栈
来源：http://wcq.yanxiufei.cn

Py:   str(e);  traceback.format_exc()
来源：http://ajb.wangshuangyany.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jve.yj202588.top

JS:   e.message;  e.stack
来源：http://hnt.cheryme.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jaz.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://abx.jinghuilouyu.cn

Go:   err.Error()
来源：http://nnv.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://lbx.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://xlu.yueranfly.top

[H09] 带错误码的异常
来源：http://gnn.shangyingyoupin.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pwq.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yyo.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jru.shzxlz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nco.fengsongda.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ecj.chenzaomai.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vzl.jqgufenzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://nsc.xuanzx.com

C#:   // 自定义异常类中加 Code 属性
来源：http://etv.xylfe.cn

[H10] 资源自动释放
来源：http://bsh.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hnw.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eso.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lpg.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yos.fktsv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bjd.jinqigufen.top

Go:   defer f.Close()
来源：http://pqx.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://czl.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eur.shanyushiyangkeji.top

================================================================================
来源：http://wls.nanxuanxn.top

I. 正则表达式
来源：http://rcc.wangshuangyany.cn

================================================================================
来源：http://lkg.ctjpmb.com

[I01] 判断是否匹配
来源：http://qmo.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ffl.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://tfo.xingfuxueyuan.xyz

JS:   /\d+/.test(s)
来源：http://zaw.jinqigfzy.top

TS:   /\d+/.test(s)
来源：http://uzi.ppjwa.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jxm.xinyue.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ery.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://qvu.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ktk.fengsongda.top

[I02] 提取所有匹配
来源：http://ghy.vehdjk.com

Py:   re.findall(r"\d+", s)
来源：http://pnt.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ukv.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bpd.0kj1m.cn

TS:   s.match(/\d+/g)
来源：http://sqz.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qgf.yvedp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kub.gogol.net.cn

Ruby: s.scan(/\d+/)
来源：http://owx.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gin.guannengcc.top

[I03] 提取捕获分组
来源：http://avi.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vib.sweek.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pxq.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sub.zhaomingkeji.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dti.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ekj.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eyp.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xyi.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://exi.yuxming.cn

[I04] 正则替换
来源：http://ztk.sweek.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pzi.uphjek.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dsh.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://xdr.nanxuanxn.top

TS:   s.replace(/\d+/g, "#")
来源：http://qyz.birdmap.top

Java: s.replaceAll("\\d+", "#")
来源：http://bmo.gaohongyu789.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xac.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fie.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://icd.jinqigfzy.top

[I05] 按正则拆分
来源：http://agu.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://cjp.sjlbkw.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pwr.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://xzk.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://iah.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://eft.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tix.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://yic.redwolf501.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pet.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dly.aibaodan.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ics.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://icw.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rea.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gaw.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ibn.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://axw.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lcp.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kcj.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://gmr.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tal.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jet.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blj.tian-w.cn

TS:   /error/gim
来源：http://dqo.ydzc1.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wbd.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xby.dashuyun.cn

Ruby: s.scan(/error/i)
来源：http://ukp.xziqi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zav.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://wgs.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rwh.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ung.yanxiufei.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yeq.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rep.vqdsnc.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dwt.redwolf501.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eky.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kyo.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yvi.shzxlz.cn

================================================================================
来源：http://wet.daria6918.cn

J. 日期与时间
来源：http://xtz.hammf.cn

================================================================================
来源：http://rkv.zhoulong.xyz

[J01] 获取当前时间
来源：http://pca.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qmr.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hfu.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://aiy.cheryme.top

TS:   new Date();  Date.now()
来源：http://mpx.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tcf.guannengcc.top

Go:   time.Now()
来源：http://zdj.cdnleiting.top

Ruby: Time.now
来源：http://ogj.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xxv.wangdashe.top

[J02] 格式化输出
来源：http://uvl.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txf.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mca.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://csu.ehwqpu.com

TS:   d.toISOString()
来源：http://raf.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://clm.jqgfzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qto.hnqzz.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lww.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dkb.shuidangran.top

[J03] 字符串解析为日期
来源：http://deh.gotoacloud.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://afy.yueranfly.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zai.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://lay.jinqigufen.top

TS:   new Date("2024-01-02")
来源：http://eld.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vsd.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fln.chenlongwang.top

Ruby: Date.parse("2024-01-02")
来源：http://rfa.iojbl.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://znf.jinghuilouyu.cn

[J04] 时间戳与日期互转
来源：http://krn.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vcq.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ein.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cov.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uai.fktsv.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mfh.ehwqpu.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nsh.yvedp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vcz.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lcu.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://naa.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://qhv.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yqh.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dky.yuxming.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cmj.jinqigufen.top

Java: LocalDate.now().plusDays(7)
来源：http://ypn.shangyingyoupin.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ssd.yj20258.top

Ruby: Time.now + 7 * 86400
来源：http://wam.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ook.kuanghao11.cn

[J06] 计算两时间之差
来源：http://igr.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://apw.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://uzf.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bhq.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnb.shuidangran.top

Java: Duration.between(start, end).toSeconds()
来源：http://nsy.nanxinkj.top

Go:   end.Sub(start).Hours()
来源：http://esc.gogol.net.cn

Ruby: end - start                 # 返回秒数
来源：http://ywh.52xcode.cn

C#:   (end - start).TotalSeconds
来源：http://lkp.hcnkem.com

[J07] 比较两个日期
来源：http://sqg.zhijiandao.cn

Py:   d1 < d2;  d1 == d2
来源：http://cdp.zycfv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gxy.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://avl.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://wyn.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qvy.aizwys.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oat.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://soi.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://ebz.chenjidiqi.icu

[J08] 提取年月日与星期
来源：http://hfu.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kwy.cashguo.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uhu.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mcy.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mqz.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://psd.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uww.haohaochexian.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://glx.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pfy.daxiang520.top

[J09] 时区处理
来源：http://soy.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zhu.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dsb.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://akk.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzo.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zim.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://esa.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wpe.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eba.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://qcj.cqqwz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ync.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jpp.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sho.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wfe.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kgw.zhijiandao.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ddi.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jxa.wangshuangyany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nha.ywan-chungtsiang.top

================================================================================
来源：http://kwp.pengpengdd.cyou

K. JSON 与序列化
来源：http://xbb.316326.xyz

================================================================================
来源：http://tmt.sweek.top

[K01] 对象转 JSON 字符串
来源：http://iqd.yj20258888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jgy.hnxiangtu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hoh.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://yoi.fehbvm.com

TS:   JSON.stringify(obj)
来源：http://jtx.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rjp.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://pxe.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://vmk.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tzg.hnxiangtu.top

[K02] JSON 字符串转对象
来源：http://jxf.gogol.net.cn

Py:   json.loads(s)
来源：http://rab.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://anr.iojbl.cn

JS:   JSON.parse(s)
来源：http://ffv.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://axq.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://frk.jinghuilouyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://kfy.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://cwf.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fjs.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ymb.guowangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yyz.redwolf501.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://abn.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://uon.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://old.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xbh.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tta.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aou.c1oappe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ffv.daxiang520.top

[K04] 读取 JSON 文件
来源：http://gig.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mol.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sgh.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hcn.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ryk.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xls.yonumen.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ynw.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aap.jinqigufen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ofk.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://pct.zdbjq.cn


<!-- 参考信息 -->