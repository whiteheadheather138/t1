代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bmr.birdmap.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rdl.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wuu.ydjk.org.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mbw.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vev.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://elt.jinghuilouyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rld.zhengqikj.top

[H02] finally / ensure 收尾
来源：http://ckj.jinyuanbaomall.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pmd.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qqd.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zdw.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://xno.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://lkf.chenlongwang.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://uaq.ppjwa.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ryv.svipenyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://esn.feifeiyinyue.top

[H03] 主动抛出异常
来源：http://nwd.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://pyr.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pxy.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://wsv.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://nmm.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://azh.chenlongwang.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsh.xingfuxueyuan.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://zny.yuxming.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kya.52xcode.cn

[H04] 自定义异常类型
来源：http://kzl.hysaishi.cn

Py:   class MyError(Exception): pass
来源：http://yax.shzxlz.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yfi.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://vvm.vehdjk.com

TS:   class MyError extends Error {}
来源：http://eye.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://ktp.jinyuanbaomall.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://khq.jinyuanbaomall.cn

Ruby: class MyError < StandardError; end
来源：http://nva.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://wfg.cheryme.top

[H05] 捕获特定类型
来源：http://mkm.aibaodan.cn

Py:   except ValueError as e:
来源：http://fcg.gaohongyu789.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://phc.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://pvv.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://cvy.jinqigufen.top

Java: catch (IOException | SQLException e) {}
来源：http://qmw.zycfv.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rdy.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://eqi.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pqx.shangyingyoupin.top

[H06] 可选值 / 空值安全访问
来源：http://nhx.cashguo.top

Py:   value = d.get("k") or default
来源：http://wna.sufxvd.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lwp.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://jtp.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://aaw.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bvx.jiagoushi.top

Go:   if v, ok := m["k"]; ok { }
来源：http://voo.birdmap.top

Ruby: d&.dig(:a, :b)
来源：http://kdw.52xcode.cn

C#:   obj?.A?.B ?? default
来源：http://ype.yuanzhike.top

[H07] 断言
来源：http://zzc.ivvv.top

Py:   assert x > 0, "必须为正"
来源：http://oxn.hysaishi.cn

PHP:  assert($x > 0);
来源：http://bhh.cheryme.top

JS:   console.assert(x > 0);
来源：http://pvy.zhixingplan.top

TS:   console.assert(x > 0);
来源：http://fjd.zdbjq.cn

Java: assert x > 0 : "必须为正";
来源：http://gho.haohaochexian.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pxz.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://zfz.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://gfo.jlsjyb.cn

[H08] 获取错误信息与堆栈
来源：http://nyx.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://dxd.kuanghao11.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tbq.tanke756.top

JS:   e.message;  e.stack
来源：http://sky.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fkw.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://kpj.sysykeji.top

Go:   err.Error()
来源：http://epy.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://zpy.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://ruo.fehbvm.com

[H09] 带错误码的异常
来源：http://phj.hywenlv.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vsm.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://sjs.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nlu.bjfxy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ebr.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bis.hnxiangtu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xbw.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://tnm.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://eid.yanxiufei.cn

[H10] 资源自动释放
来源：http://yok.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://lwm.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ild.sjlbkw.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jzv.yj202588.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lwh.gotoacloud.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ete.sweek.top

Go:   defer f.Close()
来源：http://vgf.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://usp.yanxiufei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gpr.ywan-chungtsiang.top

================================================================================
来源：http://ctf.gzhubu.top

I. 正则表达式
来源：http://nbe.zycfv.cn

================================================================================
来源：http://vfd.cucudq.cn

[I01] 判断是否匹配
来源：http://ltz.birdmap.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nia.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://soh.dianchejie.cn

JS:   /\d+/.test(s)
来源：http://rtx.52xcode.cn

TS:   /\d+/.test(s)
来源：http://dvc.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ozh.jianghu66.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mvy.chenlongwang.top

Ruby: s.match?(/\d+/)
来源：http://qjf.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izj.vqdsnc.cn

[I02] 提取所有匹配
来源：http://soq.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://hrg.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://drq.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://adv.cashguo.top

TS:   s.match(/\d+/g)
来源：http://ysu.fehbvm.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ish.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tos.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://zoc.sysykeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pdf.jyoumei.cn

[I03] 提取捕获分组
来源：http://tgo.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://spr.52xcode.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jgf.cdnleiting.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bvy.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jch.uphjek.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zha.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dws.chenlongwang.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vah.yuanzhike.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kyi.jinyuanbaomall.cn

[I04] 正则替换
来源：http://fcm.yuxming.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sob.shuidangran.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nzp.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://grp.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cup.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://uce.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yjw.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cup.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gjl.redwolf501.top

[I05] 按正则拆分
来源：http://xrf.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qpc.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gfn.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://uuv.zycfv.cn

TS:   s.split(/\s*,\s*/)
来源：http://ugm.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://gvr.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vfo.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://uqg.xuetiantiany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tlc.tianlin.xyz

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ion.tian-w.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ycr.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sqa.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gzi.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://frh.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vpr.daxiang520.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zzq.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pds.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xke.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://lte.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hfo.wangshuangyany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fbb.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zft.zhengqikj.top

TS:   /error/gim
来源：http://vbk.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://opw.fanxiaobao.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://roa.gotoacloud.top

Ruby: s.scan(/error/i)
来源：http://djx.wangshuangyany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://szp.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://mdf.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ltw.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvd.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvu.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://amn.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://enw.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ojc.tanke756.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gve.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pdp.haohaochexian.top

================================================================================
来源：http://ubl.shanyushiyangkeji.top

J. 日期与时间
来源：http://rap.daria6918.cn

================================================================================
来源：http://zgj.epnwcf.com

[J01] 获取当前时间
来源：http://dys.zhiwuduotai.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qjw.sweek.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kbg.meibo888.top

JS:   new Date();  Date.now()
来源：http://sxx.zdbjq.cn

TS:   new Date();  Date.now()
来源：http://opm.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nta.0kj1m.cn

Go:   time.Now()
来源：http://ggf.vqdsnc.cn

Ruby: Time.now
来源：http://vit.zhaomingkeji.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ybn.jinqigfzy.top

[J02] 格式化输出
来源：http://dys.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ont.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qqh.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fnf.yj20258.top

TS:   d.toISOString()
来源：http://aam.ybcxt.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bhi.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hal.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ttq.zhijiandao.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hgd.fehbvm.com

[J03] 字符串解析为日期
来源：http://ssu.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rwg.hesvh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cpm.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://gld.vqdsnc.cn

TS:   new Date("2024-01-02")
来源：http://zwq.bbcook.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ezo.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iwg.aizwys.cn

Ruby: Date.parse("2024-01-02")
来源：http://qzt.xuanzx.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bvl.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://wcc.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ppr.svipenyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gac.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uog.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://uco.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qln.smart0.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nxu.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cfk.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zgq.gogol.net.cn

[J05] 时间加减（加 7 天）
来源：http://jcn.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://tzx.yonumen.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nik.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ojf.zdqjudy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jvz.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://njh.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qyt.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://pas.redwolf501.top

C#:   DateTime.Now.AddDays(7)
来源：http://aiq.jianghu66.top

[J06] 计算两时间之差
来源：http://lcn.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://jvk.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://nam.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hqj.zdqjudy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rst.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nzy.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://nzt.dashuyun.cn

Ruby: end - start                 # 返回秒数
来源：http://ivg.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://akn.yvedp.cn

[J07] 比较两个日期
来源：http://hgw.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://eob.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tjl.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://jsp.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uun.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ivs.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vpc.aizwys.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yqv.ybcxt.top

C#:   d1 < d2;  d1 == d2
来源：http://tai.xinyue.icu

[J08] 提取年月日与星期
来源：http://xru.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://okz.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qud.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mdp.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbo.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjw.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iux.cqqwz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ken.feifeiyinyue.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sej.ppjwa.cn

[J09] 时区处理
来源：http://dbe.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://caz.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewd.pycfn.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xmu.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ofc.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bxe.ydjk.org.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kpg.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ktw.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wsl.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://hom.vehdjk.com

Py:   date.today();  date.today().replace(day=1)
来源：http://drl.gogol.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ohe.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rew.wangshuangyany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lkz.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kcg.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://okj.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ofa.hfpthk.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gxw.aibaodan.cn

================================================================================
来源：http://oif.zdqjudy.top

K. JSON 与序列化
来源：http://fyn.jinghuilouyu.cn

================================================================================
来源：http://rls.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://ujg.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wpp.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dbi.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://zxx.yuxming.cn

TS:   JSON.stringify(obj)
来源：http://wwq.nanxinkj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mln.chenlongwang.top

Go:   json.Marshal(obj)
来源：http://cai.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://znd.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://trm.uphjek.com

[K02] JSON 字符串转对象
来源：http://wpd.quarkkingdee.top

Py:   json.loads(s)
来源：http://lio.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jwl.tanke756.top

JS:   JSON.parse(s)
来源：http://yhr.52xcode.cn

TS:   JSON.parse(s)
来源：http://pbw.cdnleiting.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tqa.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://fna.birdmap.top

Ruby: JSON.parse(s)
来源：http://vey.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sej.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://fld.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xdz.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qsg.shanyushiyangkeji.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lld.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qdb.jinghuilouyu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fyi.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vzz.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rzo.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fge.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://zlb.jinghuilouyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gns.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hwk.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sff.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fki.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zcr.hnqzz.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ihx.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://awg.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bud.ybcxt.top

[K05] 深拷贝对象
来源：http://axo.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://ilp.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://xlo.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://vvx.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://fyy.quarkkingdee.top


<!-- 参考信息 -->